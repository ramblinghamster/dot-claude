---
name: batch-image-generator
description: >
  Use when the user wants to batch-generate multiple image concepts across styles and
  actually render them into images (not just build prompt text) via the OpenAI Images
  API pipeline at /Users/cavittca/chatgpt-batch. Trigger on: "generate N prompts in
  different styles and batch-generate them", "batch generate images", "give me N styles
  and render Y images per prompt", "run my batch process for these", "request images
  for both the robust and compact prompts". Requires Claude Code (Bash tool + local
  OPENAI_API_KEY + local venv) — do NOT trigger in the claude.ai web sandbox, it has no
  access to the local script, key, or filesystem this depends on.
---

# Batch Image Generator

Orchestrates two things that already work independently:
- **image-prompt-builder** — builds prompt text (the 8-Block framework)
- **/Users/cavittca/chatgpt-batch/generate.py** — renders images via the OpenAI Images
  API (gpt-image-1), grouped by concept, distinguishing robust vs compact variants

This skill exists to chain them for a real batch: N concepts × styles → real image files
on disk, organized and labeled, without manual copy-pasting per prompt.

**Requires Claude Code.** This shells out to a local Python venv and reads a local
`OPENAI_API_KEY` from the environment. It cannot run in the web/claude.ai sandbox.

## Workflow

### 1. Clarify scope (if the user didn't already specify)
- How many concepts/styles (e.g. "10 different styles")
- Images per prompt variant — default 4
- Quality tier — default `medium`
- Whether to confirm each concept's 8 blocks individually (image-prompt-builder's normal
  flow) or batch-confirm all concepts at once before generating text (recommended for
  N > 3 — confirming one at a time for 10 concepts is slow; ask the user which they want)

### 2. Generate prompt text via image-prompt-builder
For each concept, run image-prompt-builder's normal flow (Path A or B, block confirmation
included) to produce all four prompt variants. **Only two of the four are used here:**
- `ChatGPT Prompt — Robust`
- `ChatGPT Prompt — Compact`

(Niji Journey Robust/Compact are irrelevant to this pipeline — the OpenAI API doesn't take
Niji-style prompts.) Extract the literal text inside the fenced code block under each of
those two headings — do not paraphrase or re-summarize it.

### 3. Assemble the batch input file
Build a JSON array with **two entries per concept** (one `robust`, one `compact`), matching
the schema `generate.py` expects:

```json
{
  "group": ["01-Concept Name", "Sumi-e"],
  "variant": "robust",
  "orientation": "landscape",
  "prompt": "<exact ChatGPT Prompt — Robust text>"
}
```

`group` is a list of folder-path segments (outermost first) — for a flat batch this is
usually just `[concept_label, style]`, but it supports arbitrary nesting (e.g.
`[category, subgroup, style]` for a lookbook-style batch spanning categories). `generate.py`
slugifies each segment and nests folders accordingly, so richer groupings from other
sources (a category/theme document, etc.) work without any script changes.

`orientation` must be one of `square` / `landscape` / `portrait` — infer it from the
scene's composition (wide environment shot → landscape, character close-up → portrait,
centered/symmetrical → square). These map to the only three fixed sizes GPT-Image
actually supports; there's no free aspect-ratio control.

Write the array to a fresh timestamped run folder, e.g.
`/Users/cavittca/chatgpt-batch/runs/2026-07-12-1900/prompts.json` — never overwrite a
previous run's file.

### 4. State the cost estimate and confirm before spending money
Total images = concepts × 2 variants × count-per-variant. Estimate using:
`low` ≈ $0.02/image, `medium` ≈ $0.07/image, `high` ≈ $0.19/image.
State the total estimate and get explicit confirmation before running — this charges the
user's real OpenAI balance.

### 5. Run the batch script
```bash
cd /Users/cavittca/chatgpt-batch && source .venv/bin/activate && source ~/.zshrc && \
python generate.py \
  --input runs/<run>/prompts.json \
  --output-dir runs/<run>/output \
  --count <N> \
  --quality <tier>
```
Never echo `$OPENAI_API_KEY` or print any part of its value in a command.

### 6. Report results organized by concept
Output lands as `runs/<run>/output/<slugified group path>/robust_01.png ... robust_0N.png`
and `compact_01.png ... compact_0N.png` — one folder per group (nested per the `group` path
given), robust and compact kept as clearly distinct filename groups within it (never merge
or renumber them together).

Summarize back to the user per concept: style, folder path, image counts for robust vs
compact, and surface any `FAIL` lines from the script's output rather than hiding them —
`generate.py` already continues past individual failures instead of aborting the run.
Re-running the same `--input`/`--output-dir` pair is safe and resumable: entries whose
expected image count already exists on disk are skipped automatically.
