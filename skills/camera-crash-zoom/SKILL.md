---
name: "camera-crash-zoom"
description: "Crash zoom — a violent zoom from a wide shot to an extreme close-up in a fraction of a second. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) when a shot needs an accent, a punchline, the hero's reaction or a sudden reveal of a key product detail."
---

# Crash zoom (violent snap zoom)

The camera is locked off, a short pause, then in a fraction of a second the lens "flies" from a wide shot into an extreme close-up of one detail. It works like an exclamation mark: the hero's reaction, a punchline, a price, a logo, a key product detail.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- The camera is locked in place: only the zoom moves. No dolly, no pans, no cuts.
- A calm pause of about 2 seconds on the wide shot, then the zoom in a fraction of a second.
- The zoom targets one specific detail (eyes, logo, screen, button, label).
- A slight shake at the moment of "landing", then hold on a sharp close-up.
- Audio: a hard whoosh exactly on the zoom.
- Always keep the lines `crash zoom ONLY` and `No dolly, no pan, no cuts`: they stop the model from adding extra movement.

## What to swap in
Film stock or look, time of day and light, location, the hero or product (with an Image 1 reference), a static pose before the zoom, the target detail, background audio.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face / product details]. [SUBJECT] [stands still / holds a pose] in [LOCATION], [small static action], staring ahead. Camera movement: crash zoom ONLY. The camera stays locked in place; at second 2 the lens zooms violently in a fraction of a second from a wide shot to an extreme close-up of [TARGET DETAIL], with a tiny shake on landing. End: hold on [TARGET DETAIL], sharp. Audio: [AMBIENCE], a hard whoosh on the zoom. No dolly, no pan, no cuts.
```

## Source example
```
Shot on Kodak Vision3 500T 35mm film, night, sodium streetlight, heavy grain, cinematic. Image 1 is Ramón: keep his exact face, thick mustache, slicked-back hair, cream guayabera, gold chain and tattooed forearms. Ramón stands in a rain-soaked Mexico City alley, cigarette in his mouth, staring ahead. Camera movement: crash zoom ONLY. The camera stays locked in place; at second 2 the lens zooms violently in a fraction of a second from a wide shot to an extreme close-up of his eyes, with a tiny shake on landing. End: hold on his eyes, sharp. Audio: rain, distant traffic, a hard whoosh on the zoom. No dolly, no pan, no cuts.
```

## With HyperFrames
- **Live-action shot (people, locations, photorealism).** Generate the clip from the template in a video model (image-to-video with a reference) and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the whoosh and ambience separately in the compose prompt, with the whoosh tied to the moment of the zoom.
- **Without generation (product photo, screenshot, graphics).** Describe a virtual camera in compose: a static wide shot for 2 s, then scale from 1 to 4–6 in 0.15–0.25 s with hard acceleration and radial blur, 2–3 frames of micro-shake on the stop, a 1–2 s hold, a whoosh on the zoom. The source must be high resolution, otherwise the close-up will look mushy.

## Tips
- One crash zoom per clip: a second one cheapens the first.
- The target detail must already be visible in the wide shot and sit close to the center of the frame.
- Right after the zoom is a good place for a title, a price or a cut to the next shot.
- For 9:16, keep the hero and the target detail in the central third of the frame.
