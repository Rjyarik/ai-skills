---
name: "camera-rack-focus"
description: "Rack focus — focus pulls from an object in the foreground to the hero deeper in the frame while the camera stays completely still. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) when you need to link a product and a person, show a reaction to a product, or shift attention from a detail to what matters most."
---

# Rack focus (focus pull)

The camera does not move at all. The object in the foreground is sharp, and the hero behind it is blurred. Then focus travels to the hero, who gives a small reaction, while the object falls out of focus. This links product and person in a single shot: an item and its buyer, a dish and a guest, a gadget and its owner.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- The camera is completely still: only the focus changes.
- A long lens (85mm) and a very shallow depth of field.
- Foreground: one object in sharp focus, filling one side of the frame.
- Background: the hero, out of focus.
- At second 2 focus shifts to the hero, who gives a micro-reaction to the camera (raises an eyebrow, smiles, nods).
- Audio is quiet and detailed: ticking, a faint sizzle, room tone.
- Always keep the lines `rack focus ONLY` and `No dolly, no zoom, no cuts`.

## What to swap in
Film look, light, the foreground object or product, the side of the frame, the hero (with an Image 1 reference), the hero's place and pose, the micro-reaction, quiet sounds.

## Prompt template
```
Shot on [FILM LOOK], [LIGHT], 85mm lens, very shallow depth of field, cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. Foreground: [OBJECT / PRODUCT], in sharp focus, filling the [left / right] of frame. Background: [SUBJECT] [pose and place], out of focus. Camera movement: rack focus ONLY. The camera is completely still; at second 2 focus shifts from [OBJECT] to [SUBJECT], who [MICRO REACTION] at the camera. [OBJECT] goes soft. Audio: [QUIET ROOM TONE], [faint detail sound]. No dolly, no zoom, no cuts.
```
Reverse version for an ad that ends on the product: start with focus on the hero and pull it to the product: `focus shifts from [SUBJECT] to [PRODUCT]. [SUBJECT] goes soft.`

## Source example
```
Shot on Kodak Portra 400 look, warm tungsten kitchen light at night, 85mm lens, very shallow depth of field, cinematic. Image 1 is Dolores: keep her exact face, grey hair, glasses and clothing. Foreground: a fork holding one golden croquette, in sharp focus, filling the left of frame. Background: Dolores sitting at the kitchen table, out of focus. Camera movement: rack focus ONLY. The camera is completely still; at second 2 focus shifts from the croquette to Dolores, who slowly raises one eyebrow at the camera. The croquette goes soft. Audio: kitchen clock ticking, faint sizzle. No dolly, no zoom, no cuts.
```

## With HyperFrames
- **Live-action shot.** Generate the clip from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the quiet sounds in the compose prompt. Place a title on the free side of the frame, opposite the object.
- **Without generation.** This move reproduces well in graphics. You need two layers: the foreground object (a PNG with no background) and a background with the hero. In compose, describe: for the first 2 s the foreground layer is sharp and the background is blurred by about 12–16 px; then over 0.6–0.8 s the blur swaps between them; both layers scale up by 1–2 percent to imitate lens "breathing".

## Tips
- The object and the hero must sit on opposite sides of the frame, otherwise the focus pull won't read.
- Keep the hero's reaction small: restraint is what makes this move work.
- For product cards and food ads, use the reverse version that ends on the product.
- For 9:16, put the object at the bottom of the frame and the hero higher up and deeper in.
