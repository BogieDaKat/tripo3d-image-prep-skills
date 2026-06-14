---
name: heroic-mini-mesh-reference
description: Create and refine prompt packs for high-resolution tabletop RPG miniature and terrain mesh references from a single source image. Use when the user wants heroic-scale miniatures, 3D-printable mini depth maps, pose-preserving front views, pose-preserving front/back/left/right turnarounds, bases added to character or creature minis, terrain references without bases, paint-friendly eye handling on depth maps, or help using this tabletop mini mesh prompt workflow.
---

# Heroic Mini Mesh Reference

## Core Workflow

Use this skill to create image-generation prompts for high-resolution tabletop RPG miniatures and terrain meshes.

1. Confirm the user has a source image when the task depends on image-to-image. If no source image exists, ask for it or provide templates using `[SOURCE IMAGE]`.
2. Ask for a short `[SUBJECT DESCRIPTION]` only when the user has not provided enough identity context. Keep it short; the uploaded image remains the primary reference.
3. Determine whether the subject is a character/creature miniature or terrain.
4. Read `references/prompt-library.md` when producing, adapting, or revising prompts.
5. Preserve the source image pose. Do not convert characters to A-pose, T-pose, neutral stance, or a new action pose.
6. Default to depth-map prompts unless the user asks for `rendered`, `full render`, `beauty render`, or similar. If rendered is requested, provide both a rendered reference prompt and a matching depth-map prompt.
7. Do not generate images unless the user explicitly asks for image generation. By default, provide prompts the user can paste into ChatGPT Image Generation or another image-to-image tool.

## Heroic Scale Rules

Assume tabletop heroic scale for character and creature minis unless the user specifies another scale.

- Exaggerate heads, hands, feet, weapons, readable accessories, facial features, and silhouette enough to read clearly on the tabletop.
- Make wrists, ankles, weapon shafts, horns, fingers, thin cloth, tails, straps, and fragile extensions thicker and more printable.
- Keep the character's identity, costume, proportions, pose, and silhouette recognizable from the source image.
- Avoid true-scale fragility. Favor durable sculpting, clean forms, and paintable surface separation.
- Do not add extra props or redesign the character unless the user asks.

## Base Rules

For character or creature miniatures, add an appropriately sized tabletop miniature base.

- Use a simple round or oval base unless the source image clearly calls for a different practical base shape.
- Size the base to the figure's footprint and pose, with a small clean margin around feet, tail contact points, cloak edges, or support points.
- Keep the base low, stable, centered, and print-friendly. Do not let it hide important feet, paws, hooves, or lower-costume details.
- Add a flight stem or support only when needed to preserve the original pose.

For terrain, do not add a miniature base, plinth, display stand, or character base. Terrain may have a flat underside or natural ground contact surface only when useful for printing.

## Depth Map Eye Rules

For character or creature depth maps, keep eyes paint-friendly.

- Preserve the overall eye shape, eyelids, brow ridge, eye socket, and smooth eyeball volume.
- Do not include iris rings, pupils, catchlights, eye color patterns, eyelashes drawn as surface grooves, or painted eye details in the depth map.
- Do not carve pupils or irises into the mesh. The printed eye should be a clean sculpted surface that can be painted later.
- Rendered reference prompts may still show iris and pupil color; this restriction is only for depth maps.

## View Rules

For character or creature minis, produce:

- A single front view preserving the original pose.
- A four-view turnaround showing front, back, left side, and right side while preserving the original pose in every view.

For terrain, produce the same front view and four-view turnaround structure, but without a base.

For every multi-view output, place each view in its own invisible lane or cell with wide blank gutters. No view may touch, overlap, hide behind, or visually merge with another view. Scale views smaller or widen the canvas if weapons, tails, wings, cloth, terrain overhangs, or silhouettes need room.

## User Help

When the user asks how to use this skill, give a concise answer like:

```text
Upload one reference image and tell me whether it is a character/creature mini or terrain. By default I will make depth-map prompts for a single front view and a front/back/left/right turnaround. Character and creature minis keep the original pose, get heroic-scale print-friendly proportions, and receive an appropriately sized base. Terrain keeps the original form and does not get a base. Ask for "rendered" if you want both fully rendered reference prompts and matching depth-map prompts.
```

## Output Selection

Use only the needed prompts unless the user asks for the full set.

- Default character/creature mini: `Miniature Front Depth Map` and `Miniature Four-View Depth Map`.
- Rendered character/creature mini: add `Miniature Front Rendered Reference` and `Miniature Four-View Rendered Reference`, then provide matching depth-map prompts.
- Default terrain: `Terrain Front Depth Map` and `Terrain Four-View Depth Map`.
- Rendered terrain: add `Terrain Front Rendered Reference` and `Terrain Four-View Rendered Reference`, then provide matching depth-map prompts.
