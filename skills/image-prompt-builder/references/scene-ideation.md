# Scene Ideation — Subskill

This subskill generates anime-themed **scene concept cards** — distinct ideas with genre,
tone, visual situation, and style recommendations. It is an ideation step, not a prompt
generation step. After the user selects a concept, proceed to the main 8-Block flow to
build the full prompts.

---

## When to Invoke

The core test: **does the user know what they want to generate?**
- If yes → 8-Block flow
- If no → Scene Ideation

Trigger when the message signals wanting ideas rather than describing a scene. Key signals:
- Contains "ideas", "suggestions", "concepts", "inspire", "inspiration", "recommend"
- Contains "what should I make", "don't know what to generate", "help me decide",
  "give me something", "surprise me", "random", "pick something for me"
- "something [adjective]" with no scene content ("something dark", "something cozy")
- A genre, mood, character, or theme with no situation attached ("dark fantasy ideas",
  "something with a knight", "fantasy theme", "give me a scene with a mage")
- Message is too short or vague to be a scene description

Also trigger when the user provides only constraints (genre, mood, character type, setting)
but no actual scene — they want help deciding what to do with those constraints.

Do NOT trigger when the user describes a subject doing something somewhere — even loosely.
Any message with a character + action + setting is a scene description; use the 8-Block flow.

---

## Input

The user may optionally provide any constraints to work within:
- **Genre or mood** (e.g., "dark fantasy", "slice of life", "action")
- **Character description** — fixed traits or a specific OC to place in scenes
- **Setting** — a world or environment they want to explore
- **Style preference** — a style or aesthetic direction they want to stay within

If nothing is provided, generate freely varied concepts.

---

## Output Format

Generate **3 Scene Concept Cards**, each a distinct, self-contained image idea.

Each card must include:

### [CONCEPT #] — [Evocative one-line scene hook]

| Field | Value |
|---|---|
| **Genre / Vibe** | Primary genre + optional emotional flavor |
| **Tone** | Emotional register (e.g., melancholy-cool, absurd, quiet, explosive) |
| **Scene** | What is happening — who is in the frame, what they're doing, where they are |
| **Visual Hook** | One specific detail that makes this image memorable and distinct — an object, shadow, texture, or spatial oddity (e.g., sword used as a walking stick, oversized shadow with the wrong shape, a single lantern reflected in pooled water) |
| **Visual Theme** | Art direction feel (e.g., rain-soaked neon, sun-drenched ruin, flat ink on white) |
| **Recommended Styles** | 2–3 styles from the library that best serve this concept, with a one-line reason each |

After the 3 cards, add:

> *Pick a concept (1, 2, or 3), mix elements from different cards, or say "more ideas" for
> 3 new concepts. Once you choose, I'll build the full prompts.*

---

## Style Recommendation Rules

Match recommended styles to the concept's visual theme and emotional register.
Always recommend at least one **rendering style** (the look) and optionally one **mood or
composition anchor**. Explain in one line why each style fits.

| Concept direction | Strong style candidates |
|---|---|
| Dark/gritty fantasy, brutal detail | Miura, Soulslike, Dark Fantasy, Ufotable |
| Dramatic anime key visual | Cinematic Anime, Ufotable, Gacha Splash |
| Melancholy, distance, glowing skies | Makoto Shinkai, Cinematic Anime |
| Cyberpunk, neon, urban night | Neon Noir, Cinematic Anime, Webtoon |
| Premium dark fantasy portrait | Velvet, Cinematic Anime, Ufotable |
| Soft, flat, healing/iyashikei | Gossamer, Aquarelle, Flat Cel |
| Shounen action, power moment | Shounen Burst, Ufotable, Cel Shading |
| Nostalgic, 80s–90s retro feel | Retro Anime, Aquarelle |
| Gothic horror, decay | Soulslike, Dark Fantasy, Miura |
| Warm slice-of-life, cozy | Ember, Studio Ghibli, Aquarelle |
| Vibrant gacha/VTuber energy | Gacha Splash, Cinematic Anime |
| Clean modern manhwa | Webtoon, Pixiv Clean, Flat Cel |
| Mascot / vinyl figure / gacha keychain art | Moe Gacha |
| Whimsical fairy tale | Storybook, Studio Ghibli, Gossamer |
| Flat graphic, bold and punchy | Flat Cel, Cel Shading, Flat Chibi |
| Armored characters, mech, tactical | Ironbloom, Miura, Cinematic Anime |
| Candlelit interior, warmth | Ember, Aquarelle, Studio Ghibli |
| Minimal portrait, clean technique | Pixiv Clean, Gossamer, Flat Cel |

---

## Randomization Guidelines

The 3 concepts must feel genuinely distinct — different genre, energy level, and visual
register. Avoid generating three cards in the same emotional key or art direction family.

Vary across these axes:
- **Scale:** intimate portrait vs. two-character scene vs. wide environment shot
- **Energy:** still and quiet vs. mid-motion vs. explosive action
- **Tone:** serious vs. wistful vs. comedic or absurd
- **Palette feel:** dark and moody vs. vivid and warm vs. cool and minimal

Scenes should be specific and visual — describe what the eye sees, not what it means.

- **Weak:** "a girl feeling sad in the rain"
- **Strong:** "a girl in a soaked school uniform standing at an empty crosswalk at 2am, head
  tilted up, eyes closed, letting the rain hit her face — a crumpled letter visible in her
  open hand"

---

## After Concept Selection

Once the user picks a concept (or a mix of elements):

1. Confirm the chosen concept back in one sentence.
2. Ask if they want to add any character details or world specifics before building the blocks,
   or proceed directly.
3. Auto-populate an 8-Block draft from the concept:
   - Block 1: visual expert persona suited to the style (e.g., "an anime key visual illustrator",
     "a manga concept artist", "a cinematic anime art director")
   - Block 2: from Scene field (character, pose, expression, details)
   - Block 3: from Scene field (environment, world, setting)
   - Block 4: composition appropriate to the scene's energy and scale
   - Block 5: lighting derived from Visual Theme
   - Block 6: load the recommended style(s) from styles.md
   - Block 7: mood and palette from Tone and Visual Theme fields
   - Block 8: quality and finish language suited to the style
4. Display the full 8-Block mapping and ask the user to confirm before generating prompts
   (standard Path A flow from this point).
