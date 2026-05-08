---
title: "Image 2.0 Style System"
lead_reference: "images-2-indie-comic"
use_case: illustration-story
created: 2026-04-23
---

# Image 2.0 Style System

## Intent

Generate scene art for a mobile-first medical explainer comic about a patient's first seizure doctor visit.

The art should feel:
- warm
- editorial
- human
- tactile
- calm rather than dramatic
- simple and close to the original PDF comic unless a prompt asks for another style

The best-fit reference direction is the `images-2-indie-comic` branch from the local Image 2.0 style guide.

## What To Keep From The Existing Comic

- Marcus in an olive hoodie
- supportive mother in burgundy
- father in gray polo
- Dr. Rehim as the updated simplified likeness from `physician-reference.md` and `../assets/characters/dr-rehim-character-sheet-simplified-v2.png`: light olive skin, dark side-swept hair with soft volume, clear translucent glasses, strong brows, smooth face, soft smile lines, and a gray or brown blazer over a dark shirt
- warm clinic environment
- approachable, non-threatening tone

## What To Change

- no multi-panel page compositions
- no giant speech balloons
- no long explanatory text inside the image
- stronger composition and more intentional negative space
- cleaner emotional focus per scene

## Generation Rules

1. Generate one scene at a time.
2. Use 6:5 composition sized for a mobile card unless a prompt specifically asks for another ratio.
3. Keep all critical text out of the image.
4. Avoid comic-panel borders unless a specific prompt asks for a two-moment split.
5. Do not include readable paperwork, forms, or medical chart text.
6. Keep the clinic modern, calm, bright, and believable.

## Character Lock

- Marcus: early-20s Black man, short fade, olive green hoodie, dark jeans, white sneakers
- Mrs. Johnson: Black woman, shoulder-length natural curls, burgundy cardigan, cream blouse
- Mr. Johnson: Black man, gray polo, khaki pants, broadest silhouette
- Dr. Rehim: match the active simplified physician character sheet in `../assets/characters/dr-rehim-character-sheet-simplified-v2.png`; light olive skin, dark brown to black side-swept hair with soft volume, clear translucent rectangular-round glasses, strong dark eyebrows, oval face, softly defined jaw, smooth simplified face, clean-shaven or only the faintest stubble, calm listening smile; wardrobe is a brown or gray blazer over a dark knit or shirt with tailored dark trousers; no white coat

## Eye And Face Style

- Match the original PDF comic's simple eye style.
- Eyes should be only small, slightly vertical black dots or short vertical ovals.
- Do not draw whites of the eyes, eye outlines, eyelid lines, irises, pupils inside whites, highlights, glossy pupils, realistic eyes, or almond eye shapes.
- For Dr. Rehim, eyes behind glasses should still read as small vertical black dots, not detailed eyes. Draw the glasses frame only; do not let the glasses create whites, eye outlines, eyelid lines, or almond-shaped eyes.
- Keep faces simple, flat, and cartoon-like with restrained expressions.

## House Prefix

Use this at the start of each Image 2.0 prompt:

`Art-directed editorial comic illustration with tactile analog texture, warm human-centered storytelling, restrained palette, soft paper grain, generous negative space, emotionally legible body language, and composition designed for a mobile vertical reading experience.`

## Shared Constraints

- no speech balloons
- no readable text embedded in the art
- no stock-photo realism
- no glossy CGI finish
- no harsh hospital drama
- no cluttered background
- no medical horror cues
- do not turn Dr. Rehim into a generic hospital doctor; keep his glasses light and translucent, and avoid ID badge text or white-coat styling
- keep Dr. Rehim simpler and smoother than a portrait reference; avoid pores, heavy stubble, fine wrinkles, and dense facial hatching

## Prompt Skeleton

```text
Use case: illustration-story
Asset type: mobile web comic scene card
Primary request: <one scene only>
Subject: Marcus, his parents, and/or Dr. Rehim
Scene/backdrop: modern neurology clinic, waiting room, consult room, or clinic exterior
Style/medium: simple patient-education comic close to the PDF, warm ink and restrained watercolor
Composition/framing: 6:5, clear focal point, readable on a phone
Lighting/mood: soft daylight, reassuring, calm
Color palette: cream, warm charcoal, olive, burgundy, muted teal accents
Materials/textures: off-white paper, inked outlines, soft watercolor wash
Constraints: no speech balloons, no readable text, no panel grid unless explicitly requested
Avoid: glossy CGI, photorealism, medical fear imagery, busy background clutter
```

## Pilot Deliverables

Generate these first:
- cover / hero
- check-in scene
- meeting doctor scene
- leaving with a plan scene
