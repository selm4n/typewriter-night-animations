# Carriage Return

A front-facing typewriter types by itself, returns its paper carriage, and begins another quiet line. The quiet, literary mood comes from the machine's small movements and one crescent moon.

## Files and preview
- index.html — standalone demo and inline SVG.
- style.css — scoped component rules followed by demo presentation.
- README.md — usage notes.

Open index.html directly in a modern browser. No JavaScript, dependencies, embedded fonts, images, server or build step are required.

## Reuse
Copy figure.typewriter-animation and the CSS before the Demo presentation comment. Keep its variation class. The component rules are shared across all three folders; include them once. No SVG IDs or external resources are used.

## Customize
Set color on the figure or its parent; every line inherits currentColor. Set width or max-width to fit the container. Intrinsic 600 × 400 dimensions and a 3:2 aspect ratio preserve the drawing at 180–900px. Set --twn-duration to change the complete 8-second loop.

The reusable scene is transparent. It consists only of a front-facing typewriter, visible paper with abstract marks, and a small moon. Preview surfaces are separate. The full keyboard and roller are visible; no human figure, furniture or room is included.

## Accessibility
prefers-reduced-motion:reduce stops all key, paper and carriage movement and retains the complete static drawing. Native demo controls pause motion and change the inherited color. For purely decorative use, replace the figure's role and aria-label with aria-hidden="true".

## Writing rhythm
Four short, abstract strokes reveal progressively using normalized SVG path lengths and CSS stroke-dashoffset. The reflective variant holds an extended pause before the last phrase. Only these new marks fade at the end; they reset while invisible, keeping the machine and page continuously visible. Reduced motion displays every stroke immediately. The small crescent is secondary to the machine.
