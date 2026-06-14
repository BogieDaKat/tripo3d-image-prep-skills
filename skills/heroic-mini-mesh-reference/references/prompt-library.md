# Heroic Mini Mesh Prompt Library

Use these prompts for ChatGPT Image Generation or image-to-image workflows that turn one source image into high-resolution tabletop RPG miniature or terrain mesh references.

## Placeholders

`[SUBJECT DESCRIPTION]` = short description of the character, creature, object, or terrain.

`[SOURCE IMAGE]` = the single uploaded reference image.

## Global Miniature Instruction

Add this to every character or creature miniature prompt:

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution 3D-printable tabletop RPG miniature mesh reference. Preserve the subject's identity, silhouette, outfit, armor, weapons, accessories, anatomy, facial features, markings, colors, and original pose from the source image. Do not change the pose. Do not convert the subject to A-pose, T-pose, neutral stance, or a different action pose. Do not redesign the subject and do not add extra props unless requested.

Assume heroic-scale miniature sculpting for tabletop play: make the head, hands, feet, weapons, readable accessories, facial features, and important silhouette details slightly exaggerated for tabletop readability. Thicken wrists, ankles, fingers, horns, weapon shafts, straps, tails, cloth edges, and other fragile parts so they are durable and 3D-print-friendly. Keep forms crisp, sculptural, paintable, and suitable for a high-resolution resin mini.

Add an appropriately sized tabletop miniature base under the figure. Use a simple round or oval base unless another practical base shape is clearly needed. Size the base to the pose and footprint with a small clean margin around feet, tail contact points, cloak edges, support points, or wide stance. Keep the base low, stable, centered, and print-friendly. Do not let the base hide the feet or lower-costume details.
```

## Global Terrain Instruction

Add this to every terrain prompt:

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution 3D-printable tabletop RPG terrain mesh reference. Preserve the terrain object's identity, layout, silhouette, proportions, surface forms, readable details, damage, textures, material cues, and original composition from the source image. Do not redesign the terrain and do not add extra props unless requested.

Do not add a miniature base, character base, display plinth, or stand. Terrain should remain a terrain piece, not a based miniature. A flat underside or natural ground contact surface is allowed only when it improves printability.

Make thin details thicker and more durable for tabletop printing. Keep edges, cracks, stones, wood grain, ruins, roots, stairs, doors, cliffs, ground layers, and surface relief crisp and paintable.
```

## Multi-View Separation Rule

Add this to every turnaround or multi-view prompt:

```text
Place each view in its own invisible lane or cell with wide blank gutters between adjacent views. No part of one view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep all silhouettes completely separate, including weapons, tails, wings, horns, hair, cloaks, terrain overhangs, rocks, stairs, roots, and base edges. If any feature needs more room, scale all views smaller or use a wider canvas instead of allowing contact between views.
```

## Depth Map Eye Rule

Add this to every character or creature depth-map prompt:

```text
Keep the eyes paint-friendly in the depth map. Preserve the overall eye shape, eyelids, brow ridge, eye socket, and smooth eyeball volume, but do not render iris rings, pupils, catchlights, eye color patterns, eyelashes drawn as surface grooves, or painted eye details. Do not carve pupils or irises into the mesh. The printed eyes should be clean smooth sculpted forms that can be painted later.
```

## Miniature Front Depth Map

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution 3D-printable tabletop RPG miniature depth map. Preserve the subject's identity, silhouette, outfit, armor, weapons, accessories, anatomy, facial features, markings, colors, and original pose from the source image. Do not change the pose. Do not convert the subject to A-pose, T-pose, neutral stance, or a different action pose. Do not redesign the subject and do not add extra props unless requested.

Assume heroic-scale miniature sculpting for tabletop play: make the head, hands, feet, weapons, readable accessories, facial features, and important silhouette details slightly exaggerated for tabletop readability. Thicken wrists, ankles, fingers, horns, weapon shafts, straps, tails, cloth edges, and other fragile parts so they are durable and 3D-print-friendly. Keep forms crisp, sculptural, paintable, and suitable for a high-resolution resin mini.

Add an appropriately sized tabletop miniature base under the figure. Use a simple round or oval base unless another practical base shape is clearly needed. Size the base to the pose and footprint with a small clean margin around feet, tail contact points, cloak edges, support points, or wide stance. Keep the base low, stable, centered, and print-friendly. Do not let the base hide the feet or lower-costume details.

Create a single front-facing orthographic depth map view of the miniature. Preserve the exact pose from the source image while presenting the subject from the front for mesh generation. Do not straighten the limbs, relax the stance, or restage the action. Include the entire miniature and base with nothing cropped.

Keep the eyes paint-friendly in the depth map. Preserve the overall eye shape, eyelids, brow ridge, eye socket, and smooth eyeball volume, but do not render iris rings, pupils, catchlights, eye color patterns, eyelashes drawn as surface grooves, or painted eye details. Do not carve pupils or irises into the mesh. The printed eyes should be clean smooth sculpted forms that can be painted later.

Convert the subject, base, clothing, weapons, accessories, hair, tail, wings, and all sculptural details into a clean grayscale depth map: nearest surfaces are white, farthest surfaces are black, with smooth grayscale transitions. Use a plain black background. No color, texture, labels, outlines, text, logos, dramatic lighting, or background objects. High-resolution, sharp, smooth, mesh-generation-friendly depth information.
```

## Miniature Four-View Depth Map

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution 3D-printable tabletop RPG miniature four-view depth map. Preserve the subject's identity, silhouette, outfit, armor, weapons, accessories, anatomy, facial features, markings, colors, and original pose from the source image. Do not change the pose. Do not convert the subject to A-pose, T-pose, neutral stance, or a different action pose. Do not redesign the subject and do not add extra props unless requested.

Assume heroic-scale miniature sculpting for tabletop play: make the head, hands, feet, weapons, readable accessories, facial features, and important silhouette details slightly exaggerated for tabletop readability. Thicken wrists, ankles, fingers, horns, weapon shafts, straps, tails, cloth edges, and other fragile parts so they are durable and 3D-print-friendly. Keep forms crisp, sculptural, paintable, and suitable for a high-resolution resin mini.

Add an appropriately sized tabletop miniature base under the figure in every view. Use a simple round or oval base unless another practical base shape is clearly needed. Size the base to the pose and footprint with a small clean margin around feet, tail contact points, cloak edges, support points, or wide stance. Keep the base low, stable, centered, and print-friendly. Do not let the base hide the feet or lower-costume details.

Create a single image containing four orthographic depth map views of the miniature: front view, back view, left side view, and right side view. Preserve the exact original pose in every view. The back and side views must show the same pose from those directions, not an A-pose, T-pose, neutral stance, or newly invented pose. Preserve asymmetrical gear, weapons, scars, markings, cloak flow, straps, armor, tail, wings, and base contact points accurately.

Place each view in its own invisible lane or cell with wide blank gutters between adjacent views. No part of one view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep all silhouettes completely separate, including weapons, tails, wings, horns, hair, cloaks, and base edges. If any feature needs more room, scale all views smaller or use a wider canvas instead of allowing contact between views.

Keep the eyes paint-friendly in every depth-map view where the eyes are visible. Preserve the overall eye shape, eyelids, brow ridge, eye socket, and smooth eyeball volume, but do not render iris rings, pupils, catchlights, eye color patterns, eyelashes drawn as surface grooves, or painted eye details. Do not carve pupils or irises into the mesh. The printed eyes should be clean smooth sculpted forms that can be painted later.

Convert each view into a clean grayscale depth map: nearest surfaces are white, farthest surfaces are black, with smooth grayscale transitions. Use a plain black background. No color, texture, labels, outlines, text, logos, dramatic lighting, or background objects. High-resolution, sharp, smooth, mesh-generation-friendly depth information.
```

## Miniature Front Rendered Reference

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution fully rendered tabletop RPG miniature reference. Preserve the subject's identity, silhouette, outfit, armor, weapons, accessories, anatomy, facial features, markings, colors, and original pose from the source image. Do not change the pose. Do not convert the subject to A-pose, T-pose, neutral stance, or a different action pose. Do not redesign the subject and do not add extra props unless requested.

Assume heroic-scale miniature sculpting for tabletop play: make the head, hands, feet, weapons, readable accessories, facial features, and important silhouette details slightly exaggerated for tabletop readability. Thicken wrists, ankles, fingers, horns, weapon shafts, straps, tails, cloth edges, and other fragile parts so they are durable and 3D-print-friendly. Keep forms crisp, sculptural, paintable, and suitable for a high-resolution resin mini.

Add an appropriately sized tabletop miniature base under the figure. Use a simple round or oval base unless another practical base shape is clearly needed. Size the base to the pose and footprint with a small clean margin around feet, tail contact points, cloak edges, support points, or wide stance. Keep the base low, stable, centered, and print-friendly. Do not let the base hide the feet or lower-costume details.

Create a single front-facing orthographic rendered reference of the miniature. Preserve the exact pose from the source image while presenting the subject from the front. Do not straighten the limbs, relax the stance, or restage the action. Include the entire miniature and base with nothing cropped.

Use a plain white or very pale neutral background, high resolution, sharp focus, even studio lighting, no harsh shadows hiding details, no dramatic perspective, no text, no labels, no logos, no watermark, no background objects.
```

## Miniature Four-View Rendered Reference

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution fully rendered tabletop RPG miniature turnaround reference. Preserve the subject's identity, silhouette, outfit, armor, weapons, accessories, anatomy, facial features, markings, colors, and original pose from the source image. Do not change the pose. Do not convert the subject to A-pose, T-pose, neutral stance, or a different action pose. Do not redesign the subject and do not add extra props unless requested.

Assume heroic-scale miniature sculpting for tabletop play: make the head, hands, feet, weapons, readable accessories, facial features, and important silhouette details slightly exaggerated for tabletop readability. Thicken wrists, ankles, fingers, horns, weapon shafts, straps, tails, cloth edges, and other fragile parts so they are durable and 3D-print-friendly. Keep forms crisp, sculptural, paintable, and suitable for a high-resolution resin mini.

Add an appropriately sized tabletop miniature base under the figure in every view. Use a simple round or oval base unless another practical base shape is clearly needed. Size the base to the pose and footprint with a small clean margin around feet, tail contact points, cloak edges, support points, or wide stance. Keep the base low, stable, centered, and print-friendly. Do not let the base hide the feet or lower-costume details.

Create a single image containing four orthographic rendered views of the miniature: front view, back view, left side view, and right side view. Preserve the exact original pose in every view. The back and side views must show the same pose from those directions, not an A-pose, T-pose, neutral stance, or newly invented pose. Preserve asymmetrical gear, weapons, scars, markings, cloak flow, straps, armor, tail, wings, and base contact points accurately.

Place each view in its own invisible lane or cell with wide blank gutters between adjacent views. No part of one view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep all silhouettes completely separate, including weapons, tails, wings, horns, hair, cloaks, and base edges. If any feature needs more room, scale all views smaller or use a wider canvas instead of allowing contact between views.

Use a plain white or very pale neutral background, high resolution, sharp focus, even studio lighting, no harsh shadows hiding details, no dramatic perspective, no text, no labels, no logos, no watermark, no background objects.
```

## Terrain Front Depth Map

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution 3D-printable tabletop RPG terrain depth map. Preserve the terrain object's identity, layout, silhouette, proportions, surface forms, readable details, damage, textures, material cues, and original composition from the source image. Do not redesign the terrain and do not add extra props unless requested.

Do not add a miniature base, character base, display plinth, or stand. Terrain should remain a terrain piece, not a based miniature. A flat underside or natural ground contact surface is allowed only when it improves printability.

Make thin details thicker and more durable for tabletop printing. Keep edges, cracks, stones, wood grain, ruins, roots, stairs, doors, cliffs, ground layers, and surface relief crisp and paintable.

Create a single front-facing orthographic depth map view of the terrain piece. Preserve the source terrain's structure and composition while presenting it from the front for mesh generation. Include the entire terrain piece with nothing cropped.

Convert the terrain into a clean grayscale depth map: nearest surfaces are white, farthest surfaces are black, with smooth grayscale transitions. Use a plain black background. No color, texture, labels, outlines, text, logos, dramatic lighting, character base, or background objects. High-resolution, sharp, smooth, mesh-generation-friendly depth information.
```

## Terrain Four-View Depth Map

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution 3D-printable tabletop RPG terrain four-view depth map. Preserve the terrain object's identity, layout, silhouette, proportions, surface forms, readable details, damage, textures, material cues, and original composition from the source image. Do not redesign the terrain and do not add extra props unless requested.

Do not add a miniature base, character base, display plinth, or stand. Terrain should remain a terrain piece, not a based miniature. A flat underside or natural ground contact surface is allowed only when it improves printability.

Make thin details thicker and more durable for tabletop printing. Keep edges, cracks, stones, wood grain, ruins, roots, stairs, doors, cliffs, ground layers, and surface relief crisp and paintable.

Create a single image containing four orthographic depth map views of the terrain piece: front view, back view, left side view, and right side view. Preserve the same terrain form and composition from all directions. Preserve asymmetrical damage, openings, overhangs, roots, walls, stairs, rocks, doors, windows, and surface layers accurately.

Place each view in its own invisible lane or cell with wide blank gutters between adjacent views. No part of one view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep all silhouettes completely separate, including overhangs, rocks, stairs, roots, walls, roofs, branches, and ground edges. If any feature needs more room, scale all views smaller or use a wider canvas instead of allowing contact between views.

Convert each view into a clean grayscale depth map: nearest surfaces are white, farthest surfaces are black, with smooth grayscale transitions. Use a plain black background. No color, texture, labels, outlines, text, logos, dramatic lighting, character base, or background objects. High-resolution, sharp, smooth, mesh-generation-friendly depth information.
```

## Terrain Front Rendered Reference

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution fully rendered tabletop RPG terrain mesh reference. Preserve the terrain object's identity, layout, silhouette, proportions, surface forms, readable details, damage, textures, material cues, and original composition from the source image. Do not redesign the terrain and do not add extra props unless requested.

Do not add a miniature base, character base, display plinth, or stand. Terrain should remain a terrain piece, not a based miniature. A flat underside or natural ground contact surface is allowed only when it improves printability.

Make thin details thicker and more durable for tabletop printing. Keep edges, cracks, stones, wood grain, ruins, roots, stairs, doors, cliffs, ground layers, and surface relief crisp and paintable.

Create a single front-facing orthographic rendered reference of the terrain piece. Preserve the source terrain's structure and composition while presenting it from the front. Include the entire terrain piece with nothing cropped.

Use a plain white or very pale neutral background, high resolution, sharp focus, even studio lighting, no harsh shadows hiding details, no dramatic perspective, no text, no labels, no logos, no watermark, no character base, no background objects.
```

## Terrain Four-View Rendered Reference

```text
Using [SOURCE IMAGE] as the primary reference for [SUBJECT DESCRIPTION], create a high-resolution fully rendered tabletop RPG terrain turnaround reference. Preserve the terrain object's identity, layout, silhouette, proportions, surface forms, readable details, damage, textures, material cues, and original composition from the source image. Do not redesign the terrain and do not add extra props unless requested.

Do not add a miniature base, character base, display plinth, or stand. Terrain should remain a terrain piece, not a based miniature. A flat underside or natural ground contact surface is allowed only when it improves printability.

Make thin details thicker and more durable for tabletop printing. Keep edges, cracks, stones, wood grain, ruins, roots, stairs, doors, cliffs, ground layers, and surface relief crisp and paintable.

Create a single image containing four orthographic rendered views of the terrain piece: front view, back view, left side view, and right side view. Preserve the same terrain form and composition from all directions. Preserve asymmetrical damage, openings, overhangs, roots, walls, stairs, rocks, doors, windows, and surface layers accurately.

Place each view in its own invisible lane or cell with wide blank gutters between adjacent views. No part of one view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep all silhouettes completely separate, including overhangs, rocks, stairs, roots, walls, roofs, branches, and ground edges. If any feature needs more room, scale all views smaller or use a wider canvas instead of allowing contact between views.

Use a plain white or very pale neutral background, high resolution, sharp focus, even studio lighting, no harsh shadows hiding details, no dramatic perspective, no text, no labels, no logos, no watermark, no character base, no background objects.
```
