---
name: video-prompt-design
description: Writes concise, model-friendly prompts for vertical 9:16 AI short-anime video generation from approved CUT designs and keyframes.
---

# Video Prompt Design

## Core rules

- Use one primary action per clip.
- Preserve approved character identity, costume, props, environment, lighting, and composition.
- Describe actions in chronological order.
- State the camera movement clearly and keep it secondary to the main action.
- Define the final state or pose.
- Keep Japanese spoken dialogue in Japanese.
- Do not add BGM instructions.
- Do not add unapproved story events, acting, characters, or objects.

## Prompt order

1. Vertical 9:16 and visual style
2. Elements that must remain unchanged
3. Starting state
4. One primary action
5. Camera movement
6. Ending state
7. Dialogue, when required
8. Negative constraints

## AI safety rules

- Do not combine several major actions in one prompt.
- Avoid complicated hand contact, object exchange, crowds, and choreography unless essential.
- Avoid simultaneous orbit, running, facial performance, and prop handling.
- Use clear verbs and concrete visible actions.
- Avoid abstract emotional instructions without visible behavior.
- Keep motion speed appropriate to the clip duration.

## Output

Provide:

- CUT number and duration
- English video-generation prompt
- Japanese explanation of the intended motion
- Negative constraints
- Continuity requirements
- Alternate simplified prompt when generation risk is high
