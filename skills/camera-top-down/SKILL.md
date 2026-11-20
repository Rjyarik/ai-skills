---
name: "camera-top-down"
description: "Top-down — a straight overhead view with a slow clockwise rotation and a slight camera descent. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) when you need to show a table, a product layout, food, a workspace, a map, or a scene with two people and a hand action."
---

# Top-down (rotating overhead view)

The camera looks straight down at a table or surface, slowly rotates clockwise and descends a little. The viewer sees the whole layout like a diagram, while the slow rotation adds tension and a premium feel. The focus is on hands and objects.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- The camera is directly above the center of the surface, looking straight down, with no tilt.
- A slow clockwise rotation and a small descent at the same time.
- All participants and the whole surface stay in frame until the end.
- One slow hand action in the center (in the original, flipping a card).
- Audio: a muffled room murmur, object sounds, an accent on the action.
- Always keep the lines `top-down ONLY` and `No tilt, no cuts`.

## What to swap in
Film stock or look, light and color accents, the surface (table, counter, floor, map), the objects on it, the participants (with Image 1 and Image 2 references) or just hands, the hand action, sounds.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [LIGHT], [COLOR ACCENTS], cinematic. Image 1 is [SUBJECT A] ([key details]). Image 2 is [SUBJECT B] ([key details]). Keep both faces and outfits exact. [SUBJECTS] sit facing each other at [TABLE / SURFACE] in [LOCATION], [OBJECTS laid out between them]; [SUBJECT] slowly [SMALL HAND ACTION]. Camera movement: top-down ONLY. The camera looks straight down from directly above the [TABLE] and slowly rotates clockwise while descending a little. Framing: [all subjects] and the [TABLE] stay in frame. Audio: [ROOM MURMUR], [OBJECT SOUNDS], [accent on the hand action]. No tilt, no cuts.
```
Version without people: instead of the participants, write `Only hands enter the frame from [side]` and describe the product layout.

## Source example
```
Shot on Kodak Vision3 500T 35mm film, smoky casino light, green felt, gold accents, cinematic. Image 1 is Ramón (mustache, cream guayabera, gold chain). Image 2 is Dolores (grey hair, glasses). Keep both faces and outfits exact. Ramón and Dolores sit facing each other at a green baccarat table in a Macao casino, cards and stacks of chips between them; Dolores slowly flips one card. Camera movement: top-down ONLY. The camera looks straight down from directly above the table and slowly rotates clockwise while descending a little. Framing: both players and the table stay in frame. Audio: casino murmur, chips clicking, a card flip. No tilt, no cuts.
```

## With HyperFrames
- **Live-action shot.** Generate the clip from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the murmur, object sounds and the accent in the compose prompt.
- **Without generation.** This move is easy to do in graphics. Take an overhead photo of the layout or an interface mockup and describe in compose: the frame slowly and evenly rotates clockwise by 10–15 degrees and scales from 1 to 1.1 over the full length of the scene. Use an image with extra margin at the edges so no empty corners appear during the rotation.

## Tips
- Faces are barely visible from above: clothing, hair and hands make the characters recognizable. Include them in the reference details.
- The layout should be symmetrical or have a clear center: the rotation happens around it.
- Works well for food, unboxing, trip planning over a map, product sets and desks.
- For 9:16, turn the table so its long side runs vertically.
