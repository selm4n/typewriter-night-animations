# Typewriter night animations

A minimal collection of self-typing typewriter illustrations. A front-facing machine quietly writes by itself late at night: a little mechanical rhythm, an unfinished page, and a crescent moon. Single-color SVG line art on a transparent background.

## Preview
Open index.html for all three live scenes. Each card links to a standalone demo. Dark line, Light line and Muted ink demonstrate inherited color; Pause motion freezes the scenes. No installation or build step is required.

| Variation | Motion | Loop | Placement |
| --- | --- | --- | --- |
| [Steady Typing](01-steady-typing/index.html) | Gentle key presses, typebar strokes and small paper movement | 8s | Hero or section |
| [Pause & Think](02-pause-and-think/index.html) | A short phrase, a long quiet pause, then renewed typing | 9s | Quiet editorial placement |
| [Carriage Return](03-carriage-return-loop/index.html) | Typing, a brief pause, a restrained carriage return | 8s | Divider or footer |

## Embed
Copy figure.typewriter-animation from a standalone demo and the component CSS before the Demo presentation comment. Retain its variation class. All three stylesheets contain identical component rules; include them once. The gallery has inline previews. No JavaScript, external dependencies, image files, embedded fonts, or SVG IDs are used.

## Color and size
The drawing uses currentColor throughout. For example:

    .typewriter-animation { color: #1f1f1f; max-width: 600px; }

Set width or max-width on the figure or its parent. The 600 × 400 viewBox, explicit SVG dimensions and 3:2 aspect ratio preserve the composition at approximately 180–900px. There is no fixed screen positioning.

## Composition and transparency
The typewriter faces the viewer, with a broad keyboard, visible roller and upright paper. Abstract strokes suggest writing without readable content. The small moon is the only night cue. There are no people, desks, chairs, or room scenery. Every interior remains transparent: no background-colored masks, fills, gradients, shadows or textures. Preview backgrounds belong only to the demo wrappers.

## Motion and accessibility
CSS keyframes animate a few keys, a small typebar and paper details. Pauses separate the gestures. The carriage-return variation moves the paper and roller together while keeping the keyboard stationary. Change --twn-duration to adjust the full timeline.

prefers-reduced-motion:reduce disables all animation and retains the static drawing. Keep the accessible figure label when meaningful; for decorative use, remove role and aria-label and add aria-hidden="true". Demo color and pause controls are native inputs driven by scoped CSS :has().
