# Commercial Ad Ideation — Sub-Skill

This sub-skill generates **character-inspired product advertising concepts** — an original
product invented from a character's visual/personality read, through a finished, brand-style
advertising poster prompt. It is a full alternate pipeline (like Character Creator and Light
Novel Cover Ideation), not the 8-Block flow.

It is **multi-vertical**: perfume is the first fully-specified vertical, but the pipeline is
built so new product categories (jewelry, skincare, watches, spirits, fashion accessories,
tech gadgets, etc.) can be added as their own vertical entry without changing the pipeline
shape. See **Product Verticals Library** below.

---

## Trigger

Activate when the user wants a **fictional product + advertising poster inspired by a
character** — not a generic character portrait or a real-brand ad request.

Trigger phrases:
- "perfume ad", "fragrance ad", "cologne ad", "create a perfume based on this character"
- "[product] inspired by this character/image", "design a [product] ad for them"
- "advertising poster", "ad campaign", "brand poster", "commercial poster" + a character/image
- References to any vertical in the Product Verticals Library (perfume, jewelry, skincare,
  watch, spirits, fashion accessory, tech gadget, etc.) combined with "ad", "poster",
  "campaign", "product", or "brand"

Do NOT trigger for a generic character portrait, a real product/brand request, or a scene
that merely includes a product as a prop. Only trigger when the deliverable is an **invented
product + its advertising poster** built from a character read. If unclear, ask: *"Do you
want a full product ad concept — invented product, packaging, and poster — or just an
illustration of the character holding/wearing something?"*

If the user names a vertical not yet in the library (e.g., "design a watch ad for them"),
don't refuse — run the pipeline using the closest existing vertical as a structural template,
flag which fields are improvised, and offer to lock it in as a new library entry afterward
(see **Adding a New Vertical**).

---

## The 7-Step Pipeline

| Step | What it locks |
|---|---|
| 1 | Vertical selection (perfume, jewelry, skincare, etc.) |
| 2 | Source character read — visual + personality signals |
| 3 | Product concept — name, family/type, impression, catch copy, concept |
| 4 | Compose — vertical-specific spec (fragrance notes, materials, tasting notes, etc.) |
| 5 | Product object design — bottle/case/packaging |
| 6 | Lifestyle image scenes (2–3) |
| 7 | Poster assembly — final image prompt |

Work through steps in order. If the user already has material (e.g., "here's the character
and I already know I want a woody fragrance"), skip locked steps but still display them in
the running summary so the full concept stays visible.

---

## Step 1 — Vertical Selection

Identify which product category from the **Product Verticals Library** applies. If the user
names one, use it. If they only say "make an ad" with no category, ask which vertical, or
suggest one based on what the character read (Step 2) implies (e.g., a rugged/utilitarian
character suggests a watch or leather-goods ad over a perfume).

---

## Step 2 — Source Character Read

From the attached image or description, read (do not ask the user to restate what's already
visible in the image):

- Hair color, eyes, expression, hairstyle
- Clothing, pose
- Color scheme, light
- Seasonal feeling
- The atmosphere/personality the image projects

Everything downstream (product concept, spec, object design, scenes) derives from this read —
treat it as the seed, not decoration. Do not ask the user to describe their own personality or
preferences; infer everything from the visual read, the same way a stranger would form an
impression on first meeting this person.

---

## Step 3 — Product Concept

Derive, from the Step 2 read:

- **Original product name** — invented, never a real brand or existing product name
- **Category/family** — the vertical's type classification (e.g., fragrance family for
  perfume; metal/stone family for jewelry)
- **Impression** — the one-line sensory/emotional impression the product should evoke
- **Catch copy** — a short tagline, in the voice of a real high-end ad, never generic
- **Concept** — 2–4 sentences tying the product to the character's read: what someone would
  notice about this person on first meeting, and what they'd notice as they got closer/closer
  to them over time

Do not let the user pre-supply these — the point of this sub-skill is that everything is
inferred from the image, mirroring how the source prompt for this sub-skill worked. If the
user does supply constraints (e.g., "make the name feminine"), fold them in without breaking
the "read, don't ask" principle for everything else.

---

## Step 4 — Compose (Vertical-Specific Spec)

Build the product's internal "composition" using the vertical's spec structure from the
**Product Verticals Library** (e.g., perfume's TOP/MIDDLE/LAST accords). Use real material/
ingredient/component names appropriate to the vertical — this is what makes the concept read
as a plausible real product rather than a vague description.

The composition should **evolve or cohere as a single object**, not feel like a disconnected
list — e.g., a perfume's TOP/MIDDLE/LAST should transition naturally; a jewelry piece's
materials should read as one coherent design decision, not three unrelated choices.

---

## Step 5 — Product Object Design

Design the physical product object matching the character's impression from Step 2–3.
Cover, at minimum: primary material/shape, finish/texture, color, any secondary components
(cap, clasp, strap, label, etc.), and outer packaging — refined like a real high-end brand's
object design. See the vertical's **Object elements** in the library for the specific
checklist.

⛔ Never imitate a real brand's actual product design, logo, or name.

---

## Step 6 — Lifestyle Image Scenes

Depict **2–3 everyday scenes** in which the character would be spending time while using/
wearing/carrying the product — not the moment of application, purchase, or first use itself.
Stage each scene's location, time of day, clothing, gesture, light, and background in harmony
with the product concept, so each scene reads as a natural slice of the character's daily
life or story rather than a product demo.

---

## Step 7 — Poster Assembly (Final Image Prompt)

Create a **vertical poster** in the style of a high-end brand advertisement, laying out:
product name, catch copy, the product object, the character, the Step 4 spec (shown as
text, e.g. accord/note listing), and the Step 6 image scenes — composed together into one
cohesive layout, not a grid of disconnected panels.

**Text elements** (product name, catch copy, spec labels) are written as literal quoted
strings directly in the prompt, with explicit placement, sizing, and treatment for each —
not described abstractly as "product name in the described position." Give the literal
string plus exact layout instructions (position, size/weight, color/effect), the same
approach used for title/subtitle text in Light Novel Cover Ideation.

Assemble ChatGPT prompts as one flowing paragraph in this order:

1. **Style opening** — art style block (semi-realistic/editorial commercial rendering, never
   "photorealistic" — see SKILL.md style rules)
2. **Character** — pose, expression, clothing, and color story from Step 2, matched to the
   product's world view
3. **Product object** — from Step 5, positioned prominently (e.g., foreground or beside the
   character)
4. **Lifestyle scenes** — from Step 6, composed as smaller supporting panels/vignettes around
   or behind the main figure
5. **Product name** — position (e.g., "near the top"), size/weight/treatment, literal quoted
   string: `text reading "[product name]"`
6. **Catch copy** — position relative to the name, literal quoted string:
   `smaller text reading "[catch copy]"`
7. **Spec listing** — the Step 4 composition rendered as clean typographic text (e.g.,
   "TOP: [...] / MIDDLE: [...] / LAST: [...]"), positioned so it doesn't compete with the
   name/copy for primary visual weight
8. **Finish/quality + negative constraints** — closing line naming the render mode and what
   to exclude (photorealism, character-merchandise/collectible-card look, any real-brand
   styling)

**Robust version:** full paragraph covering all 8 elements with complete detail on each.

**Compact version:** condensed to 3–5 sentences. Keep all literal quoted text (product name,
catch copy) intact — text elements are never trimmed for length, only the surrounding
scene/style description is shortened.

**Niji Journey caveat:** Niji/Midjourney renders quoted text far less reliably than DALL-E 3.
Generate the Niji Robust/Compact prompts per SKILL.md's standard format, but keep literal text
short (product name only, or omit and note it as a text-free variant) — flag to the user that
the ChatGPT version is the reliable source for accurate poster text.

Deliver all four prompts using this skill's standard final output format (ChatGPT Robust,
ChatGPT Compact, Niji Journey Robust, Niji Journey Compact — each in its own labeled fenced
code block, per SKILL.md's Final Output template).

---

## Product Verticals Library

Each vertical defines: what Step 3's category/family field means, Step 4's compose
structure, and Step 5's object checklist.

### Perfume

| Field | Spec |
|---|---|
| **Category/family** | Fragrance family (floral, woody, oriental, citrus, gourmand, aquatic, etc.) |
| **Compose structure** | TOP / MIDDLE / LAST accords, ~3–5 real fragrance materials each, evolving naturally as one perfume |
| **Object elements** | Bottle shape, glass texture, liquid color, cap, label, outer box |
| **Special notes** | Never depict the moment of applying the perfume — see Step 6 |

*(Additional verticals — jewelry, skincare, watches, spirits, fashion accessories, tech
gadgets, etc. — get added here as their own table, following the pattern below, once a
worked example exists for each.)*

---

## Adding a New Vertical

When the user brings a new product category (with a worked example, the same way perfume
was introduced):

1. Add a new subsection under **Product Verticals Library** with the same three fields:
   Category/family, Compose structure, Object elements, plus any Special notes.
2. Keep the compose structure to a similarly-sized real-world spec (perfume uses 3 stages ×
   3–5 materials; a different vertical might use a different but comparably concrete
   structure — e.g., jewelry might use material + gemstone + setting rather than staged
   notes).
3. Add trigger keywords for the new vertical to the **Trigger** section's phrase list.
4. No changes are needed to Steps 2, 3, 6, or 7 — they're vertical-agnostic by design.

---

## Key Reminders

- ⛔ Never imitate a real brand — product name, bottle/object design, and catch copy must all
  be original inventions, even when clearly inspired by real high-end advertising conventions.
- ⛔ Never depict the moment of applying/using the product for the first time — only
  established, everyday moments of already living with it (Step 6).
- Maintain the source character's likeness throughout — face, hair, and identity should stay
  recognizable across the character portrait and every lifestyle scene.
- Background, costume, and lighting in every scene should match the product's world view, not
  just the character's original image context.
- Give the product, its object design, and its lifestyle scenes one consistent story — a
  reader should be able to tell they belong to the same campaign.
- Finish the poster like a real product advertisement, not like character merchandise or a
  collectible card — this affects framing, typography treatment, and overall polish level.
- Write literal quoted text directly into the prompt for product name and catch copy — don't
  describe text elements abstractly (see Step 7).
- Niji Journey text rendering is unreliable — treat the Niji prompts as a text-light or
  text-free variant, not the primary source for accurate poster copy.
