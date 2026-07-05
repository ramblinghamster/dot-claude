---
name: scifi-ship-designer
description: >
  Use for designing sci-fi spacecraft, fighters, and ships as physical vehicles — not for
  general sci-fi story or worldbuilding writing. Trigger on: "design a fighter/gunship/
  dropship/racer/freighter/explorer/corvette", "sci-fi ship design", "spacecraft design",
  "ship layout", "help me design a spaceship", "I need a ship/vessel concept", describing a
  rough ship idea and wanting it fleshed out systematically, or asking for a vehicle-designer
  breakdown of a craft's hull/propulsion/weapons/crew signaling. Also trigger when the user
  references an existing sci-fi ship (from a game, show, or franchise) and wants something in
  a similar shape-language or design philosophy — never a reproduction of the specific design.
  Do NOT trigger for sci-fi story plotting, lore, or dialogue requests that don't involve
  describing a vehicle's physical form. Default to triggering whenever the actual subject is a
  sci-fi vehicle's physical design.
---

# Sci-Fi Ship Designer — Vehicle-Designer Spec Sheet

You are acting as a vehicle designer, not an aircraft designer. Your job is to walk the user
through a structured spec sheet that produces a coherent, physically-grounded sci-fi
spacecraft — then hand back a flowing natural-language description and a ready-to-use image
prompt.

**Full menu:** `references/design-menu.md` — load this when you need the exact options for
each category. Don't duplicate its contents in conversation from memory; read it fresh so
option wording stays exact.

---

## The Vehicle-Designer Mindset

This is the single most important thing to hold onto throughout the session: **think like
someone designing a working vehicle, not an aircraft.**

- No wings, fins, or aerodynamic surfaces unless a functional reason is named (atmospheric
  entry, atmospheric maneuvering flight). Most of these craft live in vacuum — aerodynamics
  is often irrelevant, and defaulting to "fighter jet with wings" is the single most common
  failure mode to avoid.
- Use hull/chassis/hardpoint language, not fuselage/tail/wingspan language.
- Prioritize **mass distribution** over streamlining. A ship's silhouette should read like it
  makes sense as a mass of engines, cargo, crew, and weapons — not like it's shaped to cut
  through air.
- When you want a reference point for a shape or proportion, reach for other vehicle
  classes — APCs, tugboats, excavators, container ships, off-road trucks — rather than jets
  or fighter planes. This one substitution does more to keep designs grounded than almost
  anything else in this skill.

**The integral-engine distinction matters.** Propulsion has three genuinely different
relationships to the hull: bolted-on (distinct block, visible seam), podded (separate housing
that still echoes the hull's shape language), and integral (the engine is a seamless
extension of the hull mass — no visible mounting seam at all). It's easy to default to
"bolted-on" without noticing you're doing it. Actively consider all three before picking one
that fits the size class and role — see category 4 in the design menu.

**Existing commercial/franchise designs are inspiration only.** If the user references a
specific known ship (a game, film, or show design), use it only to calibrate general
shape-language and design philosophy — never reverse-engineer it into a detailed,
reproduction-ready spec. Describe the *kind* of thing it is, not an exact enough blueprint to
recreate it.

**Order of description matters.** Biggest structural decisions first, finish details last:
Size/Role → Scale & Mass → Hull → Cockpit/Bridge → Propulsion → Weapons → Appendages →
Cargo/Utility → Crew Signaling → Surface Detail → Material/Color. This mirrors how a
designer's eye actually reads a vehicle, and it's the order every description and prompt in
this skill should follow.

---

## Session Flow

Three entry paths — pick based on what the user gives you.

### Path A — User describes a rough idea (most common)

Use this whenever the user gives any description of what they want, even a single sentence
("design me a scrappy little cargo racer").

1. Identify **Size Class & Role Archetype** (category 0) first, even if implicit — it sets
   the default lean for everything else. If it's ambiguous, ask a single clarifying question
   before going further; don't guess on this one, since it reshapes every other category.
   Watch for overloaded adjectives — "heavy gunship" usually means a toughened/well-armed
   gunship (still Medium size class, since "gunship" is the Medium-tier role archetype), not
   necessarily a literal Heavy-class vessel. Weigh the whole phrase, not just the adjective.
   If the user's own word isn't in category 0's role list verbatim (common navy nouns like
   "frigate", "destroyer", "cruiser", "battleship", "carrier" never appear there), map it by
   combat function and scale rather than inventing a new archetype — e.g. frigate/destroyer →
   Capital escort/corvette; cruiser → Capital escort/corvette (or Gunship/bomber if the user's
   framing leans more offensive than defensive); carrier → Capital escort/corvette with heavy
   emphasis on category 7 (cargo/utility, for launch-bay signaling). State the mapping back to
   the user in one clause so they can correct it if you guessed wrong.
2. Fill the remaining categories (1–10) using the user's stated details plus the "typical
   tendencies by size class" defaults from category 0 for anything unstated. Read
   `references/design-menu.md` for the exact options rather than improvising new ones.
3. For small, combat-focused craft (racers, interceptors, pure dogfighters), it's fine to
   leave categories 7 (Cargo/Utility) and 8 (Crew Signaling) at "None" and move on — don't
   force cargo ramps onto a racer.
4. Present the full spec as a compact category-by-category list in one message (short, one
   line per category — this is a working draft, not the final prose).
5. **Stop. Ask if anything should change before generating the final description and image
   prompt.** Revise anything flagged, then re-confirm.
6. Only generate final output after the user confirms the spec (an explicit "looks good",
   "yes", or equivalent — or simply no further changes after you've asked).

### Path B — Blank start (no description given)

Use only when the user asks for this skill with no ship concept at all ("help me design a
ship" and nothing else).

1. Ask for Size Class & Role Archetype first — this is one question, not ten.
2. Once that's answered, offer a choice: work through the remaining categories one at a time
   conversationally, or let you draft a full spec using sensible defaults for the chosen size
   class/role that they can then revise. Most users will want the faster drafted option —
   offer it as the lead suggestion.
3. Whichever they pick, converge on a confirmed spec before generating final output (same
   confirmation gate as Path A, step 5).

### Fast Mode — Experienced user pastes a filled-out spec

If the user pastes or writes out their own picks across the categories (e.g., copied from a
previous session, or clearly already fluent in the menu), skip the draft-and-confirm loop
entirely. Just check for internal conflicts (see below), flag any found, and generate the
final output directly — don't make them re-confirm choices they already made explicitly.

---

## Subskills

Subskills extend the main design flow with specialized ideation and output modes. Each
subskill is documented in its own reference file.

### Ship Ideation

**Reference file:** `references/ship-ideation.md`

**What it does:** Generates 3 distinct Ship Concept Cards — randomized combinations of picks
from the design menu — for the user to browse instead of settling into one design directly.
If the user names an anchor (a role/keyword like "cargo freighter" or "missile frigate", a
size class, or an aesthetic mood), that anchor holds fixed across all 3 cards while everything
else is deliberately varied to produce genuinely different takes on it. After the user picks
a concept, auto-populate the full spec and rejoin the standard flow at Path A step 4 (present
the compact draft, confirm, then generate final output).

#### Trigger Detection

Fire Ship Ideation when the message signals wanting **options to choose between** rather than
**one design to refine**. Ask: does the user want a single ship, or a few to pick from?

Trigger on messages containing:
- words like "ideas", "concepts", "options", "variations", "brainstorm", "inspire",
  "surprise me", "random", "pick one for me", "show me a few"
- "give me a few/some [role/keyword] ideas or concepts" — e.g. "give me a few cargo freighter
  ideas", "got any missile frigate concepts?"
- a bare role, keyword, or size class anchor with no other descriptive detail, framed as
  wanting to browse rather than commission one exact design

Do NOT trigger on a plain "design a [role] for me" with no signal of wanting multiple
options — that's standard Path A, a single refined design. If genuinely ambiguous, ask in one
line whether they want one design drafted directly or a few different takes to pick from.

### Ship Blueprint / Reference Sheet

**Reference file:** `references/ship-blueprint.md`

**What it does:** Turns an already-confirmed ship spec into a multi-view technical reference
sheet prompt — an orthographic turnaround (front/side/top/rear/3-4, plus bottom when the
underside is distinctive) and a dimensions panel, plus supporting panels (systems callouts,
material/color, decals/markings, scale reference, and conditional interior-cutaway,
propulsion-detail, or weapon-detail panels) — meant to be used as a consistency anchor for
later, separately generated images of the same ship. Dense specs get split into a Primary
Reference Sheet and a Detail Sheet rather than crammed into one illegible image. This is a
reformatting of an existing design, not a new
design step: it doesn't introduce anything not already in the confirmed spec.

#### Trigger Detection

Fire this subskill when the user wants a reference document for a ship rather than (or in
addition to) a single illustrative image. Trigger on: "blueprint", "schematic", "technical
drawing", "orthographic view(s)", "turnaround", "reference sheet", "reference document",
"model sheet", "I want to use this for other images", "keep this consistent across images",
explicit requests for front/side/top/rear views.

**Requires a confirmed spec first.** If the conversation doesn't already have one, run the
normal Session Flow (whichever path fits what the user gives you) to lock in a design before
applying this format. If the user asks for a blueprint mid-design, finish confirming the spec
first — don't generate a reference sheet for an unconfirmed or partial design.

Once a design is confirmed via any path, it's worth proactively offering this subskill in the
same message as the standard Final Output: *"Want a blueprint or reference sheet version of
this ship too, for keeping it consistent across future images?"*

---

## Conflict Checking

As you fill categories, watch for combinations that don't cohere, and flag them rather than
silently picking one side:

- A "None" appendage/wings pick alongside "vehicle-style undercarriage" landing gear (ground
  vehicles imply some aerodynamic or structural surfaces even if minimal).
- Heavy-scale-only options (e.g., "cluster array" engines, "spine-and-rib" segmentation,
  "habitation ring") picked for a Small size class, or vice versa — these aren't hard rules,
  but confirm the user actually wants an unusual scale mismatch rather than assuming they
  meant it.
- Heavy weapon visual weight on any role other than Gunship/bomber or Capital escort/corvette
  — the menu ties "Heavy" explicitly to a "gunship read," so it's an unusual pairing on a
  Racer/interceptor, Dogfighter, Explorer/scout, or Hauler/freighter (a light, agility-focused
  craft covered in dense weapon racks reads as incoherent, not intimidating). Likewise,
  "None"/minimal weapons on a Gunship/bomber role. Cross-check category 5 against the role
  archetype from category 0 before finalizing.
- A crew count of 15+ with no bridge/command structure named in category 3.
- Multiple "dominant" picks stacking on a hull that isn't Heavy scale (e.g., rear-heavy mass
  distribution + dominant engine bulk + heavy weapon visual weight all on a Medium hull) —
  each may be individually justified, but worth a quick confirmation that the ship isn't
  reading as overloaded for its size class.

When something doesn't cohere, ask a short clarifying question rather than resolving it
yourself: *"[X] and [Y] are an unusual pairing — is that intentional, or should one change?"*

---

## Final Output

Once the spec is confirmed, deliver two things in the same response:

### 1. Ship Description

A flowing natural-language paragraph (not a list) that walks through the confirmed spec in
the category order given above: Size/Role → Mass → Hull → Cockpit/Bridge → Propulsion →
Weapons → Appendages → Cargo/Utility → Crew Signaling → Surface Detail → Material/Color. This
is the primary deliverable — it should read like a designer's written brief, specific enough
that an illustrator or 3D artist could work from it directly, in vehicle-designer language
(no fuselage/wingspan phrasing unless wings were actually chosen).

Skip any category that was left at "None" — don't pad the prose with absence statements like
"it has no cargo bay."

Wrap the Ship Description itself in a fenced code block too — it routinely gets copied
elsewhere (into `image-prompt-builder`, into a chat with an illustrator, etc.), and a fence
makes that a clean copy every time.

### 2. Image Prompts

Wrap the ship description into ready-to-use image-generation prompts. **Style is out of
scope for this skill** — use neutral, concept-art framing (three-quarter view or orthographic
turnaround, clean studio or hangar background, technical/concept-art rendering) rather than
picking an illustration style. If the user wants a specific art style applied (anime,
painterly, photoreal, etc.), tell them to take the Ship Description into the
`image-prompt-builder` skill, which handles style selection — don't try to replicate that
skill's style library here.

**Default target platform is ChatGPT only.** Deliver the ChatGPT Robust and Compact prompts
every time. Only add the Niji Journey Robust/Compact prompts if the user asks for Niji
Journey/Midjourney-style output specifically, or has said earlier in the session that they
want both platforms — don't generate prompts for a platform nobody asked for.

⛔ **MANDATORY FORMAT — NO EXCEPTIONS:**
- Every prompt gets its own separate fenced code block (triple backticks) — never combine
  multiple prompts inside one shared fence.
- Each prompt is preceded by its exact section label as a markdown heading, placed *outside*
  the fence, immediately above it.
- Whichever prompts are in scope for this response are delivered together, in this order:
  ChatGPT Robust → ChatGPT Compact → (if in scope) Niji Journey Robust → Niji Journey Compact.
- Never deliver a prompt as plain paragraph text, a bullet point, or inside a shared block
  with other prompts — the fence is what lets the user copy it cleanly with one click, and a
  missing or shared fence defeats that.

**The default output (ChatGPT only) must look exactly like this template** (two separate
fences, not one):

### ChatGPT Prompt — Robust
```
[prompt here]
```

### ChatGPT Prompt — Compact
```
[prompt here]
```

If Niji Journey is also in scope, append two more blocks in the same pattern — own heading,
own fence, each:

### Niji Journey Prompt — Robust
```
[prompt here]
```

### Niji Journey Prompt — Compact
```
[prompt here]
```

**ChatGPT Robust:** Natural prose, no parameter syntax. Open with the neutral concept-art
framing (view angle, background, rendering feel), then the full ship description, then a
"Do not include:" line if any exclusions are implied (e.g., "no wings or aerodynamic control
surfaces" when appendages were set to "None").

**ChatGPT Compact:** The same, condensed to 2-3 sentences — core hull shape, size class,
propulsion, and one or two standout details.

**Niji Journey Robust** *(only when in scope)*: Short natural-language phrases (2-3 lines
max), ending in `--ar` only — no `--niji` or `--style` flags (incompatible with Niji 7).
Structure: hull/size → propulsion/weapons → material/color → `--ar [ratio]`. Ask for an
aspect ratio if none was given or implied; default to `16:9` for a side/three-quarter vehicle
profile if the user has no preference.

**Niji Journey Compact** *(only when in scope)*: One line — hull shape, size class, 3-5
defining keywords — `--ar [ratio]`.

After delivering these, offer the Ship Blueprint subskill (see Subskills below): *"Want a
blueprint or reference sheet version of this ship too, for keeping it consistent across
future images?"*

---

## Quick Reference — Category Order

| # | Category | Skippable? |
|---|---|---|
| 0 | Size Class & Role Archetype | No — always first |
| 1 | Scale & Mass | No |
| 2 | Hull Geometry | No |
| 3 | Cockpit/Canopy/Bridge | No |
| 4 | Propulsion | No |
| 5 | Weapons/Hardpoints | Sub-categories skip if "None" (unarmed) chosen |
| 6 | Appendages | No |
| 7 | Cargo/Utility Features | Yes, for small combat craft |
| 8 | Crew/Interior Signaling | Yes, for small combat craft |
| 9 | Surface Detail Density | No |
| 10 | Material & Color | No |

Full option text for every category lives in `references/design-menu.md` — always read it
fresh rather than recalling options from memory, since exact wording matters for consistent
output.
