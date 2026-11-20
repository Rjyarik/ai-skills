---
name: "camera-dolly-out"
description: "Dolly out — a fast camera pull-back from a close-up of a face or detail to an extreme wide shot that reveals the scale around the hero. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) when you need a reveal — showing the system, team, product range or audience behind one person or product."
---

# Dolly out (pull-back reveal of scale)

The shot opens on a close-up of a calm face. The camera pulls straight back fast, and it turns out the hero is standing alone in the middle of a huge space, surrounded by hundreds of identical objects, all facing them. The move flips the meaning of the shot: from a single person to the scale of what stands behind them.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- Opening frame: a close-up of a face or detail that gives no clue about the surroundings.
- The camera travels straight back in a line, fast; no pans, no zoom, no cuts.
- The reveal: the hero alone in a huge space, surrounded by hundreds of identical objects, all turned toward them.
- End: an extreme wide shot, the hero small in the center.
- Audio builds with the pull-back: a low hum plus detailed sounds from the objects.
- Always keep the lines `dolly out ONLY` and `No pan, no zoom, no cuts`.

## What to swap in
Film stock or look, key light and rim light color, the hero or product (with an Image 1 reference), a huge space (warehouse, hangar, hall, stadium, field), the mass of objects around them (robots, screens, boxes, people, cars), sounds.

For a brand, the mass of objects = what stands behind the hero: AI agents, the team, customers, products, orders, servers, travel destinations.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [KEY LIGHT], [RIM LIGHT COLOR] rim light, haze, cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. Opening frame: close-up of [SUBJECT]'s calm face, lit in [COLOR]. Camera movement: dolly out ONLY. The camera pulls straight back fast, revealing that [SUBJECT] stands alone in [VAST SPACE] surrounded by [HUNDREDS OF OBJECTS with a shared visual detail], all turned toward [SUBJECT]. End: extreme wide shot, [SUBJECT] small in the center. Audio: [LOW HUM] rising, [OBJECT DETAIL SOUNDS]. No pan, no zoom, no cuts.
```

## Source example
```
Shot on Kodak Vision3 500T 35mm film, dark industrial light, red rim light, haze, cinematic. Image 1 is the man: keep his exact face, shaved head, clear glasses, beard and black T-shirt. Opening frame: close-up of his calm face, lit in red. Camera movement: dolly out ONLY. The camera pulls straight back fast, revealing that he stands alone in a vast warehouse surrounded by hundreds of frozen humanoid robots with glowing red LED faces, all turned toward him. End: extreme wide shot, him small in the center. Audio: low electronic hum rising, servo whirs. No pan, no zoom, no cuts.
```

## With HyperFrames
- **Live-action shot.** Generate the clip from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the rising hum in the compose prompt. Put a title or tagline on the final extreme wide shot.
- **Without generation.** This move works well as graphics. In compose, describe: the shot opens on a tight close-up of the central element (a face, a logo, a product screen), then the whole scene quickly scales down from 5–6 to 1 with a smooth ease-out, revealing a grid of dozens or hundreds of elements around it (cards, screens, avatars, logos); the central element stays in the center; the sound builds until the stop.

## Tips
- The surrounding objects need a shared, bright detail (glowing faces, identical screens, one color): that is what makes the mass read at first glance.
- Keep the facial expression calm at the start: the contrast between calm and scale is what creates the effect.
- A strong closing shot for a video, or a transition to the logo.
- For 9:16, line the objects up in rows going back and up, not just out to the sides.
