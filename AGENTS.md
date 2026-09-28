# AGENTS.md

## Project snapshot

This repository is a static HTML5 Canvas learning game for children. It teaches English tense meaning through spatial, motion-based cues and simple yes/no concept-checking questions.

- Primary files: [index.html](index.html), [style.css](style.css), [script.js](script.js)
- Curriculum and design references: [README.md](README.md), [docs/master_prompt.md](docs/master_prompt.md)
- Supporting lesson plans: [docs/lesson1_plan.md](docs/lesson1_plan.md), [docs/lesson2_plan.md](docs/lesson2_plan.md), [docs/lesson3_plan.md](docs/lesson3_plan.md)

## Core design principles

- Context comes before rules: the learner should be placed in the visual scene before the target sentence or grammar explanation appears.
- Use a 5-year-old vocabulary level. Avoid grammatical jargon. Prefer child-friendly phrasing such as “going bye-bye,” “just left,” and “still moving.”
- Keep all visuals procedural and canvas-based. Do not import external images or textures.
- Use the animation loop as the source of truth for state transitions, collisions, and temporal boundaries.
- Treat the Web Audio API like a synchronized teaching signal: trigger sound changes immediately with the physics state change.

## Technical guardrails

- Rendering must happen in the canvas frame loop using raw drawing commands such as `fillRect`, `arc`, `lineTo`, and simple gradients.
- `AudioContext` must be created only after the user clicks the start button; do not initialize audio on page load.
- Keep all state transitions deterministic and physically grounded. When a boundary is crossed, update audio and visuals in the same frame.
- Use simple, reliable browser behavior: this is a static app, not a framework project.
- Prefer small, focused JS changes in one file unless a new module is clearly needed.

## How to work in this repo

- For local testing, open [index.html](index.html) in a browser. The app is intentionally static and does not require a build step.
- If you need to debug behavior, use browser devtools and focus on the animation loop, state transitions, and synthesizer graph in [script.js](script.js).
- If you are modifying pedagogy, check [docs/master_prompt.md](docs/master_prompt.md) and the lesson-specific docs before changing wording or game flow.
- Preserve the existing child-friendly tone and avoid technical grammar explanations in UI strings.

## Acceptance checklist for changes

Before finishing work in this repository, confirm that:

- The app still runs as a single-page canvas experience without external assets.
- Audio remains gated behind the start interaction.
- Visual state changes and sound cues stay synchronized in the same frame.
- Text remains easy for a native 5-year-old child to understand.
- Any new behavior aligns with the lesson plan and the “Tense Edge” teaching model.

## Helpful defaults

- Keep drawing commands concise and declarative.
- Favor clear object names and small state updates over abstraction layers.
- Do not add libraries or build tooling unless the task specifically requires it.

## Sources of truth

- [README.md](README.md): project overview and run instructions
- [docs/master_prompt.md](docs/master_prompt.md): pedagogy and lesson design
- [docs/lesson1_plan.md](docs/lesson1_plan.md) / [docs/lesson2_plan.md](docs/lesson2_plan.md) / [docs/lesson3_plan.md](docs/lesson3_plan.md): detailed lesson behavior and intent
