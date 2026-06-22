# Character Creator — Sub-Skill
## Image Prompt Builder — Character Identity Board

This sub-skill guides the user through creating an original character and assembling a
complete CHARACTER IDENTITY BOARD prompt ready to paste into ChatGPT (DALL-E 3).

⚠️ **ChatGPT only.** The 16:9 multi-panel identity board layout relies on spatial composition
control that Niji Journey 7 handles inconsistently. Do not generate a Niji Journey version
for this output format.

---

## Trigger

Activate this sub-skill when the user's intent is to **invent** a character from scratch —
not to depict a character in a scene. Trigger phrases include:

- "create a character" / "design a character"
- "I need a character sheet" / "character identity board"
- "build me a character" / "original character" / "new character"
- "I want a character for my story / game / comic"
- "help me come up with a character"

Do NOT trigger on: "generate an image of a character," "make a scene with," or any request
that describes a scene and happens to include a character — those go to the main skill.

---

## Session Flow

⛔ **NEVER use interactive UI widgets, dropdowns, buttons, or form elements. Plain
conversational chat text only.**

### Step 1 — Parse the request

Extract any fields the user has already provided from their opening message:

| Field | What to look for |
|---|---|
| Character Seed | Core concept, archetype, role, creature type |
| Age / Body Type | Age impression, build, posture, creature anatomy |
| Visual Medium | Rendering style — check Style Library first (see below) |
| Style / Aesthetic | Mood, genre direction, aesthetic tone |
| Optional Details | Outfit hints, palette, personality, props, constraints |

Pre-fill any fields you can extract. Only ask about what's missing.

### Step 2 — Intake (missing fields only)

If any of the 5 fields are missing, ask for them conversationally. You may group them
into a single message if multiple are missing — don't ask one at a time unless only one
is missing.

For **Visual Medium** and **Style**: offer the Style Library as an option.

> *"You can use any of your saved styles for Visual Medium / Style — here are the options:*
>
> Kurosawa · Crewdson · Neon Noir · Editorial Fashion · Studio Ghibli · Dark Fantasy ·
> Ember · Prism · Aquarelle · Ironbloom · Makoto Shinkai · Ufotable · Retro Anime ·
> Cel Shading · Soulslike · Miura · JRPG Pixel Art · Shounen Burst · Moe Gacha · Webtoon ·
> Storybook · Storybook Impasto · Daily Chibi · Velvet · Gacha Splash · Cinematic Anime ·
> Hyperreal Anime · Gossamer · Flat Chibi · Flat Cel · Pixiv Clean
>
> *Or describe your own visual direction."*

If the user references a style by name (e.g., "use Velvet" or "something like Soulslike"),
load that style from `references/styles.md` and use its ChatGPT Translation to populate
the Visual Medium and Style fields. Confirm:

> *"Loaded style: **[Name]** — [one-line visual description]. Applied to Visual Medium and
> Style fields. You can still override any element."*

### Step 3 — Confirm the character before generating

Once all fields are populated, display the full character profile in a single message:

> **Character Profile — confirm before I generate the prompt:**
>
> **Seed:** [value]
> **Age / Body Type:** [value]
> **Visual Medium:** [value]
> **Style / Aesthetic:** [value]
> **Optional Details:** [value or "none"]
>
> *"Does this look right, or would you like to adjust anything?"*

Wait for confirmation. Do not generate the prompt until the user confirms.

### Step 4 — Generate and deliver

Assemble the completed identity board prompt (see template below) and deliver it in a
single fenced code block, ready to paste.

Follow with a brief note reminding the user how to lock the character for future prompts:

> *"Once you generate this in ChatGPT, save the result as your character reference.
> You can upload it as a reference image in future sessions to lock the character's look
> across prompts — see the Character Consistency Workflow in your skill notes."*

---

## Prompt Template

Fill in the bracketed fields from the confirmed character profile. Do not leave any field
as a placeholder — if a detail wasn't specified, invent something appropriate and fitting.

```
Create a fully original, copyright-safe character and present them as an artistic CHARACTER IDENTITY BOARD.

[CHARACTER SEED]:
[value]

[AGE / BODY TYPE]:
[value]

[VISUAL MEDIUM]:
[value]

[STYLE]:
[value]

[OTHER DETAILS - OPTIONAL]:
[value, or omit this section if none]

Invent everything else:
character name, alias or title, role, personality traits, emotional tone, visual theme, outfit design or body design, color palette, signature prop or signature biological feature, recognizable silhouette, pose language, small identity notes.

Originality rules:
The character must not resemble any existing anime, manga, game, movie, comic, celebrity, athlete, mascot, franchise character or known copyrighted creature.
Do not copy recognizable IP elements, costumes, hairstyles, uniforms, weapons, logos, symbols, color combinations, silhouettes, powers or signature visual traits.
Avoid fan-art aesthetics.
Create a fresh visual identity from scratch.

Character authenticity rules:
Create the character with a strong sense of individuality and non-generic design.
Avoid overly polished, overly idealized or repetitive visual features that make the character feel like a default AI-generated face, stock design, cloned archetype or generic creature.

If the character is human or humanoid:
Use distinctive facial structure, subtle asymmetry, natural variation, small imperfections and believable proportions.
The character should feel specific, grounded and recognizably individual.
If the character is attractive, keep the appeal natural, tasteful and appropriate to the chosen visual medium.

If the character is stylized:
Preserve uniqueness through original shape language, expressive proportions, distinctive features, posture and clear personality cues.
Avoid default genre clichés and repeated beauty standards.

If the character is non-human:
Preserve uniqueness through original anatomy, believable biological structure, distinctive proportions, functional features, surface texture and clear personality cues.
Do not make it feel like a generic mascot, pet monster or stock fantasy creature.

Medium and style control:
[VISUAL MEDIUM] controls the rendering language.
[STYLE] controls the aesthetic direction.
The character identity board format is only the presentation format.
The presentation must adapt to [VISUAL MEDIUM] and [STYLE], not override them.
Use visual traits that belong naturally to the selected medium.

Create an artistic 16:9 CHARACTER IDENTITY BOARD.

The board should feel like a curated visual identity presentation, not a generic turnaround sheet.

Board content:
large full-body main character view, neutral full-body view, back view, profile view, secondary attitude pose, 4 to 6 face or expression studies, outfit detail close-ups or anatomy detail close-ups, key prop close-up or signature feature close-up, small silhouette or shape study, color palette strip, short readable identity notes.

Layout:
asymmetrical, elegant, visually memorable, large empty space, clean separation between all views, no overlapping bodies, no cropped faces, no hidden limbs, no clutter.

Text on the board may include:
character name, alias, role, personality traits, core theme, signature prop or feature, color notes.

Background:
pure white or soft off-white, minimal clean graphic design, no environment, no logo, no watermark.

Prioritize:
accurate visual medium, strong unique identity, readable outfit design or anatomy design, clear personality, original character design, natural or stylized individuality as appropriate, believable uniqueness, non-repetitive character design, artistic identity-board presentation.
```

---

## Style Integration Notes

When a Style Library style is used, its ChatGPT Translation should inform the
`[VISUAL MEDIUM]` and `[STYLE]` fields — distilled to the rendering language and
aesthetic direction that best describe the character design context.

Some styles work naturally for identity boards; others need adaptation:

| Style type | How to adapt |
|---|---|
| Anime styles (Cinematic Anime, Hyperreal Anime, Velvet, etc.) | Use directly — strong character design language |
| Flat styles (Flat Cel, Gossamer, Flat Chibi) | Use directly — clean identity board presentation |
| Cinematic/photographic styles (Kurosawa, Crewdson, Neon Noir) | Anchor to anime rendering (see Style Usage Notes in styles.md) |
| Action-scene styles (Shounen Burst, Ufotable, Gacha Splash) | Describe as the visual language, not an action scene — "Ufotable character design language" |

If the user selects a style that pulls strongly toward live-action or photorealism
(Kurosawa, Neon Noir, Crewdson), suggest pairing it with Hyperreal Anime as the
rendering base and using the selected style for aesthetic tone only. Flag this:

> ⚠️ *"[Style] is primarily a cinematic/compositional style. For a character identity board
> I'd suggest anchoring the rendering in **Hyperreal Anime** and using [Style] for the
> mood and aesthetic direction — otherwise the board may render as live-action photography
> rather than character design art. Want me to apply that pairing?"*
