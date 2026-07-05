# Ship Ideation — Subskill

This subskill generates **Ship Concept Cards** — distinct, randomized combinations of picks
from the design menu, presented as options for the user to browse. It is an ideation step,
not the final spec-and-generate step. After the user picks a concept (or mixes elements from
a few), the flow rejoins the main skill at Path A step 4 (present the compact draft spec) and
continues normally from there.

---

## When to Invoke

The core test: **does the user want one ship refined start to finish, or a few to choose
between?**
- If one, already-described ship → standard Path A.
- If several options, or the user is undecided → Ship Ideation.

Trigger on messages that signal wanting variety rather than committing to a single design:
- Words like "ideas", "concepts", "options", "variations", "brainstorm", "inspire",
  "surprise me", "random", "pick one for me", "show me a few", "give me some choices"
- "give me a few/some [role/keyword] ideas or concepts" — e.g. "give me a few cargo freighter
  ideas", "got any missile frigate concepts?", "pitch me some heavy corvette options"
- "what are some ways to do a ___" or "I want a ___ but don't know what it should look like"
- A bare role, keyword, or size class anchor offered with no other descriptive detail, framed
  as wanting to browse rather than commission one exact design

Do NOT trigger on a plain "design a [role] for me" with no signal of wanting multiple
options — that's standard Path A, one refined design. If it's ambiguous whether the user
wants one design or several, ask in one line: *"Want me to draft one design directly, or
sketch out a few different takes for you to pick from?"*

---

## Input

The user may optionally anchor the ideation with any of the following. Anything not given is
left free to vary across the concepts.

- **Role/keyword anchor** — a term like "cargo freighter", "missile frigate", "scout ship",
  "dropship", "racer". Map it to the nearest Size Class & Role Archetype in category 0 and
  hold that pick fixed across all concepts; vary everything else.
- **Size class anchor only** — e.g. "give me some heavy ship ideas" with no role stated. Hold
  the size class fixed, vary the role archetype and everything else.
- **Aesthetic/mood keywords** — e.g. "beat up", "sleek", "military", "scrappy", "elegant".
  Bias categories 9 (Surface Detail) and 10 (Material & Color) toward that mood, but still
  vary the specific picks within it across the three concepts so they aren't identical reads
  of the same mood.
- **Nothing at all** — fully free. Vary size class and role archetype themselves, along with
  everything else, to maximize the spread across the three concepts.

Whatever is given as an anchor is a hard constraint for every concept card. Everything else is
where the variety lives.

---

## Output Format

Generate **3 Ship Concept Cards**, each a distinct, self-contained design idea.

Each card must include:

### [CONCEPT #] — [Evocative one-line ship name or hook]

| Field | Value |
|---|---|
| **Size Class & Role** | Category 0 pick — fixed across all cards if anchored, varied otherwise |
| **Silhouette** | 1–2 sentences: hull shape, mass distribution, and one propulsion or weapons detail — enough that the reader can picture the ship's overall shape at a glance |
| **Standout Trait** | The single most distinctive design choice that sets this concept apart from a generic version of the same role — a specific, memorable pick from any category (e.g., "engines are fully integral, no visible seam at all — unusual for a hauler this size", "an asymmetric scavenged sensor pod bolted to one flank", "hull reads as stacked layered decks like a real ship's plating rows") |
| **Character** | The use-case or history read in one line — what kind of owner, crew, or life this ship has had (e.g., "pristine corporate courier fresh off the line" vs. "independent runner patched together from three different wrecks") |

After the 3 cards, add:

> *Pick a concept (1, 2, or 3), mix elements from different cards, or say "more ideas" for 3
> new concepts. Once you choose, I'll fill out the full spec and confirm it with you before
> generating the final description and prompts.*

---

## Randomization Guidelines

The 3 concepts must feel genuinely distinct — this is the entire point of ideation. Don't let
all three quietly converge on the "most obvious" version of the anchor.

There's no real dice roll available, so simulate one deliberately: for each major category,
actively choose a *different* value across the three cards rather than defaulting to
whichever option comes to mind first. Specifically vary across:

- **Hull geometry** (category 2) — don't give all three the same primary shape. A wedge, a
  cylinder, and a faceted polyhedron read as three different ships even before anything else
  changes.
- **Propulsion mounting relationship** (category 4) — spread bolted-on, podded, and integral
  across the three rather than picking the same one every time. This is the single easiest
  way to make three concepts feel mechanically distinct.
- **Mass distribution** (category 1) — vary nose-heavy vs. rear-heavy vs. centered/even.
- **Wear and material** (categories 9–10) — vary pristine vs. lightly weathered vs. heavily
  worn, and vary the base material read, unless an aesthetic anchor constrains this.
- **Size class and role** (category 0), when not anchored — spread across Small/Medium/Heavy
  and across genuinely different role archetypes rather than three flavors of the same role.

Everything else (cockpit/bridge, weapons, appendages, cargo/utility, crew signaling) should
still follow the size-class-and-role tendencies from category 0 as a baseline, but feel free
to deviate on one or two categories per card to give each concept a genuine identity — that
deviation is often exactly what becomes the "Standout Trait."

Keep the vehicle-designer mindset from the main skill in force here too: no wings or
aerodynamic surfaces without a functional reason, mass distribution over streamlining, and
vehicle-class reference points (APCs, tugboats, excavators) rather than aircraft ones. Random
does not mean sloppy — every concept should still read as a coherent, physically-sensible
vehicle, just a different one each time.

---

## After Concept Selection

Once the user picks a concept (or a mix of elements from a few):

1. Confirm the choice back in one sentence.
2. Auto-populate the full spec across all 10 categories: start from whatever the chosen
   card's Silhouette, Standout Trait, and Character fields imply, and fill anything not
   already implied using the "typical tendencies by size class" defaults from category 0 —
   same fallback the main skill uses in Path A. When a concept card's implied value actively
   conflicts with the size-class default (not just leaves it unstated — e.g. the card implies
   a forward bridge block but the size class's default tendency is a raised bridge tower), the
   card's value wins. Note the override in the draft spec (a short parenthetical is enough)
   so the user can see it was a deliberate choice from their selected concept, not a mistake.
3. Present the compact category-by-category draft (Path A, step 4) and proceed with the
   standard confirmation gate and Final Output from there (Path A, steps 5–6). Nothing about
   the output format changes because the design started as an ideation pick rather than a
   user description.
