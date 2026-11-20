---
name: "camera-orbit"
description: "Orbit — the camera glides around the hero or product in a smooth arc, keeping the subject centered while the background rotates behind it. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) that needs a hero shot, an introduction of a founder, expert or product, or a feeling of confidence and scale."
---

# Orbit (circling the hero)

The camera travels around the hero in a smooth arc. The hero stays in the center of the frame while the background turns behind them. This is the "meet our hero" shot: it makes a person or product the main character and shows the world around them.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- The camera moves along a circle around the subject; the subject stays centered the whole time.
- Camera height is chest level, speed is smooth and constant.
- The hero is almost still: a calm, confident pose, at most a small movement (wind in clothes, a head turn).
- The background must be readable and rotate nicely: a city skyline, the sea, a workshop, a hall.
- Always keep the lines `orbit ONLY` and `No zoom, no cuts`.

## What to swap in
Film stock or look, time of day and light, the hero or product (with an Image 1 reference), an object in hand, a location with a wide background, the arc angle (90, 180 or 360 degrees), direction, background audio.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face / product details]. [SUBJECT] stands [in LOCATION with a wide readable background], [holding OBJECT / posing], calm and confident. Camera movement: orbit ONLY. The camera circles [180] degrees around [SUBJECT] at chest height, keeping [SUBJECT] centered, while the [BACKGROUND] rotates behind. Speed: smooth constant motion. Audio: [AMBIENCE]. No zoom, no cuts.
```

## Source example
```
Shot on Kodak Vision3 500T 35mm film, blue hour, city lights, light grain, cinematic. Image 1 is the man: keep his exact face, shaved head, clear glasses, beard and black T-shirt. He stands on a windy rooftop above a glowing modern skyline, holding a cinema camera at his side, calm and confident. Camera movement: orbit ONLY. The camera circles 180 degrees around him at chest height, keeping him centered, while the skyline rotates behind him. Speed: smooth constant motion. Audio: wind, distant city. No zoom, no cuts.
```

## With HyperFrames
- **Live-action shot.** Generate the clip from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the ambience and music in the compose prompt. A name, title or product name works well as an overlay.
- **Without generation.** A real orbit can't be made from a single photo. For graphics, describe a 3D equivalent in compose: a product card, phone or mockup slowly rotates 30–40 degrees on the Y axis at constant speed, the background drifts the opposite way (parallax), the object stays centered.

## Tips
- 180 degrees is enough for a 5–8 second clip; 360 needs more time and breaks faces more often.
- If the model distorts the face during the turn, shorten the arc to 90–120 degrees.
- For a product: put it on a plinth or table; a backlight gives a nice rim on the turn.
- For 9:16, pick a tall background (skyscrapers, cliffs, shelving) so the rotation reads in a narrow frame.
