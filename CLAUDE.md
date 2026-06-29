# Claude Session Context

## Image Prompt Builder Skill

A custom image generation prompt skill built using the 8-Block Visual Prompt Anatomy Framework.
Targets ChatGPT (DALL-E 3) and Niji Journey 7, producing 4 prompt variants per session.

### File Locations

| Purpose | Path |
|---|---|
| Source of truth | `~/.claude/skills/image-prompt-builder/` |
| Live Claude Code location | `~/Library/Application Support/Claude/local-agent-mode-sessions/skills-plugin/0c10f75f-df4f-4793-821e-f46266595e95/200a7c70-cef9-4012-ba07-6a4f500167a1/skills/image-prompt-builder/` |
| Web upload zip | `~/.claude/skills/image-prompt-builder.zip` |

### Key Files

- `SKILL.md` — core skill, always loaded, contains 34-style quick reference table
- `references/styles.md` — all 34 styles with ChatGPT and Niji Journey translations
- `references/style-guide.md` — style descriptions, category table, concept→style lookup
- `references/character-sheet.md` — 12-panel production reference sheet spec
- `references/inspirations.md` — 5 example scenes per style (145 total), add new ones on request

### Current Styles (34)

Sumi-e · Crewdson · Neon Noir · Editorial Fashion · Studio Ghibli · Dark Fantasy ·
Ember · Prism · Aquarelle · Ironbloom · Makoto Shinkai · Ufotable · Retro Anime ·
Cel Shading · Soulslike · Miura · JRPG Pixel Art · Shounen Burst ·
Moe Gacha · Webtoon · Storybook · Storybook Impasto · Gacha Splash ·
Cinematic Anime · Hyperreal Anime · Daily Chibi · Velvet · Gossamer ·
Flat Cel · Flat Chibi · Sketch Moe · Pixiv Clean · Colored Pencil · Pencil Sketch

### Sync Workflow

After editing any file in `~/.claude/skills/image-prompt-builder/`:

1. Run `imgprompt-sync` in terminal (syncs to live Claude Code location, removes any v2 ghost)
2. Rebuild zip for web upload:
```bash
cd ~/.claude/skills/image-prompt-builder && zip ~/.claude/skills/image-prompt-builder.zip SKILL.md references/styles.md references/style-guide.md references/character-sheet.md references/inspirations.md -j
```
3. Upload zip to claude.ai to update the web skill

### Known Gotchas

- **`imgprompt-sync` alias is MISSING from `~/.zshrc`** — needs to be recreated. Until then, sync manually by copying all 5 files from `~/.claude/skills/image-prompt-builder/` to the live Library path (SKILL.md, and references/styles.md, style-guide.md, character-sheet.md, inspirations.md → flat into live dir)
- Niji Journey translations use `--ar` only — `--niji` and `--style` params removed (incompatible with Niji 7). SKILL.md compliance check also updated to strip these if present
- The manifest.json at the live location controls which skills appear — no v2 ghost entries currently present
- Web environment uses `/mnt/skills/user/` not `~/.claude/` — skill references files by name only (flat zip structure)
- `~/.claude/skills/` is the edit location; the Library path is the runtime location
- All styles now require anime anchoring in ChatGPT translations — enforced and verified as of this session
- No style should use "photorealistic" language — "semi-realistic" is acceptable

### Adding a New Style

1. Append entry to `references/styles.md` (follow existing format — Visual Description, ChatGPT Translation, Niji Journey Translation)
2. Add description to `references/style-guide.md` (category section + lookup table row)
3. Add row to style table in `SKILL.md` (update count too)
4. Add 5 inspiration scenes to `references/inspirations.md`
5. Run sync workflow above
