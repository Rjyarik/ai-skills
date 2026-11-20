---
name: "camera-low-angle-tracking"
description: "Low-angle tracking — a knee-height camera moves backward in front of the heroes as they walk toward it in slow motion while something huge happens behind them. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) that needs an epic walk for a hero or team, a launch, an announcement or a feeling of power."
---

# Low-angle tracking (the heroes' walk from a low angle)

The camera is low, at knee height, and pulls back at exactly the heroes' speed. They walk straight at the viewer in slow motion while something enormous happens behind them, and they don't turn around. The low angle makes the heroes look bigger and stronger. The shot for a launch, an announcement, a team or a founder.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- The camera is at knee height, looking up at the heroes.
- The camera moves backward in front of the heroes at exactly their speed: their size in frame doesn't change.
- The heroes walk toward the camera side by side, centered in frame, in slow motion.
- A big event happens behind them; the heroes never look back. That is the whole effect.
- Light from the event backlights the heroes.
- Audio: the low boom of the event plus a slow-motion rumble.
- Always keep the lines `low-angle tracking ONLY` and `No zoom, no cuts`.

## What to swap in
Film stock or look, time of day, one or more heroes (Image 1, Image 2 references), an empty street, corridor or runway, the event behind them, the light source from the event, sounds.

The event doesn't have to be an explosion. For a brand, try fireworks, a confetti blast, a sign or shop window lighting up, a giant screen, a wave, a plane taking off, a crowd surging forward.

## Prompt template
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT FROM THE EVENT], [GRAIN], epic action cinema. Image 1 is [SUBJECT A] ([key details]). Image 2 is [SUBJECT B] ([key details]). Keep both faces and outfits exact. [SUBJECTS] walk side by side toward the camera down [EMPTY STREET / CORRIDOR / RUNWAY] in slow motion while [BIG BACKGROUND EVENT] behind them. They never look back. Camera movement: low-angle tracking ONLY. The camera is at knee height, moving backward in front of them at exactly their walking speed, keeping [both / the subject] centered. Audio: [EVENT SOUND], [DETAIL SOUND], slow-motion rumble. No zoom, no cuts.
```

## Source example
```
Shot on Kodak Vision3 500T 35mm film, night, orange fire light, heavy grain, epic action cinema. Image 1 is Ramón (mustache, cream guayabera, gold chain). Image 2 is Dolores (grey hair, glasses). Keep both faces and outfits exact. Ramón and Dolores walk side by side toward the camera down an empty street in slow motion while a car explodes behind them in a huge fireball. They never look back. Camera movement: low-angle tracking ONLY. The camera is at knee height, moving backward in front of them at exactly their walking speed, keeping both centered. Audio: deep explosion boom, debris, slow-motion rumble. No zoom, no cuts.
```

## With HyperFrames
- **Live-action shot.** This move needs a generated clip. Generate it from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the event boom and the rumble in the compose prompt, with the boom tied to the moment of the event.
- **Styling in HyperFrames.** Leave the center of the frame to the heroes. Put a large title or the product name in the top third, and sync the title's entrance with the event behind them.
- **Without generation.** There is no full substitute. The closest graphic version: cut-out heroes stay still in the center, the background behind them slowly shrinks and recedes into the distance, with a flash of light from behind. Use it only if the clip can't be generated.

## Tips
- A single hero works too: drop Image 2 and replace `both` with `the subject`.
- The event must be behind them and centered, otherwise the heroes block it awkwardly.
- In 9:16, two heroes fit shoulder to shoulder; three or more need 16:9.
- A great final shot for a video, right before the logo.
