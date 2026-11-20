---
name: "camera-handheld"
description: "Handheld — a handheld camera with the operator running right behind the hero, live shake and jolts in the frame, documentary realism. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) that needs energy, urgency, a chase, a sense of presence or the feel of real, unstaged footage."
---

# Handheld (handheld camera following the hero)

The operator runs right behind the hero: the frame shakes and breathes, the hero keeps drifting to the edge and the camera catches up. It feels like everything is happening for real, right now. The move for urgency, chases, behind-the-scenes and reportage-style videos.

Only the camera, the effect and the action are taken from the source shot. Location, time of day, light, film look and characters are swapped in to fit the video.

## Core of the move — do not change
- The camera is in the hands of an operator running right behind the hero.
- Organic shake, a "breathing" frame, small jolts when reframing; the operator struggles to keep the hero in frame.
- The hero moves fast through a crowded place, gets past obstacles, glances back over the shoulder.
- Documentary look: 16mm, harsh natural light, heavy grain.
- Audio: footsteps, crowd voices, heavy breathing.
- Always keep the lines `handheld ONLY` and `No zoom, no cuts`.

## What to swap in
Film stock (16mm or a "documentary" look works best), light, the hero (with an Image 1 reference), a crowded location, the obstacles and what the hero knocks into, where they are rushing to, ambient sounds.

## Prompt template
```
Shot on [FILM STOCK] 16mm film, [HARSH NATURAL LIGHT], documentary realism, heavy grain. Image 1 is [SUBJECT]: keep [exact face and clothing]. [SUBJECT] runs fast through [CROWDED LOCATION], [OBSTACLE ACTIONS: shoving past ..., knocking over ...], glancing back over the shoulder. Camera movement: handheld ONLY. An operator runs right behind [SUBJECT] with organic shake, breathing, small reframing bumps, fighting to keep [SUBJECT] in frame. Audio: footsteps, [CROWD SOUNDS], heavy breathing. No zoom, no cuts.
```
Calm variant for interviews and behind-the-scenes: replace the running with `walks through` and the shake with `subtle handheld sway and breathing, gentle reframing`.

## Source example
```
Shot on Kodak Vision3 500T 16mm film, harsh midday sun, documentary realism, heavy grain. Image 1 is Ramón: keep his exact face, mustache, slicked hair, cream guayabera and gold chain. Ramón runs fast through a crowded street market, shoving past stalls, knocking over a crate of oranges, glancing back over his shoulder. Camera movement: handheld ONLY. An operator runs right behind him with organic shake, breathing, small reframing bumps, fighting to keep him in frame. Audio: footsteps, shouting vendors, heavy breathing. No zoom, no cuts.
```

## With HyperFrames
- **Live-action shot.** Generate the clip from the template in a video model and pass HyperFrames a direct https link to the mp4. The clip is inserted without sound, so request the footsteps, crowd and breathing in the compose prompt.
- **Styling in HyperFrames.** Keep titles over the shaky clip static and large: the contrast between still text and a live frame reads well. Put subtitles on a background plate.
- **Without generation.** A handheld feel can be added to a still shot or graphics: in compose, describe a slight floating offset of the frame by 6–10 px and rotation of up to 0.3 degrees with a slow "breathing" rhythm, with the frame slightly scaled up so the edges never show. Define the shake with fixed keyframes, not random numbers: the render must be identical on every run.

## Tips
- Make the obstacles specific (a crate, chairs, a clothing rack): they give the shot events.
- A glance over the shoulder creates a story: someone or something is chasing the hero (a deadline, a sale, a departing bus).
- The move is ideal for 9:16: shooting from behind fits the vertical frame naturally.
- Don't combine it with other camera moves in the same clip.
