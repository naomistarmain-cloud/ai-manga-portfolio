# AI Short Anime Studio

## Purpose

This repository contains reusable production rules and projects for AI-generated vertical short anime.

## Mandatory startup message

For every task related to short anime production in this repository, the first line of the first response must be exactly:

GitHubのリポジトリ「naomistarmain-cloud/ai-manga-portfolio」の`AGENTS.md`を更新し、短編アニメ用の自動ルーティング手順で進めています。

Display this sentence before plans, explanations, questions, file changes, or production output. Do not omit, shorten, paraphrase, or translate it.

## Automatic startup procedure

For every task related to short anime production in this repository, Codex must automatically follow this procedure. The user does not need to mention `AGENTS.md` or any Skill name.

1. Read this `AGENTS.md` before beginning the task.
2. Identify the relevant project under `ai-short-anime-studio/projects/`.
3. Read that project's README, PROJECT file, and all files marked approved or final.
4. Identify the current production phase.
5. Read and apply every relevant Skill from `.agents/skills/` before creating or changing files.
6. Preserve approved story settings, dialogue, character designs, props, locations, CUT numbers, visual direction, and continuity.
7. Do not advance into a later production phase unless the user requests it or the current phase has been approved.

If the user begins a new short-anime project without naming a Skill, start with `$vertical-short-anime-story-design`. Do not create CUTs, image prompts, or video prompts until requested.

## Mandatory rules

- Design primarily for vertical 9:16 video.
- Standard target duration is 60–90 seconds.
- Extended stories may run longer only when necessary, with an absolute maximum of 180 seconds.
- Never add scenes, dialogue, CUTs, or camera moves merely to increase duration.
- Use one primary action per CUT.
- Keep each CUT only as long as its action requires.
- Prefer visually clear storytelling over explanatory dialogue.
- Keep dialogue short and natural.
- Use compositions that remain readable on a smartphone screen.
- Design start and end images when they improve video-generation stability.
- Do not include BGM instructions in image or video generation prompts.
- Do not change approved story settings, dialogue, characters, or CUTs without explicit instruction.

## Automatic Skill routing

Codex must select and apply the relevant Skills automatically. The user does not need to type Skill names.

- Story development and restructuring: `$vertical-short-anime-story-design`
- Script-to-CUT conversion and CUT revision: `$cut-design`
- Shot size, composition, and camera movement: `$camera-direction`
- Start/end image design and image prompts: `$image-prompt-design`
- AI video motion and camera prompts: `$video-prompt-design`

When a task spans multiple phases, apply the relevant Skills in production order. Do not skip an earlier required phase or overwrite approved work.

## Language

- Production documents may be written in Japanese.
- Image and video prompts should normally be written in English.
- Spoken Japanese dialogue must remain in Japanese.
