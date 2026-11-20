---
name: "camera-fpv-drone"
description: "FPV drone — one continuous drone flight: a dive from above, a low skim over the surface and a sharp pull-up onto the hero. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) that needs a dynamic showcase of a place — travel, hotels, real estate, restaurants, events."
---

# FPV drone (a one-shot drone fly-through)

The drone dives from above, races along the terrain and pulls up sharply onto the hero, who greets the camera. In a few seconds the viewer gets the whole place plus an emotional payoff at the end. The best move for travel, hotels, real estate and events.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- One continuous shot, no cuts.
- A four-point route: high above the location, a dive down along a vertical feature, a low skim over the surface, a sharp pull-up to the hero.
- Fast, fluid banking turns with a tilting horizon.
- Ending: a close-up of the hero making a gesture to the camera (raising a glass, showing the product, waving).
- Audio: rushing wind, the sound of the surface, an accent on the final gesture.
- Always keep the lines `FPV drone shot ONLY` and `One continuous shot, no cuts`.

## What to swap in
Film stock or look, time of day and light, the wide view of the location, a vertical feature (cliff, facade, waterfall), the surface (sea, street, pool, vineyard), the arrival point (terrace, entrance, deck), the hero (with an Image 1 reference), the gesture to the camera, sounds.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT], cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. Camera movement: FPV drone shot ONLY. The drone dives fast from above [WIDE LOCATION], plunges down [VERTICAL FEATURE], skims low over [SURFACE], then pulls up sharply onto [DESTINATION] where [SUBJECT], [detail], [GREETING ACTION to the camera]. Fast, fluid banking turns. End: close on [SUBJECT] [smiling / PRODUCT in focus]. Audio: rushing wind, [SURFACE SOUND], [accent sound of the final action]. One continuous shot, no cuts.
```

## Source example
```
Shot on Kodak Vision3 250D 35mm film, golden hour, warm sun flares, cinematic. Image 1 is Dolores: keep her exact face, grey hair, glasses and clothing. Camera movement: FPV drone shot ONLY. The drone dives fast from above a white Mediterranean village on a cliff, plunges down the cliff face, skims low over the sea, then pulls up sharply onto a terrace where Dolores, wearing sunglasses, raises a glass of vermouth to the camera. Fast, fluid banking turns. End: close on Dolores smiling. Audio: rushing wind, waves, a glass clink. One continuous shot, no cuts.
```

## With HyperFrames
- **Live-action shot.** This move almost always needs a generated clip. Generate it from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the wind, the surface sound and the final accent in the compose prompt. Put a title or call to action on the final close-up.
- **Without generation.** In compose, describe a fly-through over a large map or collage: a fast continuous move from the wide view to the destination with increasing scale, a slight frame tilt on the turns and motion blur, stopping on a card for the place or product. Works well for a travel route.

## Tips
- Describe the route with movement verbs in order (dives, plunges, skims, pulls up): the model follows them like waypoints.
- You can't fit more than four route points into one clip: the shot will fall apart.
- The gesture to the camera at the end is a must: without it the fly-through is just a pretty view.
- For 9:16, choose routes with a vertical feature (cliff, tower, facade): the dive reads much stronger.
