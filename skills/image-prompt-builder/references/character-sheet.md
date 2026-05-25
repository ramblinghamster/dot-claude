# Character Sheet Format
## Image Prompt Builder — Production Reference Sheet Specification

This file defines the structure and layout requirements for generating anime-style character
reference sheets. It is an **output format**, not a visual style — it defines what panels to
include and how to organize them. Apply a visual style from `styles.md` alongside this format
to define the aesthetic.

When a user requests a character sheet, load this file and ask:
> "Which visual style should the sheet use? (e.g., Ironbloom, Aquarelle, Ember — or describe
> your own aesthetic)"

Then apply both: this file for structure, the chosen style for look.

---

## Core Design Goals

The character sheet should:
- Present the character clearly from multiple angles
- Maintain strict visual consistency across all panels
- Showcase outfit construction and equipment details
- Provide expression references
- Support future illustration consistency
- Feel like a professional game/anime production asset
- Use clean infographic-style organization
- Maintain readable spacing and layout hierarchy

---

## Art Style Requirements

### Rendering (override with chosen visual style)
- High-quality anime concept art
- Studio production design aesthetic
- Clean linework
- Soft cel shading with subtle painterly gradients
- Matte textures over glossy rendering
- Consistent proportions across all panels
- Controlled anime stylization (not chibi unless intentional)
- Professional RPG/fantasy visual design

### Lighting
- Neutral studio lighting
- Minimal dramatic shadows
- Readability prioritized over cinematic mood
- White or light parchment background

### Composition
- Flat orthographic presentation for reference panels
- Dynamic pose allowed only in action section
- Consistent scale and anatomy

---

## Standard Layout — 12 Panels

### Panel 1 — Character Information
*Location: top-left*

Required fields:
- Character name, race/species, age, class/job
- Height, weapon type, affiliation, alignment
- Years adventuring (if applicable)

Optional:
- Short lore paragraph, personality summary, background notes

---

### Panel 2 — Full Body Turnaround
*Main centerpiece*

Required views: **Front · 3/4 · Side · Back** · Optional: weapon pose variant

Requirements:
- Consistent proportions and outfit construction across all views
- Accurate equipment placement
- Hair consistency between views
- Proper silhouette readability

---

### Panel 3 — Expression Sheet
*Upper-middle or right section*

Include 4–6 expressions from:
Neutral · Determined · Happy · Surprised · Concerned · Reflective · Battle Ready

Requirements:
- Same face structure across all expressions
- Consistent eye shape and hairstyle continuity
- Emotional readability

---

### Panel 4 — Color Palette
*Small swatch area*

Swatches for:
- Hair, eyes, skin tone
- Primary and secondary outfit colors
- Leather, metal, accent materials

---

### Panel 5 — Hair Breakdown
*Front · Side · Back views*

Requirements:
- Accurate volume and silhouette
- Correct hair accessories
- Consistency with turnaround views

---

### Panel 6 — Close-Up Detail Panels
*Small zoom-in panels*

Select relevant elements from:
Eye detail · Gloves · Belt · Boots · Jewelry · Hair ornament · Embroidery ·
Staff crystal · Weapon engraving · Buckles/pouches

---

### Panel 7 — Outfit Breakdown
*Separated outfit components*

Typical panels: Upper body · Cloak/cape · Corset · Shirt/vest · Legwear ·
Boots · Gloves · Skirt layers · Armor pieces

Requirements:
- Layer logic must make physical sense
- Outfit must look wearable
- Practicality balanced with style

---

### Panel 8 — Equipment & Accessories

Show secondary carried items relevant to class:

| Class | Items |
|---|---|
| Mage | Spellbook, potion vials, satchel, focus crystal, ink & quill |
| Thief | Lockpicks, smoke bombs, grappling hook, throwing knives |
| Warrior | Pouches, maintenance tools, combat accessories |
| Healer | Medical kits, holy charms, recovery potions |

---

### Panel 9 — Weapon Sheet

Views: **Front · Side · Back · Detail close-up** · Optional: exploded parts view

Requirements:
- Consistent scale, clear material definition
- Practical grip/handling
- Visual storytelling through wear and use marks

---

### Panel 10 — Action Pose
*Single dynamic illustration*

Purpose: demonstrate personality, combat style, outfit movement

Requirements:
- More cinematic treatment allowed here
- Consistent with rest of sheet design
- Effects must not obscure character

---

### Panel 11 — Scale Reference
Silhouette comparison: character · average human · weapon height

---

### Panel 12 — Silhouette Panel
Black silhouette variants for readability testing.
Used for: game design · animation readability · visual identity testing

---

## Character Age Progression Guidelines

When creating sheets across different life stages:

| Phase | Character Traits | Equipment |
|---|---|---|
| Teen / Student | Cleaner outfit, softer face, smaller frame, less confidence | New/simple gear, few survival tools |
| Novice Adventurer | Sharper features, better posture, practical modifications | Extra pouches, travel wear, small repairs |
| Veteran Adventurer | Mature structure, composed expressions, calm confidence | Worn materials, reinforced gear, trophy history |

---

## Material Rendering Standards

| Material | Treatment |
|---|---|
| Fabric | Matte, visible stitching, fold logic |
| Leather | Slight wear, edge discoloration, stress creases |
| Metal | Scratches, tarnish, edge wear |
| Aged cloth | Fraying, repairs, patchwork, dirt accumulation |

---

## Fantasy RPG Design Principles

**Characters should feel:** visually striking · functional · role-appropriate · distinct at silhouette level

**Avoid:** overcrowded detail · random accessories · inconsistent materials ·
overdesigned silhouettes · excessive ornamentation without purpose

---

## Prompt Keywords

**Positive:**
anime character reference sheet · turnaround sheet · professional model sheet · clean layout ·
labeled parts · studio anime style · concept art sheet · RPG character design · cel shaded ·
high detail · consistent proportions

**Negative:**
cluttered · messy layout · inconsistent anatomy · extra limbs · low detail ·
photorealistic · chibi · distorted proportions

---

## Output Specifications

**Preferred aspect ratio:** 16:9
**Alternative:** 21:9 for very large multi-panel sheets

**Layout feel:**
- Clean infographic organization
- Thin decorative dividers
- Elegant fantasy typography
- White or parchment background
- Consistent spacing
- Balanced visual density

---

## Final Quality Checklist

Before marking production-ready, confirm:

- [ ] Character proportions consistent across all views
- [ ] Hair consistent across all panels
- [ ] Outfit construction logically layered
- [ ] Weapons correctly scaled
- [ ] Expressions recognizable and distinct
- [ ] Materials visually distinct from each other
- [ ] Accessories role-appropriate
- [ ] Layout readable with clear hierarchy
- [ ] Silhouette unique and readable
- [ ] Age progression believable (if applicable)
