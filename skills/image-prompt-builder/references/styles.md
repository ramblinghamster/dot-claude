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

## STYLE: Kurosawa
**Aliases:** kurosawa, kuro, akira k, japanese cinema
**Best for:** lone figures, dramatic landscapes, samurai, feudal Japan, moral weight
**Conflicts with:** bright/cheerful palettes, comedic tone, hyperrealistic product shots

### Visual Description
Inspired by Akira Kurosawa's cinematography — high-contrast black-and-white or desaturated
near-monochrome compositions. Dramatic use of negative space, weather as emotional atmosphere
(rain, wind, fog), and characters that feel isolated against vast or oppressive environments.
Shots are wide and deliberate. Stillness conveys weight. Film grain is present.

### Usage Notes
- **For anime rendering:** Kurosawa alone pulls toward live-action film photography. To
  render in anime/manga style, use Kurosawa as the **composition and mood reference only**
  and anchor the rendering with *Vagabond* or *Dororo* as the illustration reference.
  Add these terms to the prompt: `ink wash illustration`, `bold brushstroke outlines`,
  `manga linework`, `screen tone shading`. Remove any reference to film grain.
- **Stacking:** When stacking with Hyperreal Anime, lead with Hyperreal Anime as the
  rendering base and use Kurosawa for composition, framing, and mood descriptors only.

### ChatGPT Translation
```
Kurosawa-inspired anime illustration — near-monochrome palette of deep blacks and cool grays,
dramatic high-contrast composition, ink wash rendering with bold brushstroke outlines and manga linework, deliberate stillness, weather as
emotional texture, wide establishing framing, profound sense of solitude and moral gravity,
2D anime art style.
```

### Niji Journey Translation
```
Kurosawa cinematic anime illustration, near-monochrome desaturated palette, dramatic ink wash atmosphere,
high contrast shadows, 35mm film grain, deliberate stillness, theatrical composition,
Japanese feudal aesthetic
```

---

## STYLE: Crewdson
**Aliases:** crewdson, gregory crewdson, staged, suburban surreal
**Best for:** interior scenes, portraiture, emotionally loaded stillness, suburban or coastal settings
**Conflicts with:** action scenes, fantasy environments, bright comedic tone

### Visual Description
Large-format staged photography aesthetic — images that feel like stills from a film that
doesn't exist. Hyper-real yet constructed, every element in the frame deliberately placed
as though by a set designer. Single dominant light source, often from a window or doorway,
casting raking shadows. Desaturated midtones with warm amber highlights and deep teal
shadows. The subject is always in the middle of something private, emotionally ambiguous,
and slightly melancholic. No direct eye contact.

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
cinematic staged large-format aesthetic, theatrically composed, every element deliberately
placed as though by a set designer, still from a film that does not exist, desaturated
midtones, warm amber and deep teal palette, single raking window light, long dramatic
shadows, emotionally loaded stillness, soft painterly anime illustration, no direct eye contact
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
blacks and intense color. Inspired by Blade Runner, Ghost in the Shell, and classic noir.

### Usage Notes
- **For anime rendering:** Neon Noir alone pulls toward photorealistic/live-action feel.
  To render in anime style, stack Hyperreal Anime as the base rendering layer and apply
  Neon Noir conditions on top. Also add a specific anime title anchor to lock the rendering
  language: *Ghost in the Shell: Stand Alone Complex* and/or *Cyberpunk Edgerunners* are
  the strongest fits for this style's urban night aesthetic.
- **Stacking:** Lead prompt with Hyperreal Anime rendering language, then add Neon Noir
  atmosphere conditions (neon color palette, wet reflections, anamorphic flare, etc.).

### ChatGPT Translation
```
Neon noir anime illustration — rain-slicked urban streets reflecting electric neon light in
magenta, cyan, and amber, deep shadow contrast, smoke and steam rising from vents, cinematic
wide shot, figures silhouetted or half-lit, Blade Runner atmosphere, mysterious and predatory
mood, wet surface reflections, anamorphic lens flare, desaturated except for neon color pops,
clean anime linework, 2D anime art style.
```

### Niji Journey Translation
```
neon noir anime illustration, rain-slicked cyberpunk city night, electric magenta and cyan neon reflections,
deep shadows, steam vents, silhouetted figure, clean anime linework, Blade Runner atmosphere, anamorphic lens flare,
wet street puddle reflections, mysterious mood, high contrast
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
space is used deliberately. Feels like a Vogue or Patek Philippe spread — elevated, restrained,
and aspirational.

### ChatGPT Translation
```
High-end editorial fashion anime illustration — clean and minimal composition, precise
directional softbox lighting, crisp highlights with soft shadow falloff, desaturated and
cool color palette with lifted blacks, generous negative space, aspirational and restrained
mood, Vogue editorial quality, ultra high detail, 2D anime art style.
```

### Niji Journey Translation
```
luxury editorial fashion anime illustration, minimal composition, precise soft directional lighting,
desaturated cool palette, lifted blacks, crisp highlights, negative space, aspirational mood,
Vogue magazine aesthetic, clean illustration, high detail
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

### ChatGPT Translation
```
Studio Ghibli-inspired aesthetic — warm, painterly illustration with handcrafted texture,
soft dappled natural lighting, lush detailed environments, wistful and wonder-filled mood,
emotionally gentle atmosphere, rich saturated warm greens and golden yellows, expressive
character design, Hayao Miyazaki visual language.
```

### Niji Journey Translation
```
Studio Ghibli style, Miyazaki aesthetic, soft painterly illustration, warm dappled natural
lighting, lush environment, wistful wonder-filled mood, rich saturated warm palette,
golden yellows and soft blues, handcrafted texture, expressive character
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
Characters feel mythic in scale. The world has weight and danger. Inspired by Dark Souls,
Witcher, and Zdzisław Beksiński.

### ChatGPT Translation
```
Dark fantasy anime illustration — brooding and atmospheric, deep jewel tones of emerald and
crimson against near-black backgrounds, dramatic volumetric rim lighting, heavy fog and smoke,
gothic architectural ruins, crumbling stone and iron, mythic character scale, dangerous and
ancient world, Souls-like visual weight, painterly cinematic anime art style, expressive anime linework.
```

### Niji Journey Translation
```
dark fantasy anime illustration, brooding atmosphere, deep jewel tones emerald crimson obsidian,
volumetric rim lighting, heavy fog and smoke, gothic ruins crumbling stone, mythic scale,
dangerous ancient world, Dark Souls aesthetic, dramatic shadow contrast, expressive anime linework
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
semi-painterly anime, matte finish, soft diffuse shading, cinematic warm lighting, gentle
amber rim light, luminous lantern glow, soft cel shading, thin elegant lineart, hand-painted
anime texture, subtle bloom, warm midtones, softly illuminated faces, dark fantasy anime
aesthetic, inviting warmth, smoky ambience, visual novel illustration style, painterly depth
```

---

## STYLE: Prism
**Aliases:** prism, crystal, holographic, glitter, refracted light, rainbow crystal
**Best for:** fantasy portraits, ethereal characters, luxury product shots, cyber-fantasy, surreal close-ups, jewelry and crystal subjects
**Conflicts with:** minimalist/clean aesthetics, matte finishes, dark moody realism, Kurosawa, Crewdson

### Visual Description
A hyper-detailed, surreal luxury aesthetic built around refracted light and crystal surfaces.
Rainbow prism reflections scatter across the subject from faceted glass or gemstone elements.
Glitter particles and holographic highlights float in the frame. Skin is luminous, colors are
vibrant and saturated, and the background is dark and moody to maximize contrast with the
glowing light effects. Neon and holographic lighting create a dreamy cyber-fantasy atmosphere.
Every surface catches and refracts light — glossy, translucent, jewel-like. The mood is
surreal, glamorous, and visually overwhelming in a controlled way.

### ChatGPT Translation
```
2D anime illustration, clean precise anime linework, digital anime painting, smooth color
gradients, stylized anime character design — surreal luxury cyber-fantasy aesthetic with
rainbow prism reflections scattered across the character, faceted jewel-like crystal surfaces,
holographic shimmer, glitter highlights, vibrant saturated colors, cinematic neon lighting,
dark moody background with glowing rainbow bokeh, detailed crystal light effects, clean smooth
rendering, no texture noise, dreamy and visually opulent mood.
```

### Niji Journey Translation
```
clean precise anime linework, crystal prism reflections, rainbow refracted light scattered
across face, faceted jewel-like glossy surfaces, holographic highlights, glitter particles,
vibrant saturated colors, cinematic neon lighting, hyper-detailed reflections, dark moody
background, glowing rainbow bokeh, dreamy cyber-fantasy aesthetic, surreal luxury vibe,
refracted light effects, ultra sharp focus, anime illustration masterpiece, insanely detailed
```

---

## STYLE: Aquarelle
**Aliases:** aquarelle, watercolor anime, soft wash, washi, analog anime, quiet anime, gouache
**Best for:** original character portraits, full-body illustrations, emotionally subtle scenes, understated fantasy, slice-of-life, travel or nature themes
**Conflicts with:** Prism, Neon Noir, Dark Fantasy, dramatic cinematic lighting, glossy/polished aesthetics, sci-fi or magical effects

### Visual Description
A delicate, hand-painted watercolor anime aesthetic that prioritizes restraint, atmosphere,
and emotional presence over visual complexity. Characters feel unique and slightly
unconventional — deliberately avoiding generic moe or gacha-idol beauty. Slightly low
proportions: larger head, compact torso, fragile silhouette, but not chibi. Soft desaturated
colors, gentle natural lighting, and generous negative space keep the character as a clear
focal point surrounded by breathing room. The rendering feels analog despite being digital —
slightly rough linework, faint paper texture, subtle paint unevenness, soft watercolor or
gouache-like edges, and organic imperfections. No sterile vector lineart, no over-polishing,
no dense detail. High quality through restraint, not complexity.

### ChatGPT Translation
```
Delicate watercolor-inspired anime illustration with a hand-painted analog feel — soft
desaturated colors, gentle natural lighting, and generous negative space surrounding the
character. Slightly unconventional character design with a small fragile build and one
memorable visual quirk, deliberately avoiding generic moe or gacha aesthetics. Simple,
tasteful clothing with silhouette-focused design. Rendering feels like a physical watercolor
or gouache painting: slightly rough linework, faint paper texture, subtle paint unevenness,
soft edges, organic imperfections. Minimal softly-blended background using large atmospheric
shapes. Refined but not over-rendered — warmth, atmosphere, and emotional presence over
detail density.
```

### Niji Journey Translation
```
watercolor anime illustration, hand-painted analog feel, soft desaturated colors, gentle
natural lighting, generous negative space, unique unconventional character design, small
delicate build, slightly low proportions, one memorable design quirk, simple tasteful
clothing, silhouette clarity, minimal softly blended background, large atmospheric shapes,
slightly rough linework, faint paper texture, subtle paint unevenness, soft watercolor edges,
organic imperfections, gouache softness, refined not over-rendered, emotional warmth,
no moe no gacha no glossy finish
```

### Negative (apply to Niji Journey with --no flag)
```
--no generic anime face, sameface, gacha face, idol beauty, adult proportions, super chibi,
over-detailed hair, glossy plastic texture, overly smooth digital finish, hard vector lineart,
oversaturated colors, harsh contrast, excessive decoration, dense rendering, busy background,
dramatic cinematic lighting, magical effects, sci-fi elements, floating decorative objects
```

---

## STYLE: Ironbloom
**Aliases:** ironbloom, iron bloom, tactical anime, arms girl, gear girl, mech contrast
**Best for:** characters with complex armor, mechanical suits, military/tactical gear, fantasy plate armor, sci-fi equipment, steampunk machinery, any scene contrasting a soft anime character with hard technical detail
**Conflicts with:** Aquarelle, Ghibli, soft painterly styles, lush detailed backgrounds, warm intimate interiors

### Visual Description
The defining tension of this style is a soft anime character face and fragile human presence set against hyper-detailed, technically precise mechanical or structural complexity — armor, gear, weapons, equipment, machinery. The rendering is clean bold manga lineart with semi-flat shading, earth and neutral tones (sand, khaki, olive, dark brown), and a white or near-white negative space background that isolates the subject. Equipment is rendered with almost technical-illustration precision — every buckle, panel, joint, and surface detail present and readable. The anime character within or beneath the gear remains soft, expressive, and emotionally present. Often carries a thematic juxtaposition: something delicate (a flower, a small creature, a gentle gesture) against something formidable. The contrast is the point.

### ChatGPT Translation
```
Clean bold manga lineart with semi-flat shading and hyper-detailed technical rendering of
complex armor or equipment. Muted earth tone palette of sand, khaki, olive, and dark brown.
White or near-white negative space background isolating the subject. Soft expressive anime
character face contrasted with precisely rendered mechanical or structural complexity — every
panel, joint, and surface detail present. Emotionally resonant thematic contrast between
something formidable and something delicate. Technical illustration precision, manga quality.
```

### Niji Journey Translation
```
clean bold manga lineart, hyper-detailed armor and equipment, technical illustration
precision, semi-flat shading, muted earth tones sand khaki olive dark brown, white negative
space background, soft expressive anime character face, hard mechanical contrast, every panel
and joint detailed, thematic juxtaposition of strength and delicacy, manga illustration
masterpiece
```

---

## STYLE: Makoto Shinkai
**Aliases:** makoto shinkai, shinkai, your name, weathering with you, luminous sky, shinkai sky
**Best for:** emotional outdoor scenes, dramatic skies, distance and longing, cityscapes at golden hour, two characters separated by space or light
**Conflicts with:** interior-only scenes, Kurosawa monochrome, flat design, Borderlands cel shading

### Visual Description
Inspired by Makoto Shinkai's films — hyper-detailed atmospheric skies with layered clouds,
lens flares, and luminous volumetric light rays that feel almost tactile. Colors are intensely
saturated but natural: deep blues, burning ambers, electric golds. Backgrounds are rendered
with near-photographic detail while characters retain clean anime stylization, creating a
dreamlike contrast. Emotional depth comes from light — the way it falls on a face, refracts
through rain, or floods a train window. A pervasive sense of distance, longing, and beauty
in transience.

### ChatGPT Translation
```
Makoto Shinkai anime illustration — hyper-detailed atmospheric sky with layered clouds and
luminous volumetric light rays, lens flare, intensely saturated natural colors in deep blues
and burning amber gold, richly detailed background contrasting with clean anime character
stylization, emotional depth through light and distance, dreamlike beauty, sense of longing
and transience, cinematic anime composition.
```

### Niji Journey Translation
```
Makoto Shinkai style, hyper-detailed atmospheric sky, luminous volumetric light rays,
lens flare, layered dramatic clouds, intensely saturated natural palette deep blue amber gold,
hyper-detailed painterly background, clean anime characters, emotional cinematic depth,
dreamlike luminosity, sense of longing and distance, your name aesthetic
```

---

## STYLE: Ufotable
**Aliases:** ufotable, demon slayer, fate zero, fate stay night, ufotable dark fantasy, kimetsu
**Best for:** action sequences, dark fantasy combat, supernatural scenes, dramatic character moments, high-production anime key visuals
**Conflicts with:** Aquarelle, Kurosawa monochrome, flat design, retro anime

### Visual Description
The signature visual language of Ufotable studio — the team behind Demon Slayer and Fate/Zero.
High-contrast dramatic lighting with richly saturated jewel-toned colors: deep crimson, electric
blue, vivid gold against near-black shadows. Cinematic polish with fluid motion energy even in
still images. Characters are rendered with meticulous detail and glowing intensity — effects
like fire, water, and supernatural energy are rendered as breathtaking visual spectacles. The
overall feel is expensive, dramatic, and technically flawless. Dark settings are elevated by
explosive color rather than muted.

### ChatGPT Translation
```
Ufotable animation studio aesthetic — high-contrast dramatic lighting, richly saturated jewel
tones of deep crimson, electric blue, and vivid gold against near-black shadows, cinematic
production polish, meticulous character detail with glowing intensity, supernatural energy
effects rendered as visual spectacle, fluid motion energy, expensive and technically flawless
dark fantasy anime quality, Demon Slayer and Fate/Zero visual language.
```

### Niji Journey Translation
```
Ufotable studio style, high contrast dramatic lighting, richly saturated jewel tones,
deep crimson electric blue vivid gold, near-black shadows, cinematic anime polish,
meticulous character detail, glowing intensity, supernatural energy effects, fluid motion,
dark fantasy anime key visual, Demon Slayer aesthetic, production quality masterpiece
```

---

## STYLE: Retro Anime
**Aliases:** retro anime, 80s anime, 90s anime, akira aesthetic, vhs anime, old school anime, analog anime, slayers, city hunter
**Best for:** nostalgic scenes, action and drama, urban or sci-fi settings, character-driven moments, any scene benefiting from analog warmth and grain
**Conflicts with:** Prism, Ufotable, clean modern anime aesthetics, hyperrealistic rendering

### Visual Description
The visual language of 1980s–90s anime — Akira, Ghost in the Shell, Slayers, City Hunter,
Cowboy Bebop. Analog warmth with visible film grain and subtle color bleed at edges. Linework
is slightly thicker and less precise than modern anime, with a hand-drawn quality that feels
intentional and characterful. Color palette has a distinctive muted warmth — faded yellows,
dusty blues, warm oranges — as if slightly sun-bleached or viewed through a VHS lens. Cel
animation textures, limited color banding, and the occasional halftone dot pattern. Emotionally
direct and kinetic.

### ChatGPT Translation
```
Retro 1980s–90s anime aesthetic — analog film grain, subtle VHS color bleed at edges,
slightly thick hand-drawn linework, muted warm palette of faded yellows, dusty blues, and
warm oranges, cel animation texture, limited color banding, emotionally direct and kinetic
energy, Akira and Ghost in the Shell visual language, nostalgic analog warmth, hand-crafted
imperfection over digital polish.
```

### Niji Journey Translation
```
retro 80s 90s anime aesthetic, analog film grain, VHS warmth, color bleed edges,
thick hand-drawn linework, muted warm palette faded yellows dusty blues warm oranges,
cel animation texture, limited color banding, Akira aesthetic, Ghost in the Shell style,
nostalgic analog feel, hand-crafted imperfection, old school anime energy
```

---

## STYLE: Cel Shading
**Aliases:** cel shading, borderlands, cel shaded, bold outline, graphic anime, borderlands style, comic shading, toon shading
**Best for:** action scenes, graphic novels, high-energy characters, poster compositions, any scene where bold graphic impact matters more than realism
**Conflicts with:** Aquarelle, Crewdson, Makoto Shinkai, any painterly or atmospheric style

### Visual Description
Bold black outlines, flat color fills, and high-contrast shading with no gradients — the
visual language of Borderlands, comic books, and graphic novel illustration. Colors are
vivid and fully saturated. Shading is binary: lit or shadow, with a hard edge between them.
Linework is thick, confident, and expressive. The overall effect is graphic, energetic, and
immediately readable. Depth comes from composition and color contrast rather than rendering
subtlety. Feels designed to be seen from a distance and understood instantly.

### ChatGPT Translation
```
2D anime cel shading illustration — bold black outlines, flat fully-saturated color fills,
high-contrast binary shading with hard edges between light and shadow, no gradients,
thick confident expressive linework, vivid color palette, graphic novel and Borderlands
visual language, energetic and immediately readable, depth through composition and color
contrast rather than rendering subtlety.
```

### Niji Journey Translation
```
anime cel shading style, bold black outlines, flat color fills, high contrast binary shading,
no gradients, thick expressive linework, vivid saturated colors, graphic novel aesthetic,
Borderlands art style, toon shading, energetic graphic impact, comic book illustration
```

---

## STYLE: Soulslike
**Aliases:** soulslike, bloodborne, elden ring, dark souls, fromsoft, souls aesthetic, gothic horror fantasy
**Best for:** gothic architecture, horror fantasy, fog-shrouded landscapes, cursed or corrupted characters, bleak and grand environments, ancient decaying worlds
**Conflicts with:** Ember, Ghibli, Makoto Shinkai, warm or inviting aesthetics

### Visual Description
Inspired by FromSoftware's Bloodborne, Dark Souls, and Elden Ring concept art — a
desaturated, fog-heavy gothic aesthetic where grandeur and dread occupy the same space.
Color palette is predominantly grey, ash, and muted teal with isolated accents of deep
amber or bloodred. Architecture is massive, decaying, and inhuman in scale. Characters
are dwarfed by their environments. Fog, ash particles, and atmospheric haze obscure
backgrounds, creating mystery and weight. Unlike Dark Fantasy (which uses jewel tones
and epic warmth), Soulslike is bleaker, quieter, and more unsettling — beauty that comes
from ruin.

### ChatGPT Translation
```
FromSoftware Soulslike anime illustration — desaturated gothic atmosphere in grey, ash, and
muted teal with isolated accents of deep amber or bloodred, massive decaying architecture
that dwarfs human scale, fog and ash particles obscuring the background, a pervasive sense
of ancient ruin and quiet dread, grandeur and horror coexisting, bleaker and more unsettling
than traditional dark fantasy, Bloodborne and Elden Ring visual language, 2D anime art style, detailed anime linework.
```

### Niji Journey Translation
```
soulslike gothic anime illustration, desaturated palette grey ash muted teal deep amber accents,
massive decaying architecture, human figures dwarfed by environment, atmospheric fog and
ash particles, ancient ruin and quiet dread, grandeur and horror, bleak beauty,
Bloodborne concept art style, Elden Ring atmosphere, FromSoftware visual language, detailed anime linework
```

---

## STYLE: Miura
**Aliases:** miura, berserk, kentaro miura, dark manga, crosshatch, berserk manga
**Best for:** intense character portraits, brutal battle scenes, dark fantasy figures, deeply detailed armor and weapons, monochromatic or limited-color dramatic compositions
**Conflicts with:** Ghibli, Aquarelle, Ember, soft or colorful styles

### Visual Description
Inspired by Kentaro Miura's Berserk — one of the most technically demanding manga art styles
ever produced. Dense, precise crosshatching builds shadow and texture in ways that feel almost
engraved. Linework is extraordinarily detailed, with heavy blacks that create dramatic contrast.
Armor, weapons, and environmental detail are rendered with obsessive specificity — every rivet,
scratch, and surface texture accounted for. Figures feel massive and heavy. The overall
aesthetic is monochromatic or near-monochromatic, with shadow doing the emotional and
atmospheric work. Brutal, meticulous, and awe-inspiring.

### ChatGPT Translation
```
Kentaro Miura's Berserk manga aesthetic — dense precise crosshatching building shadow and
texture with engraving-like depth, extraordinarily detailed linework, heavy blacks creating
dramatic contrast, obsessively detailed armor and weapons with every rivet and scratch
rendered, massive and heavy figure weight, monochromatic or near-monochromatic palette with
shadow doing the emotional work, brutal meticulous and awe-inspiring dark manga quality.
```

### Niji Journey Translation
```
Berserk manga style, Kentaro Miura aesthetic, dense crosshatching, heavy black ink shadows,
extraordinarily detailed linework, obsessively detailed armor and weapons, every surface
texture rendered, massive figure weight, dramatic contrast, near-monochromatic dark manga,
brutal and meticulous detail, dark fantasy manga masterpiece
```

---

## STYLE: Botanical Lineart
**Aliases:** botanical lineart, botanical, clean manga portrait, garden portrait, floral lineart
**Best for:** elf and fae characters, soft fantasy portraits, characters in garden or nature settings, character-plant compositions, any portrait where a clean elegant character contrasts with organic botanical detail
**Conflicts with:** dark or gritty themes, heavy backgrounds, action sequences, Neon Noir, Soulslike, Miura

### Visual Description
Clean digital manga lineart with precise, confident strokes and semi-flat cel shading — no
gradients, no painterly texture. Color palette is deliberately restrained: muted earth tones,
warm naturals, and soft skin against a near-white or white background. Botanical elements
(flowers, vines, leaves) are rendered with loose organic detail and used compositionally to
frame or interact with the character. The contrast is between the precision of the character
and the casual looseness of the surrounding flora. Mood is serene and quietly elegant — not
epic, not melancholy, just present.

### ChatGPT Translation
```
Clean digital manga aesthetic — precise confident lineart with semi-flat cel shading, no
gradients, muted restrained color palette of warm naturals and soft earth tones against a
white or near-white background, botanical elements (flowers, leaves, vines) rendered with
loose organic detail framing the character, serene and quietly elegant mood, the contrast
between precise character rendering and casual organic flora as the compositional anchor.
```

### Niji Journey Translation
```
clean digital manga lineart, semi-flat cel shading, precise confident lines, muted warm
natural palette, white background, botanical framing elements, white flowers loose leaves,
soft fantasy character, serene elegant mood, restrained color, organic flora composition,
no gradients, no heavy backgrounds --ar 2:3
```

---

## STYLE: JRPG Pixel Art
**Aliases:** jrpg pixel art, pixel art, pixel sprite, hd pixel, octopath, jrpg sprite, modern pixel art
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
JRPG sprite work — Octopath Traveler, high-end mobile RPG character art, or premium gacha
game sprites.

### ChatGPT Translation
```
High-resolution modern JRPG pixel art aesthetic — fine pixel grid with anime-influenced
character design, large expressive eyes, flowing styled hair rendered in pixel form, detailed
fantasy armor and equipment with rich full-color pixel shading, careful dithering to simulate
metallic volume and jewel tones, warm skin tones against a near-white or transparent
background, Octopath Traveler and premium mobile RPG sprite visual language, every pixel
intentional and expressive.
```

### Niji Journey Translation
```
high resolution JRPG pixel art sprite, anime character design, fine pixel grid, detailed
fantasy equipment, full color palette, dithered metallic shading, jewel tone accents,
warm skin tones, near-white background, Octopath Traveler style, modern mobile RPG sprite,
premium gacha character art --ar 2:3
```

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
modern shounen anime aesthetic, warm sepia environment aged paper tones cream yellow-brown,
crisp cold sharp supernatural energy contrast, high detail environmental destruction rubble
cracked walls scattered debris, clean character rendering fuller color contrast, clean anime linework,
volumetric backlit window light atmospheric haze, determined mid-action character pose,
warm decay vs cold power visual tension, A Certain Scientific Railgun style --ar 2:3
```

---

## STYLE: Moe Gacha
**Aliases:** moe gacha, gacha, chibi gacha, cute chibi, fantasy chibi, chibi knight, chibi warrior, gacha chibi
**Best for:** fantasy characters in dynamic action, chibi knight and warrior designs, cute-but-capable characters mid-motion, any scene where full chibi proportions and warm cinematic energy combine
**Conflicts with:** Miura, Soulslike, Kurosawa, Liminal Horror, any dark gritty or restrained aesthetic

### Visual Description
The full chibi action art aesthetic of fantasy gacha games — characters rendered at extreme
chibi proportions where the head is roughly one-third to one-half of total body height,
creating a tiny-but-capable figure that feels both adorable and powerful. Linework is clean
and precise with subtle weight variation. Cel shading is crisp and flat rather than painterly
— smooth color transitions, clean shadow edges, no heavy gradients. Detailed fantasy plate
armor with gold trim and decorative motifs is rendered with care despite the chibi scale.
Weapons are oversized relative to the character, which reads as charming rather than absurd
at chibi proportions. Hair is flowing and wind-swept with good strand separation. Poses are
dynamic — low-angle action shots, mid-charge, debris and particles in motion. Lighting is
warm and atmospheric: golden ambient glow, floating light particles, soft environmental haze.
Backgrounds are soft-focus fantasy ruins or stone architecture, supportive rather than
detailed. The overall mood is cute and determined — a small figure with complete confidence.
Closest to Princess Connect, Granblue Fantasy chibi sprites, and similar fantasy gacha
in-game character art.

### ChatGPT Translation
```
Full chibi fantasy gacha art aesthetic — extreme chibi proportions with large round head
roughly one-third to one-half of total height and tiny elegant body, clean precise anime
linework with crisp flat cel shading and smooth clean shadow edges, detailed fantasy plate
armor with gold trim and decorative motifs rendered carefully at chibi scale, oversized
fantasy sword and shield proportional to chibi frame, flowing wind-swept hair with strand
separation, dynamic low-angle action pose with debris and motion particles, warm golden
ambient lighting with floating atmospheric particles, soft-focus fantasy ruins or stone
architecture background, cute determined expression, confident and capable despite small
frame, Princess Connect and Granblue Fantasy chibi character art quality.
```

### Niji Journey Translation
```
full chibi proportions large round head tiny body, cute fantasy chibi character, clean anime
linework crisp flat cel shading, detailed fantasy plate armor gold trim decorative motifs,
oversized sword and shield chibi scale, flowing wind-swept hair strand separation, dynamic
low-angle action pose debris particles mid-motion, warm golden ambient lighting floating
particles atmospheric haze, soft focus fantasy ruins stone architecture background, cute
determined expression, confident capable chibi warrior, Princess Connect gacha chibi art
style --ar 16:9
```

---

## STYLE: Webtoon
**Aliases:** webtoon, manhwa, korean webtoon, line webtoon, solo leveling, tower of god, manhwa art
**Best for:** dramatic character moments, fashion-forward character designs, urban fantasy, action sequences, romance and slice-of-life, any scene that benefits from crisp clean linework and strong character presence
**Conflicts with:** Kurosawa, Aquarelle, Crewdson, painterly or atmospheric styles, anything requiring analog texture or heavy environmental mood

### Visual Description
The clean, high-polish aesthetic of Korean webtoon and manhwa — Solo Leveling, Tower of God,
True Beauty visual language. Linework is crisp and confident with consistent weight, slightly
rounder and more fashion-forward than Japanese manga. Shading is smooth and controlled, often
cel-style with soft gradient accents on hair and skin. Characters are the undisputed focal
point — faces expressive, hair rendered with precision and volume, clothing detailed and
fashion-conscious. Color is saturated but clean; palettes are deliberate rather than
atmospheric. Backgrounds are either high-detail and architectural or minimal, depending on
the scene. The overall feel is polished, modern, and cinematic — built for scrolling vertical
presentation but striking in any format.

### ChatGPT Translation
```
Korean webtoon and manhwa aesthetic — crisp confident linework with consistent line weight,
smooth cel shading with soft gradient accents on hair and skin, fashion-forward character
design with expressive faces and precisely rendered hair volume, saturated clean color
palette, characters as the primary focal point against either high-detail architectural
backgrounds or minimal clean settings, polished cinematic production quality, Solo Leveling
and Tower of God visual language.
```

### Niji Journey Translation
```
Korean webtoon manhwa style, crisp clean confident linework, smooth cel shading soft
gradients, fashion-forward character design, expressive face precise hair rendering,
saturated clean color palette, strong character focus, polished cinematic quality,
modern digital anime aesthetic, Solo Leveling style, Tower of God aesthetic --ar 9:16
```

---

## STYLE: Liminal Horror
**Aliases:** liminal horror, liminal, backrooms, liminal space, horror, scp, wrong lighting, unsettling
**Best for:** empty institutional spaces, abandoned or transitional environments, psychological unease, scenes where the setting itself is the subject, any image where dread comes from wrongness rather than explicit threat
**Conflicts with:** warm or inviting palettes, fantasy environments, character-forward portraits, any style with explicit beauty or grandeur

### Visual Description
The visual language of liminal spaces and psychological horror — emptiness that feels wrong.
Scenes are mundane environments (hotel corridors, empty swimming pools, fluorescent-lit
offices, stairwells, mall food courts at 3am) rendered with hyperreal clarity that makes
the absence of people feel like a presence. Lighting is institutional and flat — fluorescent
buzz, yellow incandescent wash, or overexposed daylight from windows. Color is desaturated
and slightly wrong: yellowed whites, olive-tinged shadows, colors that feel slightly
off-temperature. Depth and perspective are slightly exaggerated, making spaces feel larger
or more receding than they should. If figures are present, they are ambiguous — too far,
too still, or facing away. The dread is in the mundane, not the monstrous.

### ChatGPT Translation
```
Liminal space and psychological horror anime illustration — mundane environments (empty
corridors, pools, offices, stairwells) rendered with clinical clarity, institutional
lighting (fluorescent, yellow incandescent, overexposed window light), desaturated slightly
wrong color palette (yellowed whites, olive shadows, off-temperature tones), exaggerated
depth and perspective that makes spaces feel too large or too receding, absence of people
as a presence in itself, dread through mundane wrongness rather than explicit threat,
backrooms and liminal space visual language, 2D anime art style.
```

### Niji Journey Translation
```
liminal space aesthetic, empty mundane environment, hyperreal clinical rendering,
institutional fluorescent lighting yellow incandescent, desaturated wrong color temperature
yellowed whites olive shadows, exaggerated depth perspective, vast empty space, absence
of people, psychological unease, backrooms visual language, wrongness without explicit
threat, still and silent atmosphere --ar 16:9
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
anime storybook illustration, soft warm painterly anime style, gouache-like digital painting,
rounded anime characters large expressive eyes soft simplified silhouettes, warm palette
ochre sage green dusty rose cream, gentle brush texture soft color washes, whimsical anime
fairy tale environments, simplified charming backgrounds, wonder and warmth mood, Japanese
anime picture book aesthetic, Ghibli artbook illustration style --ar 4:3
```

---

## STYLE: Kuudere
**Aliases:** kuudere, cool anime, midnight portrait, reserved anime, cool character, quiet authority
**Best for:** composed or world-weary characters, traveler and mage archetypes, kuudere personality types, any portrait where the contrast between a small youthful appearance and quiet experienced presence is the point
**Conflicts with:** Moe Gacha, Ember, Studio Ghibli, Storybook — anything warm, bright, or emotionally open; this style is cool, restrained, and closed

### Visual Description
Clean digital anime lineart with precise, confident strokes and semi-flat cel shading. The
defining quality is restraint — nothing is bright, nothing is warm, nothing is exaggerated.
The color palette is built entirely from cool tones: midnight blues, muted purples, steel
greys, dark neutrals, and fair cool-undertone skin. Eyes are large in the anime tradition
but calm and slightly heavy-lidded — wise and watchful rather than energetic or expressive.
Default expression is composed and reserved, carrying the quality of someone who has seen
enough to stop being surprised. Character proportions lean petite and delicate — a small,
slight frame that contrasts quietly with the weight of presence the character carries. The
contrast between the youthful softness of the appearance and the composed, capable demeanor
is the defining tension of the style. Backgrounds are minimal or atmospheric — cool fog,
soft shadow — so nothing competes with the character.

### ChatGPT Translation
```
Kuudere anime aesthetic — clean precise digital lineart with semi-flat cel shading, cool
restrained palette of midnight blues, muted purples, steel greys, and dark neutrals, fair
pale complexion with cool undertones, large calm eyes with slightly heavy lids and steel
blue irises (wise and watchful, not bright or energetic), composed reserved expression with
quiet world-weary authority, petite delicate proportions that contrast with the weight of
presence, practical layered clothing in deep cool tones, minimal or cool atmospheric
background, nothing warm, nothing exaggerated, understated elegance throughout.
```

### Niji Journey Translation
```
kuudere anime character, clean precise digital lineart, semi-flat cel shading, cool dark
palette midnight blue muted purple steel grey dark neutrals, fair pale skin cool undertone,
large calm heavy-lidded eyes steel blue irises, composed reserved expression quiet authority,
petite slender delicate frame, practical layered cool-toned clothing, minimal atmospheric
background, restrained understated elegance, no warm colors, no exaggerated expressions
--ar 2:3
```

---

## ADD YOUR OWN STYLE

## STYLE: Gacha Splash
**Aliases:** gacha splash, anime splash, key visual, gacha art, vtuber art, jrpg splash, anime key visual, gacha key visual
**Best for:** high-energy character moments, fantasy RPG characters, VTuber key visuals, spell casting and power moments, dynamic poses with motion, any scene that needs premium cinematic gacha production quality
**Conflicts with:** Kurosawa, Crewdson, Liminal Horror, Miura — anything restrained, dark, or static in a grounded way; this style is inherently energetic and polished

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
modern fantasy anime gacha art, semi-chibi proportions, polished gacha game illustration,
clean precise linework subtle line weight variation, hybrid cel shading painterly gradients,
airbrushed skin soft shadow transitions, glossy hair highlights fine strand separation,
metallic armor reflection, warm bloom lighting rim light hair and armor, floating light
particles atmospheric haze, dynamic motion composition depth of field, soft focus fantasy
castle background, magical heroic elegant mood, anime RPG splash art quality, VTuber
key visual aesthetic, ultra detailed digital painting --ar 2:3
```

---

## STYLE: Tactical Ink
**Aliases:** tactical ink, mil-moe, military manga, ink mecha, hard ink, mech sketch
**Best for:** soldiers and military characters, powered armor and mecha, sci-fi hardware, characters with complex tactical equipment, post-apocalyptic figures, pilot portraits
**Conflicts with:** painterly styles, Aquarelle, Ember, Makoto Shinkai, Prism, Studio Ghibli — anything soft, lush, or color-saturated; this style is restrained by design

### Visual Description
Clean flat manga ink linework applied to structurally complex mechanical and military subjects.
Complexity comes from the number of parts — panel seams, joint assemblies, bolt clusters,
cable runs — not from texture density. Each armor panel has a large flat interior with clean
color fill and no hatching or crosshatch shading. Wear is sparse and surgical: a few strategic
grime dots or scratch lines, never covering surfaces. Characters have soft anime proportions
and expressive faces placed in sharp contrast against the hard mechanical structure. Negative
space is preserved aggressively — within the armor itself, around the subject, and in the
background. The result feels light and airy despite the mechanical complexity. Line economy
over density. Palette is user-defined; the style is fully palette-agnostic.

### ChatGPT Translation
```
2D manga illustration, flat clean ink linework, anime character with soft expressive face —
mechanically complex armor and tactical hardware rendered with structural precision: clean
panel seam lines, joint assemblies, bolt and cable detail, large flat color fills inside each
armor panel with no hatching or texture, sparse intentional wear limited to a few strategic
grime dots and scratch marks, strong contrast between soft anime face and hard mechanical
structure, generous negative space preserved throughout including within the armor, minimal or
white background, line economy over density, light airy feel despite mechanical complexity,
professional manga illustration quality.
```

### Niji Journey Translation
```
flat manga ink linework, soft anime face, complex military mecha armor, clean panel seam
lines joint assemblies bolt detail, large flat color fills inside armor panels no hatching
no crosshatch no texture fill, sparse minimal wear marks few grime dots only, strong contrast
soft face hard machine, generous negative space within and around armor, white or minimal
background, light airy composition, line economy not density, flat 2D manga rendering,
professional manga illustration --ar 1:1
```

---

## STYLE: Cinematic Anime
**Aliases:** cinematic anime, studio anime, anime key art, premium anime illustration, anime concept art, visual novel art
**Best for:** character portraits with real-world equipment, motorsport and race characters, action characters at rest, fantasy OCs in grounded settings, strong directional lighting scenes, high production quality without photorealism
**Conflicts with:** Hyperreal Anime (photorealistic skin/materials vs. illustrated), flat cel shading, chibi proportions, Tactical Ink (ink lines vs. painted rendering)

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
cinematic anime illustration, high quality 2D anime art, smooth clean anime skin, strong
directional sunlight, warm golden color grading, hard shadows rim lighting, illustrated
material texture leather and gear, anime sweat beads illustrated wear, natural anime
proportions, premium game concept art quality, semi-realistic anime illustration style,
detailed anime digital painting --ar 2:3
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
semi-photorealistic anime, hyperreal rendering, worn leather suit, race gear with sponsor
patches, physical material texture, sweat on skin, strong directional sunlight, warm afternoon
color grade, shallow depth of field, soft bokeh background, cinematic realism, elf character,
detailed surface wear and grime, semi-realistic 2D anime --ar 2:3
```

**Dreamy sub-mood:**
```
semi-photorealistic anime portrait, hyperreal soft rendering, real skin texture with freckles,
dreamy backlit atmosphere, overexposed warm light, soft bokeh, floating light particles,
heart bokeh, pastel lens haze, emotionally quiet, eyes closed, elf character, white clothing,
contemplative mood, semi-realistic 2D anime --ar 2:3
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
cinematic anime key visual, premium dark fantasy gacha illustration, Pixiv masterpiece quality,
polished soft-rendered anime shading, refined anime line art, smooth gradient shadows,
glossy digital rendering, satin velvet material rendering reflective luxury fabrics,
deep crimson violet lighting palette, atmospheric neon noir undertones,
sophisticated color harmony controlled contrast, richly layered lighting,
soft bloom highlights, subtle rim lighting, diffused city-light bokeh,
luminous eyes focal anchor brilliant detailed, elegant character design,
clean anime facial structure, moody nighttime ambiance, ethereal cinematic atmosphere,
soft-focus background shallow depth of field city light bokeh,
highly detailed stylized anime rendering smooth shading transitions refined linework
--no painterly texture, sketch lines, flat cel shading, atmospheric suppression,
lost-and-found edges, moe chibi, dynamic action pose --ar 2:3
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
semi-chibi anime character, slightly oversized head soft rounded proportions, clean flat
cel shading, slice of life interior setting, carefully rendered everyday objects food
tableware furniture, warm ambient interior lighting, neutral or quietly unamused expression,
clean anime linework, cozy grounded mood, casual everyday scene, off-duty character moment,
gacha daily life aesthetic --ar 1:1
```

---

## STYLE: Gossamer
**Aliases:** gossamer, light novel, visual novel, visual novel cg, soft anime, pastel anime, soft fantasy, healing anime, iyashikei, fantasy portrait, shrine maiden, light novel illustration, porcelain anime
**Best for:** fantasy portraiture, visual novel CGs, light novel character illustrations, iyashikei and healing atmosphere scenes, elegant character showcases, spring or summer fantasy environments, floral scenes, tranquil interiors, fantasy fashion, elves, shrine maidens, noblewomen, romantic character art, serene magical settings
**Conflicts with:** Miura, Soulslike, Neon Noir, Liminal Horror, Ironbloom, Cinematic Anime, Hyperreal Anime, Kurosawa, Crewdson — anything dark, gritty, high-contrast, dramatic, or with strong directional lighting

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
soft flat anime style, barely visible thin outlines soft line color, flat cel shading
single shadow tone, lifted dark values near-shadowless rendering, no gradients no
blending, ambient lighting no directional source, muted cool palette sage green dusty
aqua off-white, blurred simplified background no detail, smooth flat hair planes single
shine streak, clean textureless skin faint cheek blush, large flat aqua grey-blue irises,
light novel illustration quality, minimal weightless illustrative 2D anime --ar 2:3
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

### ChatGPT Translation
```
Flat cel anime illustration — clean thin line art with a single hard-edged shadow tone and lifted dark values reading nearly shadowless, no gradients or blending, completely ambient lighting with no directional source or cast shadows, simplified flat background, hair as smooth flat planes with a single shine streak, clean textureless skin, [user-defined palette and mood per scene]. Drawn as a clean flat modern anime illustration, 2D anime art style, no painterly texture, no complex shading, no photorealism.
```

### Niji Journey Translation
```
flat cel shading anime illustration, single shadow tone lifted dark values near-shadowless, no gradients no blending, ambient lighting no directional source no cast shadows, clean thin line art consistent weight, flat smooth hair planes single shine streak, clean textureless skin, simplified flat background, [user-defined palette and mood per scene], clean flat modern 2D anime --ar [ratio]
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

### ChatGPT Translation
[Prose language to weave into the ChatGPT prompt — 1–3 sentences]

### Niji Journey Translation
[Keyword-dense form + any recommendation]
```
