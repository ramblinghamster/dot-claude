# Ship Blueprint / Reference Sheet — Subskill

This subskill turns an already-confirmed ship spec into a multi-view technical reference
sheet prompt — the kind of production document used to keep a ship's proportions, hull
details, and color scheme consistent across many separate future image generations. It is an
**output format**, applied after a design is locked in, not a design step itself — it doesn't
introduce new design decisions, it only reformats decisions already made.

---

## When to Invoke

This subskill needs a fully confirmed ship spec (all 10 categories settled) before it can do
anything. That spec can come from:
- Earlier in the same session (standard Path A/B/Fast Mode, or a Ship Ideation pick)
- The user pasting back a spec or Ship Description from a previous session

**If no confirmed spec exists yet in the conversation, run the standard Session Flow first**
(the entry path that fits what the user gives you) to lock in a design, then apply this
format at the Final Output step instead of, or alongside, the standard single-view output.

Trigger on:
- "blueprint", "schematic", "technical drawing", "orthographic view(s)", "turnaround"
- "reference sheet", "reference document", "production reference", "model sheet"
- "I want to use this for other images", "keep this consistent across images", "so I can
  reference it later", "reference for consistency"
- explicit requests for front/side/top/rear views of a ship

---

## Rendering Mode — Ask First

"Reference for future images" can mean two different visual registers, and they produce very
different results. Ask which the user wants, unless they've already named one explicitly:

> "Should this be a **technical blueprint** (schematic line art, dimension lines, blueprint
> blue-and-white or dark technical-drawing aesthetic — reads like an engineering document) or
> a **rendered reference sheet** (concept-art quality, still strictly orthographic and
> labeled, but painted/rendered like a game production asset)? Either works well as a
> consistency reference for later images."

**Technical Blueprint mode**
- Line-art or vector-style rendering, minimal color — blueprint blue-and-white, or a dark
  schematic with white/cyan linework
- Dimension lines, measurement callouts, and a technical legend/title block
- Reads as an engineering document, not an illustration — no rendered materials or lighting

**Rendered Reference Sheet mode**
- Full concept-art rendering quality — the same material, color, and lighting language a
  finished illustration of the ship would use
- Still strictly orthographic and labeled — this is a production asset, not a hero shot or
  dramatic composition
- Closer to what most people mean by "reference document concept art," and the better default
  when the sheet's real purpose is visual consistency across future *illustrated* scenes
  rather than engineering accuracy

If the user has no preference, recommend Rendered Reference Sheet — it carries over more
directly into later stylized image prompts, which is this subskill's actual purpose.

---

## Core Design Goals

Whichever mode is chosen, the sheet should:
- Present the ship clearly from multiple fixed angles, at consistent scale and proportion
- Maintain strict silhouette, hull-panel, and color consistency across every view
- Call out major functional features (propulsion, weapons, cockpit/bridge, cargo/utility
  access) so a future prompt can reference "the ship with the dorsal turret" and mean the
  same ship every time
- Feel like a professional production/engineering asset, not a dramatic illustration
- Use clean, legible layout with labeled panels — **every view gets a text label rendered
  directly on the image** (FRONT · SIDE · TOP · REAR · 3/4), and **every panel group gets a
  bold section header rendered on the image**

---

## Panel Layout

Only include panels that make sense for the confirmed spec — don't invent hardware or
sections that aren't in the ship's design just to fill a slot. Panels 6 and 7 are explicitly
conditional; skip them when the spec doesn't call for them.

### Panel 1 — Ship Info Block
*Location: top-left or top banner*

Pull directly from the confirmed spec:
- Designation/callsign if the user named one; otherwise a generic label like "DESIGNATION:
  UNNAMED" is fine — don't invent a name
- Size class & role archetype (category 0)
- Overall length category and crew count (category 1)
- A one-line design brief — the opening clause of the confirmed Ship Description works well

---

### Panel 2 — Orthographic Turnaround
*Main centerpiece — this is the panel the rest of the sheet exists to support*

Required views: **Front · Side · Top/Plan · Rear · 3/4 perspective**

Requirements:
- Identical hull proportions, panel lines, and color placement across every view — this
  consistency is the entire point of the sheet
- Each view labeled directly on the image: **FRONT · SIDE · TOP · REAR · 3/4**
- Section header: **"ORTHOGRAPHIC TURNAROUND"** or **"SHIP TURNAROUND"**

---

### Panel 3 — Systems Callouts
*Labeled pointer-line annotations over one of the turnaround views (typically side or 3/4)*

Call out only features present in the confirmed spec — pull straight from whichever
categories weren't set to "None": cockpit/bridge position (category 3), propulsion mounts and
nozzle style (category 4), weapon hardpoints (category 5, only if armed), cargo/docking
features (category 7), sensor/utility hardware (category 7). Each callout is a short label
connected to its feature with a thin pointer line — e.g. **"INTEGRAL TWIN THRUSTERS"**,
**"DORSAL TURRET"**, **"VENTRAL CARGO RAMP"**.

Section header: **"SYSTEMS CALLOUTS"**

---

### Panel 4 — Material & Color
*Small swatch block*

Swatches for: base hull material (category 10), primary color, secondary/accent color,
engine glow color if applicable. Label each swatch with its name.

Section header: **"MATERIAL & COLOR"**

---

### Panel 5 — Scale Reference
*Silhouette comparison*

Ship silhouette next to a labeled human figure for scale. For Medium/Heavy craft, optionally
add one more labeled comparison object appropriate to the role (a ground vehicle, a shipping
container, a shuttle) — only if it clarifies scale, not as decoration.

Each figure labeled: **SHIP · HUMAN** (· comparison object, if used)
Section header: **"SCALE REFERENCE"**

---

### Panel 6 — Interior Cutaway *(conditional)*
*Include if crew count (category 1) is 3 or more, OR cargo access (category 7) is anything
other than "None"*

A single broad-strokes side-view cutaway showing major internal zones only — not a detailed
deckplan. Whether the panel is included and which zones it shows are two separate questions —
figure out inclusion first from the trigger above, then populate zones independently based on
what's actually in the spec, not from whichever condition happened to trigger inclusion:
- **Cockpit/bridge zone** — always include; every ship has one.
- **Crew quarters zone** — include if crew count is 3 or more, regardless of what category 8
  (crew/interior signaling) is set to. Category 8 only controls what's visible from *outside*
  the hull (windows, catwalks); it says nothing about whether crew quarters exist internally,
  so don't skip this zone just because category 8 is "None."
- **Cargo hold zone** — include only if cargo access (category 7) is anything other than
  "None." Don't add a cargo zone just because the crew-count trigger fired if the spec has no
  cargo provision.
- **Engineering/propulsion zone** — always include; this is where the aft mass reads as
  interior volume rather than solid hull.

Zone boundaries should match the mass distribution and hull segmentation already established
in categories 1–2.

Section header: **"INTERIOR CUTAWAY"**

Skip the entire panel only when neither trigger condition is met — e.g. single-pilot or
pilot+gunner craft with cargo access left at "None." There's nothing to show in that case.

---

### Panel 7 — Weapon/Hardpoint Detail *(conditional)*
*Include only if Weapons presence (category 5) is "Armed"*

A close-up of the primary weapon mount identified in category 5 (turret, pylon cluster, or
nose-mounted guns) at larger scale than the turnaround views, showing mounting detail.

Section header: **"WEAPON DETAIL"**

Skip this panel entirely if weapons presence is "None" — don't invent an armament panel for
an unarmed ship.

---

## Layout & Rendering Language by Mode

**Technical Blueprint mode keywords:**
`orthographic technical drawing`, `blueprint schematic`, `dimension lines`, `engineering
diagram`, `vector line art`, `monochrome or blue-and-white technical rendering`, `title block`,
`grid background`, `measurement callouts`

**Rendered Reference Sheet mode keywords:**
`concept art production reference sheet`, `game/film production asset`, `orthographic
turnaround`, `clean studio lighting`, `matte technical illustration`, `labeled panels`,
`consistent proportions across views`, `neutral background`

**Shared negatives (both modes):**
`no dramatic lighting`, `no motion blur`, `no dynamic action pose in the turnaround panel`,
`no inconsistent proportions between views`, `no unlabeled panels`

---

## Output

Deliver this as the same four-variant format used elsewhere in this skill (ChatGPT
Robust/Compact, Niji Journey Robust/Compact), describing the full panel layout instead of a
single view. Wrap each in its own labeled, fenced block per the main skill's Final Output
formatting rules.

**Aspect ratio:** default to `16:9` for a standard sheet; suggest `21:9` if the confirmed spec
includes both an Interior Cutaway and a Weapon Detail panel (5+ panels tends to need the extra
width to stay legible).

**ChatGPT Robust:** Open with the rendering-mode declaration (blueprint or rendered reference
sheet), then walk through each included panel in order, describing what it contains and
requiring text labels/section headers rendered on the image for every panel. Close with a
"Do not include:" line drawn from the shared negatives above plus anything implied by the
ship's own "None" picks (e.g., no visible weapon hardpoints if unarmed).

**ChatGPT Compact:** Condensed to the rendering mode, the ship's core identity (from Panel 1),
and a list of which panels to include — trust the model to lay them out reasonably at this
length.

**Niji Journey Robust/Compact:** Short phrase-based structure as elsewhere in this skill —
lead with "orthographic production reference sheet of [ship]," list the included panels as
short keyword groups, close with `--ar [ratio]`. Keep in mind Niji Journey handles complex
multi-panel infographic layouts less reliably than ChatGPT/DALL-E — mention this to the user
if they lead with Niji Journey as their target platform, and suggest ChatGPT as the more
reliable choice for this specific format.
