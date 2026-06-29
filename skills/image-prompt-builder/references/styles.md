# Style Library
## Image Prompt Builder — Saved Styles

This file stores your personal named styles. Each style is pre-translated for both ChatGPT
(DALL-E 3) and Niji Journey so it can be applied directly to any prompt without re-describing.

To add a new style, copy any entry below and fill in your own values.
To invoke a style during a session, say its name (e.g., "use Kurosawa" or "apply Neon Noir").

---

## How Styles Are Applied

When a style is loaded, its values override or enrich the following blocks:
- **Block 5 (Lighting):** if the style specifies a lighting approach
- **Block 6 (Style, Medium & Art Direction):** primary style language
- **Block 7 (Mood, Color Palette & Texture):** mood, palette, and texture descriptors

The user can still override any element after the style loads.

---

## STYLE: Sumi-e
**Aliases:** sumi-e, ink wash, sumi, brush ink
**Best for:** character portraits, fantasy creatures, landscapes, any subject where ink brush texture and tonal drama are the point
**Conflicts with:** clean digital linework, flat cel shading, vivid color palettes, glossy rendering

### Visual Description
Traditional Japanese ink wash rendering on textured paper. Black ink tones only — no color.
Form is built through brush pressure variation: bold confident strokes for structure, soft
bleeding washes for shadow and atmosphere. Edges are organic and imperfect — ink bleeds into
paper naturally. White paper serves as light. Tonal range from pure black to pale grey wash.
Paper texture (washi or similar) is always visible. Anime character proportions rendered
through brush technique rather than pen linework.

### Style Negatives
color, clean digital linework, flat cel shading, sharp uniform edges, glossy rendering, gradient backgrounds, photorealistic rendering, chibi proportions, neon lighting

### ChatGPT Translation
```
Traditional sumi-e ink wash anime illustration on textured paper — all form built through
brush pressure variation, bold confident ink strokes for structure, soft bleeding washes for
shadow and volume, organic imperfect edges where ink bleeds into paper, black ink tones only
with full tonal range from pure black to pale grey wash, white paper as light source, visible
paper texture throughout. Drawn as a traditional ink wash illustration — 2D anime proportions,
no color, no digital linework, no sharp uniform edges.
```

### Niji Journey Translation
```
traditional sumi-e ink wash anime illustration, black ink tones, brush strokes, soft bleeding edges, textured paper, tonal shading
```

---

## STYLE: Pencil Sketch
**Aliases:** pencil sketch, pencil drawing, graphite, graphite sketch, pencil art
**Best for:** character portraits, OC showcases, detailed costume studies, fan art, any subject where a monochrome hand-drawn graphite feel is the point
**Conflicts with:** color, clean digital linework, flat cel shading, glossy rendering, painterly styles

### Visual Description
Monochrome graphite pencil drawing on paper. Smooth tonal gradients built through pencil
pressure — soft shading for skin and fabric, denser strokes for shadows and hard edges.
Line quality mixes sharp precise lines for structural detail with softer, looser strokes
for hair and cloth. Visible pencil grain throughout. Grey-scale only — no color. Paper
texture shows through, especially in lighter areas. The paper itself can be plain white
or ruled notebook paper with faint lines visible beneath the drawing.

### Style Negatives
color, clean digital linework, flat cel shading, ink outlines, glossy rendering, gradient backgrounds, painterly blending, airbrush smoothness, photorealistic rendering, neon lighting, chibi proportions

### ChatGPT Translation
```
Traditional graphite pencil anime illustration on paper — smooth tonal gradients built through
pencil pressure variation, mixed sharp and soft line quality, visible pencil grain throughout,
grey-scale only with full tonal range from dark graphite to faint sketch lines, paper texture
visible especially in light areas, denser strokes for shadows and structural edges, softer
looser strokes for hair and fabric. Drawn entirely as a graphite pencil sketch on paper — 2D
anime proportions, no color, no ink outlines, no digital rendering, no airbrush smoothness.
```

### Niji Journey Translation
```
traditional graphite pencil anime sketch, pencil drawing on paper, grey-scale, smooth tonal shading, visible pencil grain, mixed sharp and soft lines, paper texture
--ar [ratio]
```

---

## STYLE: Crewdson
**Aliases:** crewdson, staged, suburban surreal, staged cinema
**Best for:** interior scenes, portraiture, emotionally loaded stillness, suburban or coastal settings
**Conflicts with:** action scenes, fantasy environments, bright comedic tone

### Visual Description
Large-format staged photography aesthetic — images that feel like stills from a film that
doesn't exist. Hyper-real yet constructed, every element in the frame deliberately placed
as though by a set designer. Single dominant light source, often from a window or doorway,
casting raking shadows. Desaturated midtones with warm amber highlights and deep teal
shadows. The subject is always in the middle of something private, emotionally ambiguous,
and slightly melancholic. No direct eye contact.

### Style Negatives
action scenes, bright cheerful palette, fantasy environments, comedic tone, flat cel shading, chibi proportions, clean minimal backgrounds, direct eye contact, energetic poses, saturated vivid colors

### ChatGPT Translation
```
Cinematic large-format staged aesthetic, anime illustration — theatrically composed,
hyper-detailed, every element deliberately placed as though by a set designer, still from
a film that does not exist. Desaturated midtones with rich amber highlights and deep teal
shadows, single raking light source from a window or doorway, long dramatic shadows, quiet
constructed melancholy, emotionally ambiguous narrative, no direct eye contact, 2D anime
art style.
```

### Niji Journey Translation
```
soft painterly anime illustration, staged cinematic composition, warm amber and deep teal palette, single window light, long shadows
```

---

## STYLE: Neon Noir
**Aliases:** neon noir, cyberpunk noir, neon, rain noir
**Best for:** urban night scenes, cyberpunk, mystery/thriller mood, futuristic dystopia
**Conflicts with:** daylight scenes, pastoral environments, warm cheerful palettes

### Visual Description
Rain-slicked streets reflecting neon signage. Deep shadows punctuated by electric magenta,
cyan, and amber. Smoke or steam rising from vents. The city feels alive but predatory.
Figures are silhouetted or partially lit, never fully revealed. High contrast between deep
blacks and intense color. The visual language of cyberpunk noir and hardboiled detective fiction.

### Style Negatives
daylight scenes, pastoral environments, warm cheerful palette, pastel colors, flat cel shading, soft ambient lighting, clean minimal aesthetic, cute or whimsical tone, chibi proportions

### Usage Notes
- **For anime rendering:** Neon Noir alone pulls toward photorealistic/live-action feel.
  To render in anime style, stack Hyperreal Anime as the base rendering layer and apply
  Neon Noir conditions on top. Anchor with descriptors like `semi-realistic 2D anime`,
  `clean anime linework`, `cyberpunk anime aesthetic` to lock the rendering language.
- **Stacking:** Lead prompt with Hyperreal Anime rendering language, then add Neon Noir
  atmosphere conditions (neon color palette, wet reflections, anamorphic flare, etc.).

### ChatGPT Translation
```
Neon noir anime illustration — rain-slicked urban streets reflecting electric neon light in
magenta, cyan, and amber, deep shadow contrast, smoke and steam rising from vents, cinematic
wide shot, figures silhouetted or half-lit, cyberpunk noir atmosphere, mysterious and predatory
mood, wet surface reflections, anamorphic lens flare, desaturated except for neon color pops,
clean anime linework, 2D anime art style.
```

### Niji Journey Translation
```
neon noir anime, electric magenta and cyan neon reflections, deep shadows, clean anime linework, high contrast
```

---

## STYLE: Editorial Fashion
**Aliases:** editorial, fashion editorial, vogue, high fashion, magazine
**Best for:** product shots, portraiture, luxury goods, high-end commercial imagery
**Conflicts with:** rustic/organic environments, heavy texture, fantasy or sci-fi themes

### Visual Description
Clean, controlled, and intentional. Minimal props. Precise directional lighting — often a
large softbox or natural window light — that creates crisp highlights and soft shadow. Color
palette is desaturated and cool, with lifted blacks. The subject commands the frame. Negative
space is used deliberately. Feels like a luxury fashion magazine or high-end commercial spread — elevated, restrained,
and aspirational.

### Style Negatives
rustic organic environments, heavy texture, fantasy or sci-fi elements, cluttered composition, warm saturated palette, painterly rendering, chibi proportions, hand-drawn roughness, busy detailed backgrounds

### ChatGPT Translation
```
High-end editorial fashion anime illustration — clean and minimal composition, precise
directional softbox lighting, crisp highlights with soft shadow falloff, desaturated and
cool color palette with lifted blacks, generous negative space, aspirational and restrained
mood, luxury fashion editorial quality, ultra high detail, 2D anime art style.
```

### Niji Journey Translation
```
editorial fashion anime illustration, minimal composition, soft directional lighting, desaturated cool palette, crisp highlights, negative space
```

---

## STYLE: Studio Ghibli
**Aliases:** ghibli, miyazaki, studio ghibli, ghibli style
**Best for:** nature scenes, childhood wonder, fantasy worlds, quiet emotional moments
**Conflicts with:** dark horror, gritty realism, cyberpunk, hyperrealistic photography

### Visual Description
Warm, painterly, and richly detailed environments that feel handcrafted. Soft natural
lighting — dappled sunlight through leaves, golden afternoon, misty mornings. Nature is
lush and alive. Characters have expressive round features. The mood is wistful, wonder-filled,
and emotionally gentle. Colors are saturated but never harsh — warm greens, soft blues,
golden yellows, deep earth tones.

### Style Negatives
photorealistic, dark horror, gritty realism, cyberpunk neon, hyperrealistic rendering, sharp digital linework, desaturated palette, heavy shadows, dramatic contrast, cold clinical lighting, action poses, violent content

### ChatGPT Translation
```
Studio Ghibli-inspired aesthetic — warm, painterly illustration with handcrafted texture,
soft dappled natural lighting, lush detailed environments, wistful and wonder-filled mood,
emotionally gentle atmosphere, rich saturated warm greens and golden yellows, expressive
character design, classic Japanese anime film visual language.
```

### Niji Journey Translation
```
Studio Ghibli style, soft painterly illustration, warm dappled natural lighting, rich saturated warm palette, handcrafted texture
```

---

## STYLE: Dark Fantasy
**Aliases:** dark fantasy, grimdark, gothic fantasy, dark epic
**Best for:** fantasy characters, creatures, ominous landscapes, epic world-building
**Conflicts with:** cheerful or pastel palettes, comedic tone, minimal clean aesthetics

### Visual Description
Brooding, epic, and atmospheric. Deep jewel tones — emerald, crimson, obsidian — against
near-black backgrounds. Dramatic rim or volumetric lighting. Heavy use of fog, smoke, or
falling ash. Architectural elements are gothic or ancient — crumbling stone, iron, bone.
Characters feel mythic in scale. The world has weight and danger. Grand, threatening, and
mythic — the visual language of dark fantasy concept art at its most epic.

### Style Negatives
cheerful pastel palette, comedic tone, flat cel shading, clean minimal aesthetic, bright daylight, cute proportions, chibi, slice-of-life settings, soft ambient lighting

### ChatGPT Translation
```
Dark fantasy anime illustration — brooding and atmospheric, deep jewel tones of emerald and
crimson against near-black backgrounds, dramatic volumetric rim lighting, heavy fog and smoke,
gothic architectural ruins, crumbling stone and iron, mythic character scale, dangerous and
ancient world, oppressive gothic visual weight, painterly cinematic anime art style, expressive anime linework.
```

### Niji Journey Translation
```
dark fantasy anime illustration, deep jewel tones emerald crimson obsidian, volumetric rim lighting, heavy fog, gothic atmosphere, expressive anime linework
```

---

## STYLE: Ember
**Aliases:** ember, warm matte, lantern glow, tavern glow, matte anime
**Best for:** dark fantasy interiors, tavern/inn scenes, candlelit portraits, visual novel characters, anime with warmth and intimacy
**Conflicts with:** cold/clinical palettes, bright daylight scenes, hyperrealistic photography, cyberpunk neon

### Visual Description
Semi-painterly anime rendering with a matte finish and soft diffuse shading. The signature
element is warm amber light — gentle rim lighting, luminous lantern or candlelight glow —
set against a dark fantasy environment that feels inviting rather than threatening. Soft cel
shading with thin elegant lineart, hand-painted texture, and subtle bloom on light sources.
Faces are softly illuminated, shadows are balanced rather than harsh, and the overall
atmosphere is smoky, rich, and intimate. Feels like a high-quality visual novel illustration
or a cinematic anime still.

### Style Negatives
cold clinical palette, bright daylight, flat cel shading, neon cyberpunk lighting, hyperrealistic rendering, outdoor scenes, desaturated monochrome, harsh high-contrast shadows, action poses

### ChatGPT Translation
```
Semi-painterly anime aesthetic with a matte finish, soft diffuse shading, and cinematic warm
lighting. Gentle amber rim light and luminous lantern glow cast softly illuminated faces
against rich, smoky shadows. Hand-painted anime texture with thin elegant linework, subtle
bloom on light sources, balanced shadows, and warm midtones. Dark fantasy setting with
inviting warmth and tavern ambience — visual novel illustration quality, painterly depth.
```

### Niji Journey Translation
```
semi-painterly anime, matte finish, soft diffuse shading, amber rim light, lantern glow, thin elegant lineart, warm midtones, subtle bloom
```

---

## STYLE: Prism
**Aliases:** prism, crystal light, caustic light, refraction, spectral dispersion, glass light, realistic crystal
**Best for:** characters near or holding refractive objects (glass, crystal, potion bottles, lenses, prisms), product and jewelry close-ups, window-light scenes, any scene where physically accurate light behavior through glass or crystal is the point
**Conflicts with:** holographic/glitter fantasy aesthetics, Neon Noir, dark moody realism without a clear light source, Kurosawa, Crewdson

### Visual Description
A physically accurate light and refraction aesthetic where a real refractive object — a glass
bottle, crystal, prism, lens, or gemstone — is the single source of all light scatter in the
scene. The rendering base is semi-realistic anime (clean linework, smooth gradients, no
painterly texture), but the lighting behavior is governed by optics: white light enters the
object and splits into spectral color bands on exit, caustics — sharp irregular pools of
spectrum color — are projected onto nearby skin, fabric, and surfaces. Chromatic aberration
separates red and violet at the edges of refracted beams. Nothing glows on its own. There is
one coherent light source; the object bends and casts it.

The background is dark or neutral so caustic projections read with maximum clarity. The
palette outside the light effects is restrained — the spectral colors are the only saturation
in the frame. The mood is precise, luminous, and quietly scientific: beautiful because the
physics is beautiful, not because glitter was added. No holographic shimmer, no floating
particles, no ambient neon scatter.

### Style Negatives
holographic shimmer, glitter, neon glow, ambient shimmer, floating particles, sparkles, oversaturated colors, fantasy scatter, lens flare blooms, multiple light sources, painterly texture, rough linework, flat cel shading

### ChatGPT Translation
```
Semi-realistic 2D anime illustration, clean precise anime linework, smooth digital rendering —
physically accurate refraction and caustics lighting. A single refractive object (glass bottle,
crystal prism, gemstone, or lens) is the sole source of light scatter in the scene. Sharp
caustic light projections cast onto skin and fabric from the object only, spectral dispersion
splitting white light into spectrum color bands, chromatic aberration separating red and violet
at refracted beam edges. Dark or neutral background so caustic patterns read clearly. Restrained
palette — spectral refraction colors are the only saturation. No holographic shimmer, no glitter,
no ambient glow, no floating particles. Precise luminous optical realism, anime illustration style.
```

### Niji Journey Translation
```
semi-realistic anime, clean linework, smooth rendering, light refraction caustics, spectral dispersion, chromatic aberration, dark neutral background, restrained palette
--ar 2:3
```

---

## STYLE: Aquarelle
**Aliases:** aquarelle, watercolor anime, soft wash, washi, analog anime, quiet anime, gouache
**Best for:** original character portraits, full-body illustrations, emotionally subtle scenes, understated fantasy, slice-of-life, travel or nature themes
**Conflicts with:** Prism, Neon Noir, Dark Fantasy, dramatic cinematic lighting, glossy/polished aesthetics, sci-fi or magical effects

### Visual Description
A genuine analog watercolor aesthetic where the medium leads and the anime character
design sits loosely within it. The base is a visible pencil or ink underdrawing —
slightly scratchy, imprecise, showing through beneath the color. Watercolor washes
are applied sparsely and unevenly over the sketch, barely contained within outlines,
with large areas of white paper left intentionally unpainted within the hair, clothing,
and body. Nothing is fully rendered. Figures dissolve and fade at the edges, clothing
fades out below the waist into unfinished linework, and the background is almost
entirely absent — raw paper texture with faint color pooling at most.

The palette is near-greyscale: whispers of warm tan, soft grey-blue, and pale peach
that barely read as color. Saturation is suppressed throughout. The overall impression
is a beautiful sketchbook page rather than a finished illustration — intimate,
restrained, and emotionally present through what is left unpainted as much as what
is painted. High quality expressed through incompleteness, not complexity.

### Style Negatives
clean vector lineart, full rendering, detailed background, glossy plastic texture, oversaturated colors, harsh contrast, excessive decoration, dense rendering, dramatic cinematic lighting, magical effects, sci-fi elements, digital smoothness, gacha polish

### ChatGPT Translation
```
Genuine watercolor and ink sketch anime illustration — loose visible pencil and ink
linework underneath soft sparse watercolor washes, large areas of white paper left
intentionally unpainted within the figures, color barely contained within outlines,
washes applied unevenly and incompletely. Figures dissolve and fade at the edges,
clothing and bodies fading into unfinished sketch below. Almost no background —
raw paper texture only with faint color pooling at edges. Near-greyscale palette:
only whispers of warm tan, soft grey-blue, and pale peach, never saturated. Loose
scratchy analog linework, visible brush strokes, intentional incompleteness, quiet
intimate mood. A beautiful sketchbook page, not a finished illustration. No clean
vector lines, no full rendering, no detailed background, 2D anime sketch style.
```

### Niji Journey Translation
```
watercolor ink sketch anime, visible pencil linework under sparse washes, white paper areas unpainted, near-greyscale palette warm tan soft grey-blue, loose scratchy linework, sketchbook aesthetic
--ar 2:3
```

---

## STYLE: Ironbloom
**Aliases:** ironbloom, iron bloom, tactical anime, arms girl, gear girl, mech contrast, tactical ink, mil-moe, military manga, ink mecha, hard ink, mech sketch
**Best for:** characters with complex armor, mechanical suits, military/tactical gear, fantasy plate armor, sci-fi equipment, steampunk machinery — any scene contrasting a soft anime character with hard technical detail. Fantasy, sci-fi, military, steampunk, post-apocalyptic, pilot portraits all work.
**Conflicts with:** Aquarelle, Studio Ghibli, soft painterly styles, lush detailed backgrounds, warm intimate interiors

### Visual Description
The defining tension of this style is a soft anime character face and fragile human presence set against hyper-detailed, technically precise mechanical or structural complexity — armor, gear, weapons, equipment, machinery. The contrast between delicate and formidable is always the point. Both sub-moods render against a white or near-white negative space background that isolates the subject.

### Style Negatives
lush detailed backgrounds, painterly atmospheric rendering, soft warm interiors, pastel palettes, cute aesthetic, chibi proportions, flat cel shading without detail contrast, glossy smooth digital finish

**Rendered sub-mood:** Semi-flat cel shading with visible rendering depth. Earth and neutral tones (sand, khaki, olive, dark brown). Equipment rendered with technical-illustration precision — every buckle, panel, joint, and surface detail present and readable. Often carries a thematic juxtaposition: something delicate (a flower, a small creature, a gentle gesture) against something formidable.

**Flat/Ink sub-mood:** Flat manga ink linework. Each armor panel has a large flat interior with clean color fill and no hatching or crosshatch shading. Wear is sparse and surgical — a few strategic grime dots or scratch lines only. Line economy over density. Negative space preserved aggressively within the armor, around the subject, and in the background. Result feels light and airy despite mechanical complexity. Palette is fully user-defined — not locked to earth tones.

### Usage Notes
- Ask which sub-mood if context doesn't make it clear
- Rendered sub-mood: earth tones default, more rendering depth, thematic delicacy contrast
- Flat/Ink sub-mood: palette-agnostic, flat fills, line economy — lighter and more graphic

### ChatGPT Translation

**Rendered sub-mood:**
```
Clean bold manga lineart with semi-flat shading and hyper-detailed technical rendering of
complex armor or equipment. Muted earth tone palette of sand, khaki, olive, and dark brown
against a white or near-white negative space background. Soft expressive anime character
face contrasted with precisely rendered mechanical or structural complexity — every panel,
joint, and surface detail present. Emotionally resonant thematic contrast between something
formidable and something delicate. Technical illustration precision, manga quality, 2D anime
art style.
```

**Flat/Ink sub-mood:**
```
2D manga illustration, flat clean ink linework, anime character with soft expressive face —
mechanically complex armor and tactical hardware rendered with structural precision: clean
panel seam lines, joint assemblies, bolt and cable detail, large flat color fills inside each
armor panel with no hatching or texture, sparse intentional wear limited to a few strategic
grime dots and scratch marks, strong contrast between soft anime face and hard mechanical
structure, generous negative space preserved throughout including within the armor, minimal or
white background, line economy over density, light airy feel despite mechanical complexity,
[user-defined palette], professional manga illustration quality.
```

### Niji Journey Translation

**Rendered sub-mood:**
```
bold manga lineart, hyper-detailed armor, semi-flat shading, muted earth tones, white background, soft anime face with hard mechanical contrast
```

**Flat/Ink sub-mood:**
```
flat manga ink linework, soft anime face, flat color fills no hatching, sparse wear marks, white background, line economy, [user-defined palette]
--ar [ratio]
```

---

## STYLE: Makoto Shinkai
**Aliases:** makoto shinkai, shinkai, luminous sky, shinkai sky, atmospheric sky anime
**Best for:** emotional outdoor scenes, dramatic skies, distance and longing, cityscapes at golden hour, two characters separated by space or light
**Conflicts with:** interior-only scenes, Kurosawa monochrome, flat design, hard toon cel shading

### Visual Description
Inspired by a distinctive strand of contemporary Japanese animated films — hyper-detailed
atmospheric skies with layered clouds, lens flares, and luminous volumetric light rays that
feel almost tactile. Colors are intensely saturated but natural: deep blues, burning ambers,
electric golds. Backgrounds are rendered with near-photographic detail while characters retain
clean anime stylization, creating a dreamlike contrast. Emotional depth comes from light —
the way it falls on a face, refracts through rain, or floods a train window. A pervasive
sense of distance, longing, and beauty in transience.

### Style Negatives
interior-only scenes, monochrome palette, flat cel shading, hard toon outlines, chibi proportions, minimal backgrounds, dark enclosed spaces, desaturated colors

### ChatGPT Translation
```
Luminous atmospheric sky anime illustration — hyper-detailed sky with layered clouds and
luminous volumetric light rays, lens flare, intensely saturated natural colors in deep blues
and burning amber gold, richly detailed painterly background contrasting with clean anime character
stylization, emotional depth through light and distance, dreamlike beauty, sense of longing
and transience, cinematic anime composition.
```

### Niji Journey Translation
```
luminous sky anime style, hyper-detailed clouds, volumetric light rays, lens flare, saturated deep blue amber gold palette, detailed painterly background, clean anime characters
```

---

## STYLE: Ufotable
**Aliases:** ufotable, ufotable dark fantasy, dark fantasy action anime, supernatural anime spectacle
**Best for:** action sequences, dark fantasy combat, supernatural scenes, dramatic character moments, high-production anime key visuals
**Conflicts with:** Aquarelle, Kurosawa monochrome, flat design, retro anime

### Visual Description
The signature visual language of Ufotable animation studio — high-production dark fantasy
anime at its most cinematic. High-contrast dramatic lighting with richly saturated jewel-toned
colors: deep crimson, electric blue, vivid gold against near-black shadows. Cinematic polish
with fluid motion energy even in still images. Characters are rendered with meticulous detail
and glowing intensity — effects like fire, water, and supernatural energy are rendered as
breathtaking visual spectacles. The overall feel is expensive, dramatic, and technically
flawless. Dark settings are elevated by explosive color rather than muted.

### Style Negatives
flat cel shading, retro analog grain, watercolor texture, monochrome palette, minimal backgrounds, chibi proportions, soft ambient lighting, muted desaturated colors, hand-drawn roughness

### ChatGPT Translation
```
Ufotable animation studio aesthetic — high-contrast dramatic lighting, richly saturated jewel
tones of deep crimson, electric blue, and vivid gold against near-black shadows, cinematic
production polish, meticulous character detail with glowing intensity, supernatural energy
effects rendered as visual spectacle, fluid motion energy, expensive and technically flawless
dark fantasy anime quality, premium high-production anime visual language.
```

### Niji Journey Translation
```
Ufotable studio style, high contrast dramatic lighting, saturated jewel tones crimson blue gold, near-black shadows, cinematic anime polish, glowing energy effects
```

---

## STYLE: Retro Anime
**Aliases:** retro anime, 80s anime, 90s anime, vhs anime, old school anime, analog anime, retro sci-fi anime
**Best for:** nostalgic scenes, action and drama, urban or sci-fi settings, character-driven moments, any scene benefiting from analog warmth and grain
**Conflicts with:** Prism, Ufotable, clean modern anime aesthetics, hyperrealistic rendering

### Visual Description
The visual language of 1980s–90s anime — cel-animated sci-fi action, urban drama, space
opera, and fantasy adventure from that era. Analog warmth with visible film grain and subtle
color bleed at edges. Linework is slightly thicker and less precise than modern anime, with a
hand-drawn quality that feels intentional and characterful. Color palette has a distinctive
muted warmth — faded yellows, dusty blues, warm oranges — as if slightly sun-bleached or
viewed through a VHS lens. Cel animation textures, limited color banding, and the occasional
halftone dot pattern. Emotionally direct and kinetic. Crucially, background and surface detail
is limited to what genuine vintage cel animation production would allow — flat gouache-style
color blocks, broad simple shapes, and minimal texture complexity. Modern AI tendency to add
fine grain, intricate surface texture, or high-frequency detail is antithetical to this style.

### Style Negatives
clean modern digital linework, hyperrealistic rendering, smooth gradients, fine surface texture, photographic grain, high-frequency detail, complex material rendering, intricate background texture, modern digital detail levels

### ChatGPT Translation
```
Retro 1980s–90s anime aesthetic — analog film grain, subtle VHS color bleed at edges,
slightly thick hand-drawn linework, muted warm palette of faded yellows, dusty blues, and
warm oranges, cel animation texture, limited color banding, emotionally direct and kinetic
energy, classic retro anime visual language, nostalgic analog warmth, hand-crafted
imperfection over digital polish. Authentic hand-painted cel animation production art — flat
broad color fills with minimal texture detail, limited cel layers, backgrounds painted in flat
gouache-style blocks with low detail complexity, simple clean shapes over intricate surface
detail, color limited to what a 1980s anime production budget would allow. No fine surface
texture, no photographic grain, no high-frequency detail, no complex material rendering, no
modern digital detail levels, no intricate background texture.
```

### Niji Journey Translation
```
retro 80s 90s anime, analog film grain, thick hand-drawn linework, muted warm palette faded yellows dusty blues, cel animation texture, flat broad color fills, simple clean shapes
```

---

## STYLE: Cel Shading
**Aliases:** cel shading, cel shaded, bold outline, graphic anime, toon shading, comic shading, graphic toon
**Best for:** action scenes, graphic novels, high-energy characters, poster compositions, any scene where bold graphic impact matters more than realism
**Conflicts with:** Aquarelle, Crewdson, Makoto Shinkai, any painterly or atmospheric style

### Visual Description
Bold black outlines, flat color fills, and high-contrast shading with no gradients — the
visual language of toon-shaded action games, comic books, and graphic novel illustration.
Colors are vivid and fully saturated. Shading is binary: lit or shadow, with a hard edge
between them. Linework is thick, confident, and expressive. The overall effect is graphic,
energetic, and immediately readable. Depth comes from composition and color contrast rather
than rendering subtlety. Feels designed to be seen from a distance and understood instantly.

### Style Negatives
gradients, painterly rendering, soft atmospheric shading, watercolor texture, photorealistic rendering, subtle shadow transitions, muted desaturated palette, thin invisible outlines

### ChatGPT Translation
```
2D anime cel shading illustration — bold black outlines, flat fully-saturated color fills,
high-contrast binary shading with hard edges between light and shadow, no gradients,
thick confident expressive linework, vivid color palette, graphic novel and toon-shaded
game visual language, energetic and immediately readable, depth through composition and color
contrast rather than rendering subtlety.
```

### Niji Journey Translation
```
anime cel shading, bold black outlines, flat color fills, no gradients, thick expressive linework, vivid saturated colors, toon shading
```

---

## STYLE: Soulslike
**Aliases:** soulslike, souls aesthetic, gothic horror fantasy, gothic action rpg, ruin aesthetic
**Best for:** gothic architecture, horror fantasy, fog-shrouded landscapes, cursed or corrupted characters, bleak and grand environments, ancient decaying worlds
**Conflicts with:** Ember, Ghibli, Makoto Shinkai, warm or inviting aesthetics

### Visual Description
The visual language of gothic action RPG concept art — a desaturated, fog-heavy gothic
aesthetic where grandeur and dread occupy the same space. Color palette is predominantly
grey, ash, and muted teal with isolated accents of deep amber or bloodred. Architecture
is massive, decaying, and inhuman in scale. Characters are dwarfed by their environments.
Fog, ash particles, and atmospheric haze obscure backgrounds, creating mystery and weight.
Unlike Dark Fantasy (which uses jewel tones and epic warmth), Soulslike is bleaker, quieter,
and more unsettling — beauty that comes from ruin.

### Style Negatives
warm inviting palette, bright saturated colors, cute aesthetic, chibi proportions, cheerful mood, clean minimal backgrounds, flat cel shading, comedic tone, pastoral or nature scenes

### ChatGPT Translation
```
Gothic action RPG soulslike anime illustration — desaturated gothic atmosphere in grey, ash, and
muted teal with isolated accents of deep amber or bloodred, massive decaying architecture
that dwarfs human scale, fog and ash particles obscuring the background, a pervasive sense
of ancient ruin and quiet dread, grandeur and horror coexisting, bleaker and more unsettling
than traditional dark fantasy, gothic horror RPG concept art aesthetic, 2D anime art style, detailed anime linework.
```

### Niji Journey Translation
```
soulslike gothic anime, desaturated grey ash muted teal, deep amber accents, massive decaying architecture, atmospheric fog and ash, detailed anime linework
```

---

## STYLE: Miura
**Aliases:** miura, dark manga, crosshatch, crosshatch manga, dense ink manga
**Best for:** intense character portraits, brutal battle scenes, dark fantasy figures, deeply detailed armor and weapons, monochromatic or limited-color dramatic compositions
**Conflicts with:** Ghibli, Aquarelle, Ember, soft or colorful styles

### Visual Description
The aesthetic of peak-craft dark fantasy manga — one of the most technically demanding
illustration styles ever produced. Dense, precise crosshatching builds shadow and texture in
ways that feel almost engraved. Linework is extraordinarily detailed, with heavy blacks that
create dramatic contrast. Armor, weapons, and environmental detail are rendered with obsessive
specificity — every rivet, scratch, and surface texture accounted for. Figures feel massive
and heavy. The overall aesthetic is monochromatic or near-monochromatic, with shadow doing
the emotional and atmospheric work. Brutal, meticulous, and awe-inspiring.

### Style Negatives
soft colorful palette, flat cel shading, clean digital linework, cute aesthetic, chibi proportions, watercolor texture, pastel colors, minimal linework, cheerful mood, simplified detail

### ChatGPT Translation
```
Peak-craft dark fantasy manga aesthetic — dense precise crosshatching building shadow and
texture with engraving-like depth, extraordinarily detailed linework, heavy blacks creating
dramatic contrast, obsessively detailed armor and weapons with every rivet and scratch
rendered, massive and heavy figure weight, monochromatic or near-monochromatic palette with
shadow doing the emotional work, brutal meticulous and awe-inspiring dark manga quality.
```

### Niji Journey Translation
```
dark fantasy manga, dense crosshatching, heavy black ink shadows, extraordinarily detailed linework, near-monochromatic, massive figure weight
```

---

## STYLE: JRPG Pixel Art
**Aliases:** jrpg pixel art, pixel art, pixel sprite, hd pixel, jrpg sprite, modern pixel art, hd-2d pixel
**Best for:** fantasy characters with detailed equipment, knight and warrior sprites, character portrait sprites, any subject that benefits from the contrast between pixel grid constraints and rich anime-influenced design
**Conflicts with:** painterly or atmospheric styles, Aquarelle, Crewdson, Makoto Shinkai, any style relying on smooth lineart or gradients

### Visual Description
High-resolution modern pixel art with an anime-influenced character aesthetic — not chunky
16x16 retro pixel work, but a detailed fine-grid approach where every pixel is intentional
and expressive. Character proportions and facial features follow anime conventions: large
expressive eyes, styled flowing hair with visible pixel curl and movement, soft round face.
Equipment and armor are rendered with rich full-color pixel shading using careful dithering
and color stepping to simulate volume and metallic sheen. The palette is full-color rather
than limited, with warm skin tones, deep jewel accents, and clean neutrals. Background is
near-white or absent, isolating the character as a standalone sprite. Sits closest to modern
JRPG sprite work — HD-2D fine-grid pixel RPG art, high-end mobile RPG character art, or premium gacha
game sprites.

### Style Negatives
smooth gradients, soft anti-aliased edges, vector linework, painterly rendering, atmospheric lighting, watercolor texture, photorealistic rendering, smooth digital finish

### ChatGPT Translation
```
Pixel art sprite with visible square pixels — every element built from a discrete pixel grid,
NO smooth gradients, NO soft anti-aliased edges, NO vector linework. Style reference: Octopath
Traveler HD-2D sprite, Tactics Ogre Reborn unit sprite, Final Fantasy Tactics character artwork.
Anime-influenced character design rendered entirely in pixel form: large expressive eyes drawn
from individual pixel clusters, flowing styled hair built from stepped pixel color bands, detailed
fantasy armor with full-color pixel shading and manual dithering to simulate metallic volume and
jewel-toned accents. Warm skin tones, near-white or transparent background isolating her as a
standalone sprite. The pixel grid must be visible — this is a pixelated image, not an
illustration of pixel art.
```

### Niji Journey Translation
```
JRPG pixel art sprite, visible pixel grid, Octopath Traveler HD-2D style, dithered shading, full color palette, pixelated not smooth
--ar 2:3
```

### Usage Notes
- **DALL-E 3 drift warning:** DALL-E consistently interprets "pixel art aesthetic" as smooth anime illustration. The ChatGPT translation above uses hard constraints ("visible square pixels", "NO smooth gradients", game references) to fight this — always use the full translation, never paraphrase.
- If DALL-E still ignores pixels: prepend "Pixelated game sprite in the style of Octopath Traveler —" to the subject description.
- Niji Journey produces cleaner pixel results than DALL-E for this style.

---

## STYLE: Shounen Burst
**Aliases:** shounen burst, shounen, modern shounen, action anime, railgun, supernatural action, warm action
**Best for:** characters with supernatural abilities, school or urban settings mid-destruction, power awakening moments, action scenes where the contrast between a warm decaying world and cold or sharp supernatural force is the emotional anchor
**Conflicts with:** Soulslike, Kurosawa, Crewdson, Aquarelle, any style requiring restraint or quiet atmosphere

### Visual Description
A modern digital anime style where a warm, aged-paper world collides with cold or sharp
supernatural force. Backgrounds and environments are pushed into warm sepia and cream tones —
walls, floors, and debris feel sun-bleached or faded, almost like the world itself is old
paper. Against this warm decay, the character's power cuts through as something cold, sharp,
or sudden. The specific effect can take any form — electric arcs, shadow tendrils, wind
pressure waves, ice, void energy, or pure kinetic force — as long as it reads as *cold,
sharp, or sudden* against the warm environmental decay. The contrast between the warm world
and the cold power is the point, not the specific ability. Character rendering is clean and
precise with fuller, more saturated color than the environment. Environments feature high
detail — rubble, cracked surfaces, scattered debris — with strong volumetric backlit window
light. The character is always mid-motion but composed: determined, not frantic.

### Style Negatives
quiet restrained atmosphere, monochrome palette, flat cel shading, watercolor texture, static poses, soft ambient lighting, pastel cheerful mood, minimal backgrounds

### ChatGPT Translation
```
Modern shounen action anime aesthetic — warm sepia-toned environment rendered like aged paper
(cream, yellow-brown, dusty warm gray) contrasted with a crisp cold or sharp supernatural
effect (electric arcs, shadow energy, wind pressure, void force, or kinetic impact — anything
that reads as sudden and cold against warm decay), high-detail environmental destruction
(rubble, cracked surfaces, scattered debris), clean precise character rendering with clean anime linework, fuller
color against the warm environmental chaos, strong volumetric backlit window light creating
haze and silhouette contrast, character mid-action but composed and determined.
```

### Niji Journey Translation
```
modern shounen anime, warm sepia tones, cold sharp supernatural energy contrast, environmental destruction debris, clean anime linework, volumetric backlit light
--ar 2:3
```

---

## STYLE: Moe Gacha
**Aliases:** moe gacha, gacha, chibi gacha, cute chibi, fantasy chibi, chibi knight, chibi warrior, gacha chibi
**Best for:** any character in dynamic action regardless of genre — fantasy warriors, magical girls, school uniforms, sci-fi suits, sports characters, mecha pilots — any scene where full chibi proportions and warm cinematic energy combine. The chibi scale and action energy are the constants; the theme is fully user-defined.
**Conflicts with:** Miura, Soulslike, Kurosawa, any dark gritty or restrained aesthetic

### Visual Description
The full chibi action art aesthetic of gacha games — characters rendered at extreme
chibi proportions where the head is roughly one-third to one-half of total body height,
creating a tiny-but-capable figure that feels both adorable and powerful. Works across any
genre: fantasy armor, school uniforms, sci-fi suits, magical girl costumes, sports gear,
mecha pilot suits — the chibi scale and dynamic energy are the constants, not the theme.
Linework is clean and precise with subtle weight variation. Cel shading is crisp and flat
rather than painterly — smooth color transitions, clean shadow edges, no heavy gradients.
Equipment and outfits are rendered with care despite the chibi scale. Weapons and props are
oversized relative to the character, which reads as charming rather than absurd at chibi
proportions. Hair is flowing and wind-swept with good strand separation. Poses are dynamic
— low-angle action shots, mid-charge, debris and particles in motion. Lighting is warm and
atmospheric: golden ambient glow, floating light particles, soft environmental haze.
Backgrounds are soft-focus and supportive rather than detailed — ruins, classrooms, space
stations, arenas, wherever the scene is set. The overall mood is cute and determined — a
small figure with complete confidence. Closest to premium gacha game chibi sprites and
high-end mobile RPG in-game character art.

### Style Negatives
dark gritty atmosphere, monochrome palette, realistic proportions, heavy crosshatching, desaturated colors, static poses, painterly rendering, complex detailed backgrounds

### ChatGPT Translation
```
Full chibi gacha art aesthetic — extreme chibi proportions with large round head roughly
one-third to one-half of total height and tiny elegant body, clean precise anime linework
with crisp flat cel shading and smooth clean shadow edges, detailed character outfit or
equipment rendered carefully at chibi scale (fantasy armor, school uniform, sci-fi suit,
magical girl costume, or any genre), oversized weapon or prop proportional to chibi frame,
flowing wind-swept hair with strand separation, dynamic low-angle action pose with debris
and motion particles, warm golden ambient lighting with floating atmospheric particles,
soft-focus background appropriate to the scene's setting, cute determined expression,
confident and capable despite small frame, premium gacha chibi character art quality.
```

### Niji Journey Translation
```
chibi proportions large head tiny body, clean linework crisp flat cel shading, oversized weapon chibi scale, dynamic action pose, warm golden lighting, gacha chibi art
--ar 16:9
```

---

## STYLE: Webtoon
**Aliases:** webtoon, manhwa, korean webtoon, line webtoon, manhwa art, korean manhwa
**Best for:** dramatic character moments, fashion-forward character designs, urban fantasy, action sequences, romance and slice-of-life, any scene that benefits from crisp clean linework and strong character presence
**Conflicts with:** Kurosawa, Aquarelle, Crewdson, painterly or atmospheric styles, anything requiring analog texture or heavy environmental mood

### Visual Description
The clean, high-polish aesthetic of Korean webtoon and manhwa — premium manhwa action and
romance visual language. Linework is crisp and confident with consistent weight, slightly
rounder and more fashion-forward than Japanese manga. Shading is smooth and controlled, often
cel-style with soft gradient accents on hair and skin. Characters are the undisputed focal
point — faces expressive, hair rendered with precision and volume, clothing detailed and
fashion-conscious. Color is saturated but clean; palettes are deliberate rather than
atmospheric. Backgrounds are either high-detail and architectural or minimal, depending on
the scene. The overall feel is polished, modern, and cinematic — built for scrolling vertical
presentation but striking in any format.

### Style Negatives
analog texture, heavy environmental mood, painterly rendering, watercolor washes, film grain, rough hand-drawn linework, monochrome palette, atmospheric haze

### ChatGPT Translation
```
Korean webtoon and manhwa aesthetic — crisp confident linework with consistent line weight,
smooth cel shading with soft gradient accents on hair and skin, fashion-forward character
design with expressive faces and precisely rendered hair volume, saturated clean color
palette, characters as the primary focal point against either high-detail architectural
backgrounds or minimal clean settings, polished cinematic production quality, premium Korean webtoon
and manhwa visual language.
```

### Niji Journey Translation
```
Korean webtoon manhwa style, crisp clean linework, smooth cel shading soft gradients, fashion-forward character design, saturated clean palette
--ar 9:16
```

---

## STYLE: Storybook
**Aliases:** storybook, children's book, picture book, gouache illustration, storybook illustration, fairy tale art
**Best for:** fairy tale scenes, animal characters, young protagonists, whimsical fantasy, nature and forest settings, any scene that should feel warm, safe, and wonder-filled
**Conflicts with:** dark or violent themes, Soulslike, Miura, Neon Noir, any style requiring dramatic tension or adult emotional weight

### Visual Description
The warm, handcrafted aesthetic of classic illustrated children's books — gouache or
watercolor washes over ink linework, with soft rounded shapes and an inviting color palette
of warm ochres, sage greens, dusty roses, and cream. Compositions are clear and readable,
with subjects front and center and environments rendered as simplified but characterful
backdrops. Texture is visible — paper grain, brush marks, the slight irregularity of
hand-applied media. Characters have round, expressive features with large eyes and simplified
anatomy. The mood is wonder, safety, and gentle whimsy — the world is slightly magical but
never threatening. Closest to Maurice Sendak, Beatrix Potter, or the picture book style of
a Studio Ghibli storyboard.

### Style Negatives
dark violent themes, dramatic tension, adult emotional weight, sharp digital linework, hyperrealistic rendering, neon lighting, desaturated palette, complex detailed backgrounds, action poses

### ChatGPT Translation
```
Anime storybook illustration — soft warm painterly anime rendering with a gouache-like
digital finish, rounded anime characters with large expressive eyes and soft simplified
silhouettes, warm inviting color palette of ochres, sage greens, dusty roses, and cream,
gentle brush texture and soft color washes, whimsical fairy tale environments with clearly
readable illustrated backgrounds, mood of wonder, safety, and gentle warmth, Japanese anime
picture book and Ghibli artbook visual language.
```

### Niji Journey Translation
```
anime storybook illustration, gouache-like painting, rounded characters large eyes, warm palette ochre sage green dusty rose, gentle brush texture, simplified backgrounds
--ar 4:3
```

---

## STYLE: Storybook Impasto
**Aliases:** storybook impasto, heavy gouache, textured gouache, impasto picture book, thick paint storybook, dry-brush storybook
**Best for:** fairy tale scenes, animal companions, whimsical fantasy, nature settings, any scene that should feel tactile, handcrafted, and warmly painted rather than digitally smooth
**Conflicts with:** dark or violent themes, Soulslike, Miura, Neon Noir, any style requiring dramatic tension or adult emotional weight; also conflicts with glossy/sharp-rendering styles like Prism, Cinematic Anime, and Hyperreal Anime, since impasto texture works against polished surface sheen

### Visual Description
A heavier, more physically tactile variant of Storybook. Where Storybook uses soft gouache
washes, Storybook Impasto leans into thick, opaque paint applied with visible, confident
brushstrokes — dry-brush streaks, ridges of built-up pigment, and the tooth of the painting
paper showing through thinner passages. Color is laid down in flat, simplified blocks rather
than fine gradients; fur, foliage, and fabric are suggested through brushwork rather than
rendered in detail. Characters retain Storybook's round, expressive features and warm
palette of ochres, sage greens, dusty roses, and cream, but surfaces avoid any glossy,
glassy, or digitally smooth finish — even reflective materials like crystal or metal are
rendered as flat matte facets of color. Lighting stays soft and even, without dramatic rim
light or cinematic highlights, keeping the focus on the handmade, textured quality of the
paint itself.

### Style Negatives
glossy digital finish, glassy shine, smooth digital rendering, dramatic rim light, cinematic highlights, sharp precise linework, photorealistic texture, fine detail rendering, polished surface sheen, clean vector lines

### ChatGPT Translation
```
Anime storybook illustration, painted entirely in a thick, opaque gouache style with heavy visible brushwork. Every surface carries the chalky, matte texture of hand-applied gouache pigment — soft, slightly uneven brushstroke edges, visible dry-brush streaks, and the gentle tooth of painting paper showing through thin areas of color. Subjects are rendered in flat, simplified color blocks with thick, confident brushstrokes and visible ridges of dried paint rather than fine detail, fur strands, or digital smoothness. Even reflective or crystalline materials are painted as flat matte facets with no glossy or glassy shine. Lighting is soft and even, with no dramatic rim light or cinematic highlights. Rounded, simplified silhouettes in a warm palette of ochres, sage greens, dusty roses, and cream evoke the tactile, handcrafted feel of a classic illustrated picture book page — fully gouache-painted, with no digital sheen or cinematic rendering.
```

### Niji Journey Translation
```
anime storybook illustration, thick gouache texture, heavy visible brushstrokes, flat matte color blocks, rounded characters large eyes, warm palette ochre sage green dusty rose, hand-painted look
--no glossy shine, digital smoothness, rim light, cinematic highlights
--ar 4:3
```

---

## ADD YOUR OWN STYLE

## STYLE: Gacha Splash
**Aliases:** gacha splash, anime splash, key visual, gacha art, vtuber art, jrpg splash, anime key visual, gacha key visual
**Best for:** high-energy character moments, fantasy RPG characters, VTuber key visuals, spell casting and power moments, dynamic poses with motion, any scene that needs premium cinematic gacha production quality
**Conflicts with:** Kurosawa, Crewdson, Miura — anything restrained, dark, or static in a grounded way; this style is inherently energetic and polished

### Visual Description
The premium action splash art aesthetic of high-end gacha games, JRPG key visuals, and
VTuber promotional art. Semi-chibi proportions — head slightly oversized relative to the
body, petite elegant limbs, stylized anatomy that reads as cute but capable. Clean precise
digital linework with subtle line weight variation and no rough strokes. Rendering is a
hybrid of cel shading and painterly gradients: smooth transitions between shadows,
airbrushed skin, glossy hair highlights with fine strand separation, metallic sheen on
armor and weapons. Lighting is cinematic and atmospheric — warm ambient bloom, rim lighting
around hair and armor edges, floating light particles, soft environmental haze. Composition
is dynamic and character-centered: motion flow, perspective exaggeration, and depth-of-field
blur push the character forward. Weapons are oversized and decorative. Backgrounds are soft-
focus RPG environments — castle courtyards, magical interiors, atmospheric ruins — that
support the character rather than compete. The overall register is magical, heroic, and
elegant — premium anime production quality in every detail.

### Style Negatives
restrained static composition, monochrome palette, rough hand-drawn linework, flat cel shading, watercolor texture, desaturated muted colors, grounded realism, minimal backgrounds

### ChatGPT Translation
```
Modern fantasy anime gacha splash art aesthetic — semi-chibi proportions with slightly
oversized head and petite elegant body, clean precise digital linework, hybrid cel shading
with painterly gradients and airbrushed skin, glossy layered hair highlights with fine
strand separation, metallic armor sheen, cinematic anime lighting with warm bloom, rim
lighting on hair and armor edges, floating atmospheric light particles, dynamic
character-centered composition with motion flow and depth-of-field background blur,
oversized decorative fantasy weapon or magical effect, soft-focus RPG fantasy environment
background, magical heroic and elegant mood, VTuber key visual and JRPG splash art quality.
```

### Niji Journey Translation
```
gacha splash anime art, semi-chibi proportions, clean precise linework, hybrid cel shading painterly gradients, glossy hair highlights, warm bloom rim lighting, floating particles, dynamic motion composition, depth of field
--ar 2:3
```

---

## STYLE: Cinematic Anime
**Aliases:** cinematic anime, studio anime, anime key art, premium anime illustration, anime concept art, visual novel art
**Best for:** character portraits with real-world equipment, motorsport and race characters, action characters at rest, fantasy OCs in grounded settings, strong directional lighting scenes, high production quality without photorealism
**Conflicts with:** Hyperreal Anime (photorealistic skin/materials vs. illustrated), flat cel shading, chibi proportions, Ironbloom flat/ink sub-mood (ink lines vs. painted rendering)

### Visual Description
High-quality 2D anime digital illustration with cinematic lighting and production values.
Rendering stays firmly within anime illustration language — smooth clean anime skin with no
photographic texture, material detail that reads as expertly illustrated rather than
photographically accurate. Leather looks like drawn leather. Sweat and grime are rendered
in anime vocabulary: beaded sweat drops, illustrated dirt smudges, stylized wear. Lighting
is strong and directional — hard shadows, warm color grading, rim light on hair and
shoulders — but it illuminates an illustration, not a render. Natural anime proportions
throughout; nothing crosses into 3D or photorealistic territory. The overall register is
the premium production quality of high-end game concept art, visual novel key visuals, or
prestige anime promotional art.

### Style Negatives
photorealistic skin texture, 3D rendering, flat cel shading, chibi proportions, rough hand-drawn linework, watercolor texture, monochrome palette, soft ambient-only lighting

### ChatGPT Translation
```
High-quality 2D anime digital illustration with cinematic lighting — smooth clean anime
skin with no photographic texture, illustrated material detail with depth and volume on
clothing and gear, strong directional sunlight with warm golden color grading, hard shadows
and rim lighting, rendering that stays clearly within anime illustration language throughout,
anime-style detail language for sweat and wear, natural anime proportions, premium game
concept art or visual novel illustration quality.
```

### Niji Journey Translation
```
cinematic anime illustration, smooth clean anime skin, strong directional sunlight, warm golden color grading, hard shadows rim lighting, natural anime proportions
--ar 2:3
```

---

## STYLE: Hyperreal Anime
**Aliases:** hyperreal anime, photoreal anime, semi-realistic anime, 3D anime, realistic anime, chillout, cinematic anime portrait
**Best for:** elf/fantasy OC portraits, character close-ups, race-suit or armored characters with real material texture, emotionally quiet portrait moments, scenes where anime stylization meets photographic lighting
**Conflicts with:** flat cel shading, retro/grain aesthetics, chibi proportions, hard ink outlines, heavy stylization

### Visual Description
A rendering aesthetic where anime character design — expressive eyes, stylized facial structure,
fantasy features like pointed ears — meets near-photographic realism in everything else.
Skin has actual texture: pores, freckles, sweat, subtle imperfection. Clothing and armor
read as real materials — worn leather, fabric weave, scratched metal. Lighting behaves like
real light: bokeh backgrounds, lens flare, rim lighting from a physical source. Depth of field
is present and optically correct. The result sits in an uncanny sweet spot — clearly not a
photo, but rendered with enough physical accuracy that the fantasy elements feel grounded.

Two primary sub-moods:

- **Gritty / Dynamic:** Strong directional sunlight, physical grime and sweat on skin and
  costume, highly detailed gear with real wear, warm afternoon color grading. Energy is
  present — the character has been doing something. Used for racers, warriors, mechanics,
  action characters at rest.

- **Soft / Dreamy:** Overexposed, backlit, soft bokeh, drifting particles, pastel lens
  atmosphere. The character is emotionally inward — eyes closed or downcast, contemplative.
  Used for quiet moments, emotional beats, ethereal fantasy portraits.

Both sub-moods share the semi-photorealistic rendering foundation.

### Style Negatives
flat cel shading, retro analog grain, hard ink outlines, chibi proportions, heavy stylization, flat color fills, minimal shading, cartoon proportions, watercolor texture

### ChatGPT Translation

**Gritty sub-mood:**
```
Semi-realistic anime portrait — anime character design with highly detailed rendering quality.
Real skin texture with sweat and subtle imperfection, physically detailed material on worn
leather and gear, strong directional afternoon sunlight casting hard shadows, warm golden
color grading, shallow depth of field with soft bokeh background, cinematic realism, high
detail on clothing wear and surface grime, semi-realistic anime rendering with anime
stylization preserved in the face and proportions.
```

**Dreamy sub-mood:**
```
Semi-realistic anime portrait — anime character design with detailed soft rendering. Real
skin texture, soft freckles, subtle facial imperfection. Heavily backlit with overexposed
warm light, soft bokeh and drifting light particles, dreamy shallow depth of field, lens
flare and atmosphere haze, muted pastel color grading, emotionally inward pose, eyes
downcast or closed, quiet contemplative mood, semi-realistic anime rendering with anime
stylization preserved throughout.
```

### Niji Journey Translation

**Gritty sub-mood:**
```
semi-photorealistic anime, hyperreal rendering, physical material texture, sweat on skin, strong directional sunlight, warm afternoon color grade, shallow depth of field, soft bokeh
--ar 2:3
```

**Dreamy sub-mood:**
```
semi-photorealistic anime, hyperreal soft rendering, skin texture with freckles, dreamy backlit atmosphere, overexposed warm light, soft bokeh, floating particles, pastel lens haze
--ar 2:3
```

### Block Pre-fills (when loaded)

| Block | Value |
|---|---|
| Block 5 — Lighting | Physically accurate light source; directional sun (gritty) or backlit overexposed warm (dreamy); lens flare; bokeh-correct depth of field |
| Block 6 — Style | Semi-realistic anime; highly detailed anime character with stylization preserved in face and proportions; detailed material textures |
| Block 7 — Mood & Palette | Gritty: warm golden afternoon, high detail, worn surfaces. Dreamy: soft pastel overexposure, drifting particles, emotional stillness |

---

Output formats define *structure and layout*, not visual aesthetics. They are applied
alongside a visual style, not instead of one. When an output format is requested, load
its dedicated reference file and ask the user which visual style to pair with it.

---

## FORMAT: Character Sheet
**Aliases:** character sheet, ref sheet, refsheet, model sheet, turnaround sheet, character reference
**Pairs with:** any visual style — always ask which style to apply
**Reference file:** `references/character-sheet.md`

A production-quality anime character reference sheet covering up to 12 panels: full-body
turnaround, expression grid, hair breakdown, outfit breakdown, equipment sheet, weapon sheet,
color palette, action pose, scale reference, and silhouette panel. Designed to feel like a
professional game or anime studio production asset. Visual style is determined separately.

**When invoked:** load `references/character-sheet.md` for full layout spec, then ask:
> "Which visual style should the sheet use? (e.g., Ironbloom, Aquarelle, Ember — or describe
> your own)"

**Aspect ratio:** 16:9 (preferred) · 21:9 (large sheets)

---

## STYLE: Velvet
**Aliases:** velvet, luxury dark fantasy anime, crimson violet anime, Pixiv masterpiece, premium dark gacha, dark fantasy key visual, velvet luxury, satin anime
**Best for:** elegant dark-fantasy characters in luxury or supernatural settings, formal attire with lustrous materials, moody character portraits in crimson and violet lighting, premium dark gacha-style key visuals, characters who radiate dangerous elegance
**Conflicts with:** Daily Chibi, Moe Gacha, Webtoon, Botanical Lineart, Tactical Ink — too casual, flat, hand-drawn, or pastel; Kurosawa, Crewdson — live-action aesthetics that undercut the anime rendering base

### Visual Description
A premium dark-fantasy anime key visual defined by polished, layered rendering and a
signature crimson-violet palette. Unlike atmospheric styles that suppress detail into haze,
Velvet renders with lustrous precision: smooth gradient shadows, refined anime line art,
and glossy digital rendering that makes satin, velvet, and silk materials catch the light
with jewel-like quality.

Lighting is richly layered — soft bloom highlights, subtle rim lighting, and diffused
city-light bokeh working in concert to give the image depth without harshness. Eyes are
rendered with particular brilliance: luminous, detailed, immediately commanding. Character
design is elegant and composed — clean anime facial structure, sophisticated expression,
never casual or energetic.

The background is present through soft-focus depth of field: city lights, dark interiors,
or atmospheric environments rendered as bokeh and diffused glow rather than sharp detail
or abstracted haze.

The palette is non-negotiable: deep crimson and violet with atmospheric neon noir undertones.
Controlled contrast and sophisticated color harmony prevent the image from feeling garish
despite its richness. The result is a modern Pixiv masterpiece aesthetic — high-end dark
gacha key visual quality that feels like premium printed art.

### Style Negatives
flat cel shading, painterly texture, sketch lines, atmospheric suppression, lost-and-found edges, chibi proportions, dynamic action poses, casual aesthetic, pastel palette, muted desaturated colors, rough hand-drawn linework

### Usage Notes
- **Palette is fixed:** deep crimson and violet are the signature colors; don't swap for
  user-requested palettes — offer a different style if another palette is needed.
- **"Polished" means smooth gradients and refined lineart:** not cel shading, not painterly
  texture, not graphic flatness — smooth and glossy throughout.
- **Don't confuse with Gacha Splash:** Gacha Splash is dynamic, energetic, often semi-chibi;
  Velvet is still and elegant — portraits and composed scenes, not action shots.
- **Materials are a feature:** explicitly describe satin, velvet, silk, or other lustrous
  fabrics in the prompt when relevant — they define the style's surface quality.

### ChatGPT Translation
```
Cinematic anime key visual, premium Pixiv masterpiece quality, high-end dark-fantasy gacha
illustration. Polished soft-rendered anime shading with refined anime line art and smooth
gradient shadows. Glossy digital rendering on reflective satin and velvet materials.
Signature palette: deep crimson and violet lighting with atmospheric neon noir undertones,
sophisticated color harmony, controlled contrast. Richly layered lighting: soft bloom
highlights, subtle rim lighting, diffused city-light bokeh. Luminous eyes as primary focal
anchor — detailed, brilliant, immediately commanding. Elegant character design with clean
anime facial structure. Moody nighttime ambiance, ethereal cinematic atmosphere. Soft-focus
background with shallow depth of field — city lights or dark interior as diffused bokeh
rather than sharp detail. Highly detailed but stylized anime rendering — smooth shading
transitions, refined linework. No painterly texture. No lost-and-found edges. No atmospheric
suppression. No flat cel shading. No photorealistic surface detail.
```

### Niji Journey Translation
```
cinematic anime key visual, polished soft-rendered shading, refined line art, glossy digital rendering, satin velvet fabric, deep crimson violet palette, soft bloom highlights, rim lighting, city-light bokeh, luminous detailed eyes
--no painterly texture, sketch lines, flat cel shading, chibi, dynamic action pose
--ar 2:3
```

---

## STYLE: Daily Chibi
**Aliases:** daily chibi, chibi daily, cozy chibi, casual chibi, nichijou, slice chibi, SD daily life, everyday chibi, chibi slice of life, off-duty chibi
**Best for:** everyday slice-of-life scenes, characters eating or relaxing, restaurant/cafe/home interiors, mundane activities rendered with warmth, food scenes, off-duty character moments
**Conflicts with:** Moe Gacha (action-focused vs. static everyday), Dark Fantasy, Soulslike, Tactical Ink, Kurosawa — anything requiring dramatic atmosphere, action energy, or dynamic composition

### Visual Description
Semi-chibi proportions — head roughly one-quarter of total height, slightly enlarged but far
less extreme than full chibi. The character is always in a mundane, everyday context: eating
a meal, sitting at a desk, browsing a phone, standing in a convenience store. The scene around
them is the point — food, furniture, and everyday objects are rendered with genuine care and
visual weight. Clean flat cel shading with soft rounded forms. Warm ambient interior lighting
from a natural or overhead source. Expressions are typically understated: neutral, quietly
unamused, tired, or softly content. The appeal is the contrast between the slightly-oversized
anime head and the very grounded, believable world the character inhabits. Feels like a gacha
character's day off.

### Style Negatives
dramatic atmosphere, action energy, dynamic composition, dark fantasy, heavy shadows, bold thick outlines, complex detailed backgrounds, neon lighting, extreme chibi proportions, painterly rendering

### ChatGPT Translation
```
Anime semi-chibi slice-of-life illustration — slightly enlarged head with soft rounded anime
proportions, clean flat cel shading, character in a casual everyday pose surrounded by a
carefully rendered interior setting (restaurant, cafe, bedroom, kitchen), detailed everyday
objects — food dishes, tableware, furniture — given genuine visual weight, warm ambient
interior lighting, understated or quietly unamused expression, clean anime linework, cozy and
grounded mood, anime slice-of-life and gacha daily life aesthetic, 2D anime illustration style.
```

### Niji Journey Translation
```
semi-chibi anime, slightly oversized head, clean flat cel shading, slice of life interior, carefully rendered everyday objects, warm ambient lighting, clean anime linework
--ar 1:1
```

---

## STYLE: Gossamer
**Aliases:** gossamer, light novel, visual novel, visual novel cg, soft anime, pastel anime, soft fantasy, healing anime, iyashikei, fantasy portrait, shrine maiden, light novel illustration, porcelain anime
**Best for:** fantasy portraiture, visual novel CGs, light novel character illustrations, iyashikei and healing atmosphere scenes, elegant character showcases, spring or summer fantasy environments, floral scenes, tranquil interiors, fantasy fashion, elves, shrine maidens, noblewomen, romantic character art, serene magical settings
**Conflicts with:** Miura, Soulslike, Neon Noir, Ironbloom, Cinematic Anime, Hyperreal Anime, Kurosawa, Crewdson — anything dark, gritty, high-contrast, dramatic, or with strong directional lighting

### Visual Description
A clean flat modern anime aesthetic defined by minimal shading complexity and deliberate
color restraint. Line art is very thin and barely visible — soft grey or colored lines
rather than black ink, creating gentle form separation without hard edges. Shading is
flat cel-style with only one or two shadow tones, no gradients, no blending, and dark
values lifted so high the image reads nearly shadowless. Lighting is completely ambient
with no directional source — no cast shadows, no rim light, no highlight drama. Colors
are muted and slightly cool: sage greens, dusty blues, warm off-whites, and soft aquas
hold their saturation better than full pastels but avoid vibrancy. Backgrounds are
deliberately simplified — soft architectural suggestion, blurred foliage, washed-out
water — never detailed enough to compete with the figure. Hair reads as flat smooth
planes with a single controlled shine streak rather than strand-level rendering. Skin
is clean and textureless with a faint warm blush on cheeks only. Eyes are large and
flat-irised, rendered in cool aqua or grey-blue with no complex reflections. The overall
effect is quiet, weightless, and illustrative — closer to a clean Pixiv sketch with
intentional color holds than a fully rendered painting.

### Style Negatives
bold outlines, thick linework, black ink outlines, heavy shadows, dramatic lighting, directional light, rim lighting, gradients, painterly rendering, complex shading, vibrant saturated colors, dark palette, high contrast, photorealistic, detailed backgrounds

### ChatGPT Translation
```
Soft flat modern anime illustration — extremely thin soft-colored outlines barely visible
against form edges, flat cel shading with only one shadow tone and lifted dark values that
make the image read nearly shadowless, no gradients or blending on skin or fabric,
completely ambient lighting with no directional source or cast shadows, muted slightly
cool color palette where sage greens and dusty aquas hold mild saturation without going
fully pastel, simplified blurred background with no competing detail, hair as flat smooth
planes with a single shine streak and no strand detail, clean textureless skin with faint
blush on cheeks only, large flat-irised eyes in cool aqua or grey-blue. Drawn as a clean
flat light novel illustration — minimal, weightless, and illustrative. No painterly
rendering, no complex shading, no photorealism, 2D anime art style.
```

### Niji Journey Translation
```
soft flat anime, barely visible thin outlines, flat cel shading single shadow tone, no gradients, ambient lighting, muted cool palette sage green dusty aqua, blurred simplified background, light novel illustration
--ar 2:3
```

---

## STYLE: Flat Chibi
**Aliases:** flat chibi, chibi flat, graphic chibi, sticker chibi, pop chibi, flat gacha chibi, clean chibi
**Best for:** any chibi character in dynamic action regardless of genre — fantasy warriors, magical girls, school uniforms, sci-fi pilots, sports characters, mecha suits. Same genre freedom as Moe Gacha with flat cel rendering instead of warm painterly gradients. Palette fully user-defined.
**Conflicts with:** Moe Gacha (shares chibi proportions but Moe Gacha uses warm painterly rendering and atmospheric lighting), Gacha Splash, Ember, Makoto Shinkai, Hyperreal Anime, Cinematic Anime, Aquarelle, Velvet — anything requiring gradient rendering, atmospheric lighting, or painterly depth.

### Visual Description
Moe Gacha's full chibi proportions and action energy rendered through Flat Cel's technique. The head is one-third to one-half of total body height — the same extreme chibi scale — with a tiny capable body, oversized weapons or props, and detailed outfits or equipment across any genre. Everything renders flat: a single hard-edged shadow tone with lifted dark values, no gradients, no blending, no atmospheric glow or warm bloom. Line art is clean and thin with consistent weight. Outfits and armor have flat color fills with no metallic sheen or highlight drama. Weapons and props are oversized and bold but rendered as flat graphic blocks rather than detailed metallic rendering. Hair reads as flat smooth planes with a single shine streak. Particles and debris are simplified flat graphic shapes rather than atmospheric effects. Backgrounds are flat and minimal — never detailed, never competing. Lighting is completely ambient — no warm bloom, no rim light, no floating atmospheric particles. Palette is fully user-defined. The result feels like high-quality mobile game sticker art, a bold LINE character, or a flat graphic game icon — cute, readable, and graphically confident. Distinct from Moe Gacha (warm painterly rendering) and Daily Chibi (semi-chibi, static, slice-of-life).

### Style Negatives
gradients, blending, painterly texture, warm bloom, atmospheric particles, rim lighting, metallic sheen, highlight drama, detailed competing backgrounds, complex shadow rendering, photorealistic rendering, regular proportions

### Usage Notes
- Proportions from Moe Gacha, rendering from Flat Cel
- Unlike Moe Gacha: no warm bloom, no atmospheric particles, no painterly gradients — everything flat
- Unlike Daily Chibi: action-focused with dynamic poses, not slice-of-life; full chibi not semi-chibi
- Unlike Flat Cel: full chibi proportions only — not for regular-proportioned characters
- Palette fully user-defined per scene — specify in Block 7

### ChatGPT Translation
```
Flat cel chibi anime illustration — full chibi proportions with head one-third to one-half of total body height, single hard-edged shadow tone and lifted dark values reading nearly shadowless, no gradients or blending, flat color fills inside outfit and equipment with no metallic sheen or atmospheric glow, clean thin line art with consistent weight, oversized weapon or prop rendered as flat graphic block at chibi scale, detailed character outfit or equipment in flat style (any genre — fantasy armor, school uniform, sci-fi suit, magical costume), flat smooth hair planes with a single shine streak, simplified flat graphic debris and particle shapes, flat minimal background suited to scene setting, [user-defined palette and mood]. Drawn as a clean flat chibi anime illustration, 2D anime art style, no painterly texture, no complex shading, no atmospheric lighting.
```

### Niji Journey Translation
```
flat cel chibi anime, full chibi proportions, single shadow tone no gradients, flat color fills, clean thin line art, oversized weapon chibi scale, flat minimal background, [user-defined palette]
--ar [ratio]
```

---

## STYLE: Flat Cel
**Aliases:** flat cel, flat shading, flat anime, clean flat, cel flat, modern flat, flat illustration, flat style
**Best for:** any scene regardless of theme or genre — action, dark fantasy, romance, slice-of-life, comedy, horror, supernatural, school life, urban, sci-fi, fantasy. Palette and mood are fully user-defined per scene. Use when you want Gossamer's flat rendering without its palette or theme constraints.
**Conflicts with:** Aquarelle, Ember, Studio Ghibli, Makoto Shinkai, Hyperreal Anime, Cinematic Anime, Miura, Velvet — anything requiring gradients, painterly texture, volumetric lighting, complex shadow rendering, or photorealistic surface detail.

### Visual Description
The core technique of flat digital anime illustration, extracted from any specific mood or palette and made fully universal. Shading is flat cel-style with a single hard-edged shadow tone and lifted dark values that make the image read nearly shadowless. No gradients, no blending, no painterly texture, no brushstroke quality. Lighting is completely ambient — no directional source, no cast shadows, no rim light or highlight drama. Line art is clean and thin with consistent weight — slightly more defined than Gossamer's barely-visible style, providing readable form separation across all genres and palettes. Hair reads as flat smooth planes with a single shine streak. Skin is clean and textureless. Backgrounds are simplified and flat, never rendered with depth or complexity that competes with the figure. The palette is fully open and user-defined: vibrant, muted, warm, cool, dark, or light — whatever serves the scene. Dark themes are carried through palette choice rather than lighting — deep muted tones and desaturated color convey atmosphere without shadows. Gossamer is a specific application of this style (cool palette + iyashikei atmosphere); Flat Cel is the unrestricted base technique.

### Usage Notes
- **Palette:** fully user-defined — specify in Block 7 for every prompt. There is no default palette.
- **Mood:** fully user-defined — specify in Block 7 for every prompt.
- **Gossamer vs. Flat Cel:** If the user wants the muted cool palette and healing atmosphere, use Gossamer. If they want the flat technique with freedom to define palette and theme, use Flat Cel.
- **Dark themes:** handled through palette (deep muted tones, desaturated colors) — not through shadows or lighting drama.

### Style Negatives
gradients, blending, painterly texture, brushstroke quality, volumetric lighting, directional light, cast shadows, rim lighting, highlight drama, photorealistic rendering, complex shadow rendering, detailed competing backgrounds

### ChatGPT Translation
```
Flat cel anime illustration — clean thin line art with a single hard-edged shadow tone and lifted dark values reading nearly shadowless, no gradients or blending, completely ambient lighting with no directional source or cast shadows, simplified flat background, hair as smooth flat planes with a single shine streak, clean textureless skin, [user-defined palette and mood per scene]. Drawn as a clean flat modern anime illustration, 2D anime art style, no painterly texture, no complex shading, no photorealism.
```

### Niji Journey Translation
```
flat cel shading anime, single shadow tone no gradients, ambient lighting, clean thin line art, flat smooth hair, simplified flat background, [user-defined palette]
--ar [ratio]
```

---

## STYLE: Sketch Moe
**Aliases:** sketch moe, bold sketch, g-pen moe, rough moe, bold moe, minimal moe, pen moe, cute sketch
**Best for:** cute original characters, fantasy girls, market/shop scenes, character showcases with warm charm, any scene where bold readable outlines and minimal detail create a hand-crafted storybook warmth — proportions and palette fully user-defined
**Conflicts with:** Hyperreal Anime, Cinematic Anime, Miura, Velvet — anything requiring complex rendering, gradient shading, volumetric lighting, or high detail density. Also conflicts with Gossamer and Flat Cel — shares flat coloring but the bold linework and hand-drawn wobble are fundamentally different from their thin/clean line approaches

### Visual Description
Bold, confident outlines reminiscent of traditional G-pen manga inking — the lines carry
the illustration. Weight varies naturally with pressure, thicker on outer contours and
thinner on interior details. A subtle hand-drawn wobble and texture gives the linework
warmth and imperfection without sacrificing clarity. The character is constructed with
only the minimum necessary lines — silhouette readability is prioritized over decorative
detail. Information density is deliberately low. Coloring is soft flat fills with muted
saturation and only very subtle shading — no heavy gradients, no painterly rendering, no
dramatic lighting. Proportions are semi-deformed: the head is slightly enlarged but not
chibi-extreme, the body is slender and elegant with slightly longer limbs, creating a
delicate youthful silhouette that avoids both mascot-like stockiness and normal realism.
Facial features are positioned slightly lower on the face for maximum cuteness — small
chin, short mid-face, tiny simple mouth, nearly omitted nose. Backgrounds are simplified
and softened so the character's silhouette and expression remain the clear focus. The
overall effect is a warm, hand-crafted illustration that feels like premium doujinshi
cover art or a high-quality Pixiv rough-with-flats piece.

### Style Negatives
photorealistic, heavy gradients, painterly rendering, complex shading, volumetric lighting, dramatic shadows, thin invisible outlines, excessive detail, intricate decorations, realistic proportions, stocky or muscular build, extreme chibi proportions, oversized head mascot proportions

### Usage Notes
- **Proportions:** semi-deformed by default (slightly enlarged head, slim elegant body). Can be pushed toward more chibi or more normal per user request, but the sweet spot is between the two.
- **Palette:** fully user-defined — specify in Block 7. No default palette.
- **Linework is the identity:** if the user wants thin or invisible outlines, redirect to Gossamer or Flat Cel instead.

### ChatGPT Translation
```
Anime illustration with bold G-pen-style outlines — confident thick-to-thin linework with
natural pressure variation and subtle hand-drawn wobble giving warmth and texture, character
constructed with minimum necessary lines prioritizing silhouette readability over decorative
detail, soft flat color fills with muted saturation and only very subtle shading, no heavy
gradients or painterly rendering, semi-deformed proportions with slightly enlarged head and
slender elegant body with delicate elongated limbs, facial features positioned low on the
face for cuteness — small chin tiny mouth nearly omitted nose, simplified softened background
keeping character as clear focus, [user-defined palette and mood per scene], warm hand-crafted
illustration quality, 2D anime art style.
```

### Niji Journey Translation
```
bold G-pen outlines thick-to-thin linework, hand-drawn wobble, soft flat color fills muted saturation, semi-deformed proportions slender elegant body, simplified soft background, [user-defined palette]
--ar [ratio]
```

---

## ADD YOUR OWN STYLE

Copy this template and fill it in:

```
## STYLE: [Name]
**Aliases:** [name], [alias 1], [alias 2]
**Best for:** [subject types this suits]
**Conflicts with:** [things to avoid]

### Visual Description
[2–4 sentences describing the look, feel, and key visual codes of this style]

### Style Negatives
[Comma-separated list of things that break this style. These get auto-appended to the
negative prompt / --no flag when this style is loaded. Focus on rendering approaches,
shading methods, proportion types, and aesthetic clashes — not subject matter.]

### ChatGPT Translation
[Prose language to weave into the ChatGPT prompt — 1–3 sentences]

### Niji Journey Translation
[Keyword-dense form + any recommendation]
```

---

## STYLE: Pixiv Clean
**Aliases:** pixiv clean, pixiv, clean anime, clean illustration, elf portrait, pixiv portrait, pixiv oc
**Best for:** original character portraits, elf and fantasy OCs, sitting or relaxed poses, character showcases, any scene where fabric detail and clean faces are the focus — white background or with a scene background
**Conflicts with:** heavily rendered styles, painterly backgrounds, complex lighting setups, Hyperreal Anime, Cinematic Anime, Aquarelle, Velvet — anything requiring atmospheric depth or photorealistic rendering

### Visual Description
A clean, polished Pixiv illustration style defined by confident medium-weight linework and a
deliberate contrast between face rendering and fabric rendering. Lines taper naturally at hair
tips and fabric edges but never disappear. Shading is soft cel-style with one or two flat
shadow passes — skin is smooth and luminous without crossing into photorealism. The defining
characteristic is fabric: cloth folds use loose, gestural inner lines that feel almost
hand-drawn, giving ruffles and layered clothing a lively quality that contrasts the cleaner
face and skin. Background is user-defined — white is common but a simplified scene background
works equally well. Lighting is soft ambient with no directional source. Face is always the
most refined element. Palette is fully user-defined.

### Style Negatives
painterly backgrounds, complex lighting setups, atmospheric depth, photorealistic rendering, heavy gradients, volumetric lighting, dramatic shadows, rough sketch linework, chibi proportions

### ChatGPT Translation
```
Clean Pixiv anime illustration — confident medium-weight linework with natural taper at hair
tips and fabric edges, soft cel shading with one or two flat shadow passes on skin, smooth
luminous skin rendering that stays firmly 2D, loose gestural cloth fold lines on fabric and
ruffles contrasting the cleaner face rendering, soft ambient lighting with no directional
source or cast shadows, face as the most refined focal element, background and palette fully
user-defined. Drawn as a clean polished Pixiv character illustration — 2D anime art style,
no painterly texture, no photorealism, no complex lighting.
```

### Niji Journey Translation
```
clean Pixiv anime illustration, confident medium-weight linework, soft flat cel shading, smooth luminous skin, loose gestural fabric fold lines, ambient lighting, [user-defined palette]
--ar [ratio]
```

---

## STYLE: Colored Pencil
**Aliases:** colored pencil, colour pencil, pencil art, colored pencil anime, traditional pencil
**Best for:** character portraits, OC showcases, detailed costume and equipment studies, fan art, any subject where a handcrafted traditional-media feel is the point
**Conflicts with:** digital polish, clean cel shading, flat rendering, neon lighting, glossy or luminous skin, photorealistic rendering

### Visual Description
Traditional colored pencil illustration on white or off-white paper. Anime character
proportions and structure rendered entirely through colored pencil — visible directional
strokes, crosshatching for shadows, and layered color buildup define form instead of ink
outlines. Edge definition comes from darker pencil tones and stroke density rather than
clean linework. Paper tooth texture shows through everywhere, especially in lighter areas.
White paper itself serves as the highlight — untouched paper, not painted white. Colors
have the slightly muted, waxy quality inherent to colored pencil media. Palette is
user-defined but always reads as traditional colored pencil.

### Style Negatives
digital rendering, clean ink outlines, flat cel shading, glossy or luminous skin, neon lighting, gradient backgrounds, painterly blending, airbrush smoothness, photorealistic rendering, vector linework, chibi proportions

### ChatGPT Translation
```
Traditional colored pencil anime illustration on white paper — all form defined by visible
colored pencil strokes rather than ink outlines, directional hatching and crosshatching for
shadows, layered color buildup with waxy pencil texture, paper tooth visible throughout
especially in light areas, white paper left untouched as highlights, edge definition through
darker pencil pressure and stroke density not clean lines, slightly muted traditional media
color quality. Drawn entirely as a colored pencil illustration on paper — 2D anime
proportions, no digital rendering, no ink outlines, no airbrush smoothness.
```

### Niji Journey Translation
```
traditional colored pencil anime illustration, visible pencil strokes, crosshatch shading, layered color on white paper, paper texture, waxy colored pencil quality, [user-defined palette]
--ar [ratio]
```
