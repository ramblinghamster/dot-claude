# Style Augmentations

Augmentations are transparent modifier layers applied **on top of** a base style. They
reshape specific blocks while leaving the base style's identity intact. A base style
controls *how the image is rendered*; an augmentation controls *how the scene is framed
and structured*.

---

## AUGMENTATION: Tilt-Shift Miniature

**Aliases:** tilt-shift, miniature, diorama, miniature photography, model village, scale model
**Best for:** Dense urban scenes, port towns, market streets, train stations, cityscapes,
village squares, festival grounds — any scene with many small elements and human figures.
**Poor fit for:** Single-character portraits, close-ups, macro shots, sparse landscapes,
interiors with few elements.

### How It Works

The tilt-shift miniature augmentation makes the scene look like a photograph of a
handcrafted architectural diorama or scale model. The illusion comes from five visual
cues working together — selective focus is the most recognizable, but elevated perspective
and dense detail are equally critical.

### Block Overrides

These blocks are **replaced** by the augmentation. User values for these blocks are
discarded unless the user explicitly overrides the augmentation.

#### Block 4 — Composition & Camera (OVERRIDE)

- **Viewpoint:** Bird's-eye view, elevated rooftop perspective, looking downward at
  approximately 45 degrees.
- **Lens:** Slight telephoto compression (85mm equivalent). No ultra-wide, no fisheye,
  no exaggerated perspective.
- **Focus:** Extremely shallow depth of field with a razor-thin horizontal band of sharp
  focus through the center of the scene. Foreground and background dissolve into soft blur.
- **Aspect ratio:** Default to 16:9 (wide format suits the sprawling layouts that sell
  the miniature illusion). Accept user override.

⚠️ **Conflict:** If the user has already set Block 4 to eye-level, low-angle, close-up,
or macro — flag immediately. These break the miniature illusion.

### Block Modifications

These blocks are **adjusted** — the augmentation injects specific language into the
user's existing values rather than replacing them.

#### Block 2 — Subject (MODIFY)

Inject into the subject description:
- Frame the entire scene as "rendered as a handcrafted architectural diorama" or
  "miniature scale model."
- Add "dozens of tiny [figures/pedestrians/people]" if human figures aren't already
  specified.
- Add dense environmental micro-detail: market stalls, barrels, crates, signs, cables,
  lantern posts, railings, rooftop vents, chimneys, pipes, awnings, carts — whatever
  fits the scene's setting.

#### Block 3 — Environment (MODIFY)

Inject into the environment:
- Density requirement: "every part of the scene rewards close inspection" — no large
  empty areas.
- Scale cues: tiny trees, miniature lampposts, small vehicles or animals proportionate
  to the tiny figures.

#### Block 5 — Lighting (MODIFY)

Add to the existing lighting setup:
- Many tiny practical light sources: glowing windows, warm lanterns, illuminated shop
  signs, amber street lamps.
- Creamy circular bokeh from out-of-focus light sources.
- Gentle cinematic bloom and atmospheric warmth.
- The base style's lighting direction and color temperature are preserved — these
  additions layer on top.

#### Block 7 — Mood & Palette (MODIFY)

Add to the existing mood:
- Vibrant, richly saturated colors (miniatures look more colorful than reality).
- "Handcrafted," "lovingly built," "meticulously detailed" texture language.
- The feeling of peering into a miniature world.
- The base style's emotional tone and palette are preserved — these additions layer
  on top.

### Blocks Not Touched

- **Block 1 — Role:** Stays entirely from the base style.
- **Block 6 — Style:** Stays entirely from the base style. The augmentation does not
  change the rendering approach — anime stays anime, painterly stays painterly.
- **Block 8 — Constraints:** The augmentation adds its own constraints (see below) but
  does not remove any user or style constraints.

### Augmentation Constraints (added to Block 8)

These are automatically added to the negative/exclusion list:
- eye-level camera angle
- low-angle shot
- ultra-wide lens distortion
- deep focus across the entire scene
- large empty areas
- flat lighting

### Platform-Specific Language

#### ChatGPT (DALL-E 3) — Prose Inserts

For anime/illustrated styles, avoid photographic lens language that pulls DALL-E toward
photorealism. Use illustrated equivalents:

| Photographic term | Illustrated equivalent |
|---|---|
| "photographed with a tilt-shift lens" | "framed as a handcrafted miniature diorama" |
| "the camera sits at rooftop height" | "viewed from a bird's-eye elevated perspective" |
| "85mm telephoto compression" | "slight telephoto compression" (keep but don't emphasize) |
| "razor-thin depth of field" | "an extremely shallow depth of field creates a razor-thin horizontal band of sharp focus" (keep — this reads as art direction, not camera spec) |
| "creamy circular bokeh" | keep as-is — bokeh reads well in both photo and illustration |
| "f/1.4 aperture" | omit — too photographic |

**Phase 1 (Style block):** Add the diorama framing to the style declaration. Example:
"Studio Ghibli-inspired anime illustration of [subject] rendered as an exquisitely
handcrafted miniature architectural diorama."

**Phase 2 (Scene block):** Weave in the elevated perspective, selective focus, dense
detail, tiny figures, practical lights, and bokeh as part of the scene description.

#### Niji Journey — Keyword Inserts

Add these keywords to the style group (Group 1):
```
miniature photography, architectural diorama, handcrafted scale model, tilt-shift lens effect
```

Add these keywords to the scene group (Group 2):
```
bird's-eye view looking downward 45 degrees, telephoto compression, razor-thin horizontal
band of sharp focus, soft blur foreground and background, dozens of tiny [figures],
creamy circular bokeh, gentle cinematic bloom
```

Add to `--no`:
```
eye-level angle, deep focus, flat lighting
```

### Element Importance

When trimming for compact prompts, preserve in this priority order:

| Element | Priority | Why |
|---|---|---|
| Selective focus / tilt-shift | Critical (40%) | The defining visual characteristic |
| Elevated bird's-eye viewpoint | Critical (25%) | Without this, miniature illusion breaks |
| Dense miniature detail + tiny figures | High (20%) | Establishes scale |
| Warm practical lighting + bokeh | Medium (10%) | Reinforces the illusion |
| Telephoto compression | Low (5%) | Subtle but helpful |

Compact prompts must keep the top three. Telephoto compression can be dropped first.
