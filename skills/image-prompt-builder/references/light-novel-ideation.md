# Light Novel Cover Ideation — Sub-Skill

This sub-skill generates and refines **light novel cover concepts** — from a randomized
premise through a finished, publication-styled cover prompt with Japanese and English text
elements. It is a full alternate pipeline (like Character Creator), not the 8-Block flow.

**Primary language: Japanese.** Titles, subtitles, and obi band copy are drafted in Japanese
first (matching real JP light novel conventions), with romaji reading and English translation
alongside every line. The user can request an English-primary cover, a bilingual cover, or a
flip between languages at any point — see **Language Handling** below.

---

## Trigger

Activate when the user's intent is a **light novel cover** — not a generic anime scene.

Trigger phrases:
- "light novel cover", "LN cover", "light novel idea/concept"
- "generate a light novel", "randomize a light novel", "surprise me with a light novel"
- "isekai cover", "yuri light novel", "villainess cover" + similar genre + "cover"/"novel"
- "give me a title" / "light novel title" in combination with a cover/prompt request
- References to obi bands, JP book covers, or "light novel style" text layout

Do NOT trigger for a generic character portrait or scene that happens to be anime-styled —
only trigger when the deliverable is a **book cover** with title/subtitle/obi text elements.
If unclear, ask: *"Do you want a full light novel cover — title, subtitle, obi band and all —
or just an illustration in a light-novel-adjacent style?"*

---

## Language Handling

- Draft all text elements (title, subtitle, obi band) **in Japanese first**, using real JP
  light novel title conventions (see Step 3).
- Alongside every Japanese line, always show:
  1. The Japanese text
  2. Romaji reading
  3. A natural English translation (not a literal gloss — it should read like an actual
     localized LN title, matching tone)
- If the user asks for **English instead**: don't just paste the gloss — rewrite it as a
  title that reads naturally as an English-market LN title (these often keep some JP-style
  bewildered/deadpan phrasing rather than fully anglicizing). Keep the Japanese version
  alongside for reference unless the user says to drop it.
- If the user asks to **flip languages** on an already-locked cover (e.g., "now give me the
  English version" or "switch this to Japanese"): re-derive title, subtitle, and obi band
  text together, preserving tone and meaning — do not translate line-by-line in isolation,
  since title/subtitle framing sometimes needs to shift between languages to stay natural.
- If the user wants **both on one cover** (bilingual): keep the Japanese as the dominant
  text (larger, primary), with English as a smaller secondary line — matching how localized
  JP covers sometimes show a small English subtitle beneath the main JP title.
- All locked text (title, subtitle, obi band, publisher emblem) gets written as literal
  quoted strings directly into the final ChatGPT prompt — see Step 9. Keep the JP/romaji/EN
  forms in sync so whichever is quoted in the prompt matches what was locked in Steps 3 & 8.

---

## The 9-Step Pipeline

| Step | What it locks |
|---|---|
| 1 | Concept Triangle — genre, core situation, world hook |
| 2 | Conflict structure — leads, antagonist, allies |
| 3 | Title + subtitle (JP primary, romaji, EN) |
| 4 | Character visual-opposite design |
| 5 | Cover pose |
| 6 | Setting |
| 7 | Art style |
| 8 | Obi band copy (JP + EN) |
| 9 | Final image prompt assembly |

Work through steps in order. The user can jump in at any step if they already have material
(e.g., "here's my title and characters, help me pick a pose") — skip completed steps but
still display them in the running summary so the full concept stays visible.

---

## Step 1 — Concept Triangle (+ Randomizer)

Lock three things first — everything else derives from them:
- **Genre** (yuri romance, dark fantasy, isekai, villainess redemption, etc.)
- **Core situation** (confession, battle, reunion, etc.)
- **World hook** — the most important differentiator. A generic "fantasy romance" becomes
  specific the moment you add "rival religious orders serving different gods."

### Randomizer

When the user wants a random/fresh idea ("surprise me", "randomize", "give me a light novel
idea", no constraints given), generate **3 Concept Triangle Cards**, each genuinely distinct.
Vary across these axes so the 3 don't collapse into one flavor:

- **Emotional register:** tender vs. tense vs. tragic vs. triumphant
- **Relationship dynamic:** equals/rivals, protector/protected, forbidden secret, long-lost reunion
- **Power structure:** institutional (factions/orders), cosmic/divine, personal/individual stakes

**Card format:**

### [CONCEPT #] — [one-line hook]

| Field | Value |
|---|---|
| **Genre** | ... |
| **Core Situation** | ... |
| **World Hook** | ... |
| **Why it works** | one sentence on what makes the hook specific, not generic |

Randomizer table (pull from freely, remix, or invent adjacent options — don't just recite
this list verbatim every time):

**Genre pool:** yuri romance · isekai fantasy adventure · dark fantasy tragedy · reincarnation
slice-of-life · school romantic comedy · villainess redemption · demon-lord/hero subversion ·
rival mage-academy drama · modern urban fantasy · cozy iyashikei fantasy · political intrigue
fantasy · idol/entertainment drama

**Core situation pool:** a forbidden confession · a reunion after years apart · a duel that
ends in an unexpected truce · a contract/pact sealed under duress · a public engagement
announcement gone wrong · a rescue mid-losing-battle · a shared curse discovered too late ·
a defection from one's own faction · a first meeting mistaken for an enemy encounter · a
festival where secrets surface

**World hook pool:** rival religious orders serving different gods · magic powered by
memories (spend them, lose them) · two moons granting opposing powers · a caste system based
on which god chose you at birth · a war fought entirely through shared dreams · souls
literally split into two bodies · royalty forced to marry their appointed rival · magic that
manifests as visible color auras around the caster · a tower that resets time for anyone
who fails to climb it · a city built on the back of a sleeping god

After presenting 3 cards:

> *Pick a concept (1, 2, or 3), mix elements from different cards, or say "more ideas" for
> 3 new concepts. Once you choose, I'll build the conflict structure.*

If the user supplies their own genre/situation/hook (even partially), fill in only what's
missing using the pools above for inspiration, and skip straight to displaying the locked
triangle for confirmation — don't force them through the randomizer.

---

## Step 2 — Conflict Structure

Define:
- **Who are the two leads** and what separates them institutionally/ideologically
- **Who is the antagonist** and what they represent (opposition to the leads' union) —
  for romance specifically, the antagonist should be the external force keeping the leads
  apart, not a generic villain
- **Who are the allies** and their emotional role (support, witness, contrast)

Display the locked structure in one short block before moving on.

---

## Step 3 — Title Construction (JP primary, romaji, EN)

The title carries the premise — it should function almost like a one-sentence synopsis.

**Pattern:** [protagonist situation] + [twist or consequence] + [deadpan resolution]

Tonal rules:
- Narrator sounds slightly bewildered or matter-of-fact, not editorializing
- Ends with the equivalent of "so I did X" / "it turned out like this" / "apparently"
  rather than a punchline
- Avoid Western meme-endings ("Worth It", "No Regrets")
- Long titles are fine and expected

**Title + subtitle split:**
- Short, punchy main title (3–6 words in Japanese)
- Long descriptive subtitle after 〜...〜 that fills in the premise
- These are two separate text elements with different sizes/weights on the final cover

**Generate 10+ candidates.** For each, give all three forms together:

| # | Japanese | Romaji | English |
|---|---|---|---|
| 1 | [title]〜[subtitle]〜 | [reading] | [natural EN translation, not literal] |

Filter candidates by:
1. Does it sound like a real JP light novel when read aloud?
2. Does it convey the world hook and emotional core from Step 1?
3. Does the deadpan/matter-of-fact tone hold across all three language forms?

Present the filtered shortlist (not all 10+), let the user pick or request a remix, then
lock the final title + subtitle in all three forms.

---

## Step 4 — Character Visual Opposites

Design each lead visually coded to her faction/order using three coordinated elements:

| Element | Lead A | Lead B |
|---|---|---|
| Hair | Color A, possibly fading/altered | Color B, vivid/glowing |
| Robes/Vestments | Faction A palette, condition reflects story state | Faction B palette, condition reflects story state |
| Holy Item | Pendant/staff/object, condition reflects story state | Pendant/staff/object, condition reflects story state |

**Story state:** if a character has been abandoned by her god, her hair fades, trim
tarnishes, holy item cracks/dims. If still favored, everything is vivid and glowing.

**Shared visual moment:** where the two leads touch/overlap, one's light bleeds subtly onto
the other — shows the "new devotion" theme without extra symbolism.

Avoid: tattoos/markings as the primary divine indicator (too generic); identical palettes
between leads (kills contrast); matching poses or expressions (they should feel like
opposites drawn together).

Adapt this table's specific "faction/holy item" framing to whatever Step 1/2 hook and cast
actually call for — it's a template for coded visual opposition, not literally required to
be religious factions.

---

## Step 5 — Cover Pose

Choose based on what the scene demands:

- **Embrace + looking at viewer** — best "pick me off the shelf" appeal; intimacy + invitation
- **Mirrored defiance** — better for rivalry/tension covers, less intimate
- **Falling/reaching** — dynamic but anatomically risky for AI generation
- **Crowned in each other's light** — thematically rich but subtle, may not read at thumbnail size

For yuri/romance specifically: real published covers (Bloom Into You, Citrus) prioritize
**faces and emotional expressions** over dramatic action poses. Keep it intimate and readable.
For rivalry/action-forward concepts, mirrored defiance or dynamic motion reads better.

---

## Step 6 — Setting

Define one strong location:
- **Architecture** (cathedral, forest shrine, palace, etc.)
- **Lighting moment** (golden hour, candlelight, moonlight, etc.)
- **Atmospheric detail** (stained glass, floating sigils, mist, etc.)

For rival-faction stories: background architecture can subtly merge both factions' visual
styles (one side gold/sun-domed, other silver/moon-spired) — communicates the union theme
visually without extra explanation.

---

## Step 7 — Art Style

Evaluate against this checklist before committing — check whether the style's fixed palette
or lighting constraints conflict with the Step 4 character color story:

| Style | Good for | Avoid when |
|---|---|---|
| Pixiv Clean | Character focus, fabric detail, clean faces | Complex lighting, atmospheric backgrounds |
| Gossamer | Healing/quiet tone, shrine/priestess themes, light-novel-illustration look natively | High drama, strong color contrast needed |
| Ember | Warm candlelit interiors | Tends toward realism/painterly texture |
| Velvet | Premium dark fantasy, glossy rendering | Fixed crimson-violet palette conflicts with your color story |
| Cinematic Anime | Dramatic key visuals, no palette lock | Can feel more action/isekai than romance |

These five are the strongest starting points, but any style from the full library
(`references/styles.md`) is fair game — use the Style Decision Tree in `SKILL.md` if the
user wants help narrowing down further. Load the chosen style's ChatGPT and Niji Journey
translations for Step 9.

---

## Step 8 — Obi Band (JP + EN)

Write this **last**, after everything else is locked, so it reflects the actual emotional
stakes of the story. Structure:

- **Teaser line** — one dramatic sentence about the central dilemma
  ("The goddess has chosen. But which one will it be—")
- **Emotional hook** — the protagonist's emotional declaration, bolded
  ("Even if I'm declared a SINNER, I want to LIVE with you.")
- **Genre/promotional tag** — short descriptor + fake sales claim
  ("A forbidden fate. A yuri romance in a divine world!")

Tone options: cool/serious, dramatic/exaggerated, deadpan/absurd — match to the title's tone
from Step 3. Deliver all three lines in Japanese + romaji + English, same as the title.

---

## Step 9 — Final Image Prompt Assembly

**Text elements are written as literal quoted strings directly in the prompt, with explicit
placement, sizing, and treatment for each one** — not described abstractly as "title text in
the described position." ChatGPT/DALL-E 3 can approximate short quoted title/subtitle text
and will attempt full obi copy; giving it the literal string plus exact layout instructions
produces the intended cover far more reliably than a vague reference to "typography."

Assemble ChatGPT prompts as one flowing paragraph in this order:

1. **Style opening** — art style block from Step 7 (linework, shading, palette rules)
2. **Pose + characters** — from Steps 4 & 5, coordinated hair/vestment/holy-item details and
   the shared light-bleed moment, woven together
3. **Setting** — from Step 6, kept simple/uncluttered so text stays readable
4. **Supporting cast** — antagonist + allies, small and simply rendered, always
   smaller-scaled than the leads
5. **Title** — position (e.g. "at the top"), size/weight treatment (e.g. "large elegant
   calligraphic title text"), any color/glow effect, then the literal string in quotes:
   `text reading "[title]"`
6. **Subtitle** — position relative to the title (e.g. "below it, smaller subtitle text"),
   then the literal string in quotes: `reading "〜[subtitle]〜"`
7. **Obi band** — position (typically "at the bottom"), band background color, text color
   and weight, the literal quoted obi copy, plus any accent graphic (starburst, seal, etc.):
   `a horizontal obi band with [color] background and [color/weight] text reading
   "[obi copy]"` — condense Step 8's three lines into one obi string if needed for length
8. **Publisher emblem** — small graphic shape (circular, crest, etc.) with the literal
   fictional imprint name in quotes: `a small circular publisher emblem reading "[imprint]"`
9. **Finish/quality + negative constraints** — closing line naming the render mode (e.g.
   "clean, polished 2D Pixiv-style anime illustration") and what to exclude (painterly
   texture, photorealism, plus the loaded style's Style Negatives from `styles.md`)

**Robust version:** full paragraph covering all 9 elements above with complete detail on
each — matches the density of a finished, ready-to-generate prompt.

**Compact version:** condensed to 3–5 sentences. Keep all literal quoted text (title,
subtitle, obi copy, emblem) intact — text elements are never trimmed for length, only the
surrounding scene/style description is shortened.

Which language's strings to quote (Japanese, English, or both per **Language Handling**)
depends on what's locked for the cover — swap in the corresponding forms from Steps 3 & 8
without changing the layout instructions.

**Niji Journey caveat:** Niji/Midjourney renders quoted text far less reliably than DALL-E 3.
Generate the Niji Robust/Compact prompts per `SKILL.md`'s standard format, but keep any
literal text short (title only, or omit text entirely and note it as a text-free illustration
variant) — flag to the user that the ChatGPT version is the reliable source for accurate
cover text, and Niji is best treated as an alternate illustration-only rendering.

Deliver all four prompts using this skill's standard final output format (ChatGPT Robust,
ChatGPT Compact, Niji Journey Robust, Niji Journey Compact — each in its own labeled fenced
code block, per `SKILL.md`'s Final Output template).

---

## Key Reminders

- Write literal quoted text directly into the prompt for title, subtitle, obi band, and
  publisher emblem — don't describe text elements abstractly. This is what makes ChatGPT
  actually attempt the correct copy in the correct position (see Step 9 template).
- Text rendering still isn't perfect, especially for longer obi paragraphs or if the user
  wants full-accuracy JP typography — mention post-production touch-up as a fallback option,
  not the default plan.
- Real publisher names are prohibited — always invent a fictional imprint.
- Pixiv Clean and similar character-portrait styles conflict with complex background scenes
  — either simplify the background or switch styles.
- Yuri/romance covers prioritize faces and emotional expressions over action — keep the
  central pose intimate and readable at thumbnail size.
- The title + subtitle split is a text-design decision as much as a writing one — short bold
  title + long smaller subtitle gives visual hierarchy without one unreadable block.
- Every title, subtitle, and obi line should exist in Japanese, romaji, and English by the
  time Step 9 delivers — don't let one language fall out of sync with the others.
- Niji Journey text rendering is unreliable — treat the Niji prompts as a text-light or
  text-free illustration variant, not the primary source for accurate cover copy.
