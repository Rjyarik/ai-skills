---
name: "draw-architecture-building"
description: "Draw-to-build — a CGI clip in which a pencil draws the building from its floor plan or elevation, the lines rise into a structure, panels lock into place, and the finished building appears exactly as in the render. Input: floor-plan images of the house and its rendered images. The client sets the duration and the building. Use when making commercial video for social media and websites (HyperFrames, video-model prompts) when a developer, architect, builder or real-estate project needs a visual that goes from drawing to finished building."
---

# Draw-to-build (from drawing to building)

A pencil draws the building on a white sheet from its floor plan or elevation, the lines turn into a frame, panels lock into place, and the building appears exactly as it looks in the renders. It's a visual metaphor for "from idea to building": the same house travels from drawing to finished structure.

The input is images. The floor plan sets the geometry: outline, number of floors, placement of openings and balconies. The rendered images set the final look: materials, colors, light, landscape. The assembly mechanics, the order of the blocks and the "no morphing" rules stay fixed; everything else comes from the input images.

## Input
- **Floor plan (Image 1).** Used for the drawing: outlines, walls, floor slabs, openings, balconies. If the plan has several floors, each floor is a separate assembly block, built bottom to top.
- **Renders (Image 2 onward).** Used for the final look: facade, materials, glazing, roof, entrance, landscape, light and time of day. One render is the main shot; the rest clarify details.
- **Building and duration** are set by the client: a house, townhouse, tower, villa, a single block or a whole complex. Duration and the number of blocks are chosen to fit the building and the format (for example, 8, 10 or 15 seconds). Pick fractional time segments yourself to match the number of stages.
- If the plan and the renders disagree (different number of floors, different windows or balconies), don't resolve it silently. Name the mismatch and ask the client which source takes priority. By default, the plan wins for geometry and the render wins for materials.

Before generating, put together a short "building card" from the input images: number of floors, footprint shape, balconies and their placement, windows, facade materials, roof, entrance, landscape, light. This card goes into every block of the prompt so the building doesn't change from shot to shot.

## Core of the move — do not change
- **The same building from start to finish.** Floor count, balconies, windows and proportions from the card don't change from shot to shot and match the render in the final shot.
- **Rigid mechanical assembly only.** Elements extend, rotate, fold, slide and lock. No morphing, dissolves, appearing out of nowhere, particles or teleportation.
- **Every element keeps its original position and geometry.** A panel that has locked into place stays there until the end of the clip.
- **Assembly order from the base up:** first the frame and floor slabs, then walls and facade, then glazing, railings and roof.
- **The final shot looks like the render.** The hero shot repeats the render's angle and light as closely as possible.
- **Always keep the lines `NO morphing`, `no dissolves` and `No text, logos or narration`.**

## What to swap in
The building and number of floors, facade materials (from the render), shape and balconies (from the plan), location and landscape (from the render), time of day and light (from the render), paper and pencil color, duration, sound style.

## Timeline (template; the client sets the duration)
The blocks below are given as shares of the total duration, so they can be stretched or compressed. The number of stages can change too: a simple building needs 5–6 blocks, a complex may need 10 or more.

| Share of clip | What happens |
| --- | --- |
| 0–15% | Macro: a hand draws the outline and perspective from the plan. Fast transitions |
| 15–30% | Sped-up drawing of openings, balconies and joints. The camera pulls back to show the whole sketch |
| 30–40% | Lines lift off the sheet, turn into guide rails and build up the floor slabs |
| 40–50% | Balconies extend, windows slide along the rails, projections rotate, the roof unfolds |
| 50–55% | Facade panels from the render flip outward and lock in, floor by floor |
| 55–62% | Wood panels unfold, frames slot into the openings, glass panes rise out of their grooves |
| 62–68% | Railings rise, handrails join up, the entrance unfolds |
| 68–75% | Path lines become a curb, tiles assemble into a walkway, the white ground turns into the landscape from the render |
| 75–85% | Trees grow, the white surroundings fall away, the sky opens up and the camera descends to eye level |
| 85–94% | Slow push-in on the finished building |
| 94–100% | Static hero shot, as in the render |

## Prompt template
```
Generate exactly [DURATION] seconds of ultra-photorealistic [ASPECT RATIO] architectural CGI, following all storyboard frames in chronological order. Image 1 is the floor plan: build the geometry exactly from it, [FLOOR COUNT] floors, [FOOTPRINT SHAPE], [BALCONY LAYOUT], [WINDOW PATTERN]. Images 2+ are the final renders: match their [FACADE MATERIALS], [ROOF], [GLAZING], [LANDSCAPE], [LIGHT AND TIME OF DAY]. Feature ONE identical building throughout. [START %]-[END %]: [MACRO DRAWING from Image 1: tool, hand, paper, linework]. [BLOCK]: [ACCELERATED DRAWING AND PULL-BACK]. [BLOCK]: [LINES LIFT, STRUCTURE RISES, FLOOR BY FLOOR]. [BLOCK]: [BALCONIES, WINDOWS, ROOF UNFOLD INTO 3D MODEL]. [BLOCK]: [FACADE PANELS FROM RENDER FLIP AND LOCK]. [BLOCK]: [WOOD, FRAMES, GLASS INSTALLED]. [BLOCK]: [RAILINGS, HANDRAILS, CANOPY]. [BLOCK]: [PATHWAY AND GROUND TRANSFORM TO LANDSCAPE FROM RENDER]. [BLOCK]: [TREES GROW, SKY REVEALED, CAMERA DESCENDS]. [BLOCK]: [SLOW PUSH-IN TO FINISHED BUILDING]. [FINAL BLOCK]: Completely static hero shot matching Image 2 composition and light. CRITICAL: all transformations must be visible, sequential, rigid-body mechanical construction with precise extrusion, rotation, folding, sliding, assembly and locking. Every element retains its original position and geometry. NO morphing, dissolves, fades, texture blending, magical appearance, particles, teleportation or abrupt transformations. Preserve identical building proportions, floor count, windows and balconies throughout, as defined by Image 1. Dynamic macro camera during drawing, continuous three-quarter perspective during construction, smooth camera descent during landscape assembly and static final hero. Realistic mechanical physics, sharp material details, cinematic sunlight, precise construction ASMR and premium electronic soundtrack. No text, logos or narration.
```

Fill the bracketed blocks from the building card. Convert the percentages to seconds based on the chosen duration.

## Worked example (six-story building, 10 seconds)
Floor count, balconies and windows come from the plan; materials, landscape and light come from the render. Example: `six-story residential building`, `stacked balconies, angular geometry, stone facades, warm wood panels, dark metal frames and panoramic glass`.

## With HyperFrames
- **Generating the clip.** Pass the plan and renders to the video model as references (Image 1, Image 2 and onward), then generate the clip from the prompt. If the chosen model doesn't accept images as references, move the building card into the prompt text and flag it to the client: without references, geometric accuracy drops.
- **Hand HyperFrames** a direct https link to the mp4. The clip doesn't carry the sound from the prompt (the ASMR and electronic soundtrack), so add the music and pencil sounds in compose.
- **Over the clip**, the project name, floor area, number of floors or the developer's logo work well as overlays.
- **For a sequence of shots**, end the clip on the static hero shot: it's an easy point to cut to the next shot in the series.

## Tips
- One building for the whole clip. Changing floors or balconies between shots breaks the illusion of assembly.
- If the model adds elements that aren't in the plan or the render, cut the description down to 4–5 key details and repeat `Preserve identical building proportions`.
- If the assembly looks "mushy", describe the mechanics more precisely: which panels, in what order and with what motion they lock in.
- For vertical format, cut the number of blocks to 5–6 and center the building in the frame, otherwise the top or bottom gets cropped.
- If the clip came out without assembly and the building just appears, that's morphing: rewrite the assembly blocks in mechanical terms (extend, rotate, lock into place).
- If you only got a render and no plan, take the geometry from the render and tell the client explicitly that the layout may differ from the actual design.
