---
name: image-prompt-design
description: Creates consistent start-image and end-image prompts for vertical 9:16 AI short-anime CUTs.
---

# Image Prompt Design

## Purpose

Design stable keyframes that give an AI video model a clear starting pose, composition, identity, and reachable final state.

## Start image rules

- Show the moment immediately before the CUT's primary action.
- Use a stable, readable pose.
- Preserve approved character identity, age, face, hair, costume, props, and environment.
- State vertical 9:16 composition and shot size.
- Leave visible space for the intended movement.
- Avoid depicting the action as already completed.

## End image rules

- Show the clear state after the primary action finishes.
- Keep the location, lighting, costume, and character identity consistent with the start image.
- Make the final pose physically reachable from the start image.
- Prepare a composition that connects naturally to the next CUT when applicable.

## Prompt order

1. Vertical 9:16 and visual style
2. Character identity and fixed design
3. Location, time, weather, and lighting
4. Camera and composition
5. Pose, expression, gaze, and prop state
6. Continuity requirements
7. Exclusions

## Exclusions

Unless explicitly required, exclude:

- readable text
- subtitles
- watermarks
- extra people
- duplicate body parts
- altered costume
- altered hairstyle or hair color
- unrequested objects
- motion trails or trajectory lines

## Deliverables

For each required image provide:

- Japanese design summary
- English generation prompt
- Continuity checklist
- Known generation risks
