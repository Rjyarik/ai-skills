---
name: "camera-dolly-zoom"
description: "Dolly zoom (vertigo effect) — the camera dollies back while the lens zooms in, so the hero stays the same size while the background changes scale. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) when you need to show a moment of realisation, a customer's pain point, shock or a sudden decision."
---

# Dolly zoom (vertigo effect)

The camera travels backward while the lens zooms in at the same time. The hero's face stays the same size while the space behind them "warps". The viewer physically feels the hero's inner shift: "oh no", "so that's it", "I need this".

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- Two movements at once: dolly back and zoom in. The hero's size in the frame stays constant.
- The hero stands still; only the emotion on the face changes (eyes widening, a slow smile).
- Speed is slow and constant, no jerks.
- You need a deep background with perspective lines: an aisle, a corridor, a street, rows of shelves.
- Audio: a low droning tone plus quiet location ambience.
- Always keep the lines `dolly zoom ONLY (vertigo effect)` and `No pan, no cuts`.

## What to swap in
Film stock or look, light, the hero (with an Image 1 reference), a deep location, the trigger of the realisation (an empty shelf, a screen, a sign, a price tag), the emotion shift, background audio.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [LIGHT], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. [SUBJECT] stands still in the middle of [LONG DEEP LOCATION: aisle, corridor, street], in front of [TRIGGER OBJECT], realising [WHAT], [EMOTION SHIFT: eyes widening / slow smile]. Camera movement: dolly zoom ONLY (vertigo effect). The camera dollies backward while the lens zooms in, so [SUBJECT]'s face stays the same size while the [BACKGROUND] behind stretches away. Speed: slow and constant. Audio: low droning tone, [AMBIENCE]. No pan, no cuts.
```
Mirrored version for a positive "wow": `The camera dollies forward while the lens zooms out` — the background opens up wide.

## Source example
```
Shot on Kodak Vision3 250D 35mm film, flat fluorescent supermarket light, fine grain, cinematic. Image 1 is Dolores: keep her exact face, grey hair, glasses and clothing. Dolores stands still in the middle of a long supermarket frozen-food aisle in front of an empty shelf with a sign that reads AGOTADO, realising the croquettes are gone, eyes widening. Camera movement: dolly zoom ONLY (vertigo effect). The camera dollies backward while the lens zooms in, so her face stays the same size while the aisle behind her stretches away. Speed: slow and constant. Audio: low droning tone, fridge hum. No pan, no cuts.
```

## With HyperFrames
- **Live-action shot.** Generate the clip from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the low tone and ambience in the compose prompt.
- **Without generation.** You need two layers: the cut-out hero (a PNG with no background) and a separate background. In compose, describe: the hero is still and does not change size, the background slowly and evenly scales from 1 to 1.3–1.5 from the center over the full length of the shot, with a slight vignette. The effect won't work from a single flattened image.

## Tips
- It's a strong move: once per video is enough.
- Works well at the start of a video as "the customer's problem", followed by the solution.
- Keep any trigger text in the frame (a sign, a price tag) short: models get long text wrong.
- For 9:16, keep the face in the upper third, with the perspective receding behind the hero in the center.
