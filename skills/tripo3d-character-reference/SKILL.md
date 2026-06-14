---
name: tripo3d-character-reference
description: Create and refine ChatGPT Image Generation/image-to-image prompt packs that turn a single character source image into clean Tripo3D and 3D mesh modeling references. Use when the user wants character sheets, neutral A-pose references, four-view turnarounds, head/hand/feet/tail/ear/hair/clothing references, depth maps, or prompt fixes that prevent multi-view character images from touching, overlapping, or merging.
---

# Tripo3D Character Reference

## Core Workflow

Use this skill to turn one uploaded character image into mesh-generation-friendly image prompts for Tripo3D prep.

1. Confirm the user has a source image when the task depends on image-to-image. If no source image exists, ask for it or provide prompt templates using `[SOURCE IMAGE]`.
2. Ask for a short `[CHARACTER DESCRIPTION]` only when the user has not provided enough identity context. Keep it short; the uploaded image remains the primary reference.
3. Read `references/prompt-library.md` when producing, adapting, or revising prompts.
4. Preserve the source character's identity, proportions, facial features, body type, hairstyle, colors, clothing design, accessories, anatomy, ears, tail, prosthetics, markings, and silhouette.
5. Do not generate images unless the user explicitly asks for image generation. By default, provide prompts the user can paste into ChatGPT Image Generation or another image-to-image tool.

## Spacing Requirement

For any prompt that contains multiple views, multiple body parts, or a turnaround, include the prompt library's view separation language. The key requirement is:

- Place every view in its own invisible lane or cell.
- Leave wide blank gutters between adjacent views.
- Prevent every silhouette and appendage from touching, overlapping, crossing into, hiding behind, or visually merging with another view.
- If long ears, tails, hair, coats, wings, weapons, accessories, or wide clothing need more room, scale all views smaller or use a wider canvas instead of allowing contact.

This spacing rule is required for four-view body turnarounds, clothing turnarounds, head turnarounds, tail references, ear references, hair references, hands close-ups, feet/boots close-ups, accessory sheets, and four-view depth maps.

## Prompt Selection

Use the user's request to select only the needed prompts, or provide the full pack when they ask for the whole Tripo3D prep workflow.

- Start with `Single A-Pose Character Sheet` and `Four-View A-Pose Turnaround` for general full-body mesh prep.
- Use `Body Base with Underclothes` when outer clothing blocks the body silhouette.
- Use `Outer Clothing Only` and `Clothing Turnaround` when garment layers, seams, armor, straps, belts, or accessories are confusing.
- Use `Head Close-Up` and `Head Turnaround` prompts when facial identity, ears, horns, head shape, or hair attachment matter.
- Use separate `Long Ears`, `Tail`, `Hair`, `Hands`, `Feet/Boots`, and `Hats/Head Accessories` prompts when those parts distort or merge in the full-body output.
- Use depth map prompts only after a clean reference image exists; depth maps should match the uploaded/generated reference composition exactly.

## Recommended Order

For a complete Tripo3D prep set, provide prompts in this order:

1. Single front A-pose
2. Four-view full-body turnaround
3. Head close-up with hair
4. Head close-up without hair
5. Head turnaround with hair
6. Head turnaround without hair
7. Long ears or lop ears separate reference, when applicable
8. Tail separate reference, when applicable
9. Hands close-up
10. Outer clothes reference
11. Depth map versions of the best images

For lop-eared or long-eared characters, include ears in the head views and also create a separate ear reference so the ear length, droop, attachment point, and thickness remain clear.
