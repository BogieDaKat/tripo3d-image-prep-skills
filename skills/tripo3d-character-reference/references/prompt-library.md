# Tripo3D Character Reference Prompt Library

Use these prompts for ChatGPT Image Generation or image-to-image workflows that turn one character image into clean Tripo3D mesh creation references.

## Placeholders

`[CHARACTER DESCRIPTION]` = short description of the character.

`[SOURCE IMAGE]` = the single image uploaded as the primary character reference.

## Global Instruction

Add this to the start of every non-depth-map prompt:

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image of the same character. Preserve the character's identity, proportions, facial features, body type, hairstyle, colors, clothing design, accessories, ears, tail, prosthetics, markings, and silhouette. Do not redesign the character. Do not add extra props unless requested. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

If the image contains multiple views, multiple body parts, or a turnaround, place each view in its own invisible lane or cell with wide blank gutters between adjacent views. No part of one view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep all silhouettes completely separate, including hair, ears, horns, tail, clothing, accessories, weapons, fingers, feet, and props. If a character has long ears, a long tail, wide hair, wings, coats, skirts, weapons, or large accessories, scale all views smaller or use a wider canvas instead of allowing any contact between views.
```

## Single A-Pose Character Sheet

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image of the same character. Preserve the character's identity, proportions, facial features, body type, hairstyle, colors, clothing design, accessories, ears, tail, prosthetics, markings, and silhouette. Do not redesign the character. Do not add extra props unless requested. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Create a full-body character sheet on a white or very pale neutral background. The character must be standing in a neutral A-pose, facing directly forward, feet flat and shoulder-width apart, arms slightly away from the body, hands relaxed and visible, fingers clearly separated. The pose must be symmetrical and useful for 3D mesh generation.

Use an orthographic-style camera, no lens distortion, no foreshortening, no action pose, no dramatic perspective. Show the entire character from head to toe with nothing cropped. Make all important design details clear: face, hair, ears, clothing layers, hands, feet, tail, accessories, prosthetics, and silhouette.

High-resolution, crisp line and shape clarity, clean studio lighting, no shadows hiding details, no text, no labels, no logos, no background objects.
```

## Four-View A-Pose Turnaround

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling turnaround reference of the same character. Preserve the character's identity, proportions, facial features, body type, hairstyle, colors, clothing design, accessories, ears, tail, prosthetics, markings, and silhouette. Do not redesign the character. Do not add extra props unless requested. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Create a single image containing four full-body views of the character in neutral A-pose: front view, back view, left side view, and right side view. Place the views evenly spaced on a white or very pale neutral background.

Critical composition requirement: each full-body view must occupy its own invisible vertical lane. Leave large blank gutters between adjacent views, at least 10-15% of the full canvas width where possible. No part of any view may touch, overlap, cross into, hide behind, or visually merge with another view. Keep the front, back, left side, and right side silhouettes completely separate, including hair, ears, horns, tail, clothing, accessories, weapons, fingers, feet, and props. If long ears, a tail, wide hair, wings, coats, skirts, weapons, or accessories need extra room, make all four views smaller or use a wider canvas rather than letting the views touch.

Important: the left side and right side views must be genuinely drawn from their correct sides and must not be mirrored copies of each other. Preserve asymmetrical details accurately, including hair parting, clothing seams, straps, cybernetics, prosthetics, weapons, accessories, scars, markings, belts, pouches, ears, tail position, and any uneven design elements.

The character must stand upright in every view, feet flat, arms slightly away from the body, hands visible, fingers separated. Use an orthographic-style camera for all views, consistent scale, consistent proportions, no perspective distortion, no cropping.

No text, no labels, no logos, no shadows hiding details, no background objects. High-resolution, sharp focus, clean studio lighting, mesh-generation-friendly silhouette.
```

## Body Base with Underclothes

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image of the same character's base body. Preserve the character's identity, proportions, facial features, body type, hairstyle, colors, ears, tail, prosthetics, markings, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the character in a neutral A-pose wearing only simple tight underclothes or a plain fitted bodysuit suitable for 3D modeling. Preserve the character's true body proportions, height, body type, limb length, hand shape, feet shape, skin/fur color, markings, prosthetics, tail base, ears, and head shape. Remove outer clothing, coats, armor, hats, large accessories, belts, and loose fabric, but do not change the character's anatomy.

White or pale neutral background, full body visible, front-facing, orthographic-style camera, even studio lighting, high resolution, no perspective distortion, no text, no logos, no background objects.
```

## Outer Clothing Only

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image of the character's outer clothing as separate wearable layers. Preserve the character's identity, proportions, colors, clothing design, accessories, markings, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the outfit clearly in an A-pose on the character body, emphasizing garment construction, seams, collars, sleeves, cuffs, belts, skirts, coats, jackets, armor panels, boots, gloves, straps, buckles, and layered fabric. Keep the clothing faithful to the source image. Make the body visible enough to understand how the clothing fits, but focus on the outer garments.

White or pale neutral background, full body visible, front-facing, orthographic-style camera, high resolution, clean even lighting, no dramatic shadows, no text, no logos, no background objects.
```

## Clothing Turnaround

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a four-view turnaround focused on the character's clothing and outfit construction. Preserve the character's identity, proportions, colors, clothing design, accessories, markings, and silhouette. Do not redesign the character. Do not add extra props unless requested. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show front, back, left side, and right side views in neutral A-pose. Preserve all clothing details accurately, including asymmetrical seams, straps, buckles, belts, gloves, boots, collars, skirts, coats, armor plates, fabric layers, logos removed, and accessory placement.

Critical composition requirement: each clothing view must occupy its own invisible vertical lane. Leave large blank gutters between adjacent views, at least 10-15% of the full canvas width where possible. No clothing layer, limb, accessory, hair, tail, weapon, or silhouette may touch, overlap, cross into, hide behind, or visually merge with another view. If coats, skirts, straps, belts, weapons, sleeves, or accessories need extra room, make all four views smaller or use a wider canvas rather than letting the views touch.

The left and right side views must not be mirrored copies. Each side must show the correct side-specific details. Use consistent scale, orthographic-style camera, white or pale neutral background, high resolution, clean studio lighting, no text, no labels, no logos.
```

## Hands Close-Up

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image of the character's hands. Preserve the character's identity, hand proportions, colors, markings, prosthetics, gloves, materials, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show both hands clearly from the front/palm side and back side, with fingers spread naturally and fully visible. Preserve the character's correct number of fingers, hand proportions, nails, gloves, cybernetic prosthetics, markings, fur, skin, seams, joints, or mechanical parts. If the character has cybernetic hands, show the mechanical fingers, knuckles, wrist joints, panels, and material transitions clearly.

Arrange each hand view in its own invisible cell with clear blank space between views. No fingers, wrists, palms, gloves, claws, panels, or silhouettes may touch, overlap, cross into, or visually merge with another hand view. Scale the hands smaller or use a wider canvas if needed.

White or pale neutral background, close-up view, high resolution, sharp focus, even lighting, no shadows hiding finger details, no text, no logos.
```

## Feet / Boots Close-Up

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image of the character's feet or footwear. Preserve the exact design from the source image. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the character's boots, shoes, paws, feet, heels, soles, straps, buckles, seams, armor plates, or claws clearly. Include front, back, left side, right side, and sole/bottom views if possible.

Arrange each footwear or foot view in its own invisible cell with clear blank gutters between views. No soles, heels, toes, claws, straps, buckles, armor plates, or silhouettes may touch, overlap, cross into, or visually merge with another view. Scale the views smaller or use a wider canvas if needed.

White or pale neutral background, high resolution, sharp focus, even studio lighting, no text, no logos, no background objects.
```

## Tail Separate Mesh Reference

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image focused only on the character's tail. Preserve the tail's exact species type, length, thickness, curve, fur texture, color, markings, attachment point, and silhouette from the source image. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the tail as a separate modeling reference with front, back, left side, and right side views. Make it clear where and how the tail connects to the base of the spine or body.

Critical composition requirement: each tail view must occupy its own invisible lane or cell. Leave wide blank gutters between adjacent tail views. No part of any tail view may touch, overlap, cross into, hide behind, or visually merge with another tail view. If the tail is long, curved, fluffy, or wide, scale all views smaller or use a wider canvas rather than letting the views touch.

White or pale neutral background, orthographic-style views, high resolution, sharp focus, even lighting, no text, no labels, no logos.
```

## Long Ears / Lop Ears Separate Reference

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image focused only on the character's long ears. Preserve the exact ear type from the source image: long lop rabbit ears, length, thickness, droop, curve, inner-ear color, fur texture, markings, and how they hang beside or behind the head. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the ears in multiple orthographic-style views: front, back, left side, right side, and a slightly raised/clear view showing the ear attachment points on the head.

Make sure the ears are not cropped, tangled, fused into the hair, hidden, or merged together. They should be clearly readable as separate mesh forms connected naturally to the head.

Critical composition requirement: each ear view must occupy its own invisible lane or cell. Leave wide blank gutters between adjacent views. No ear, hair shape, head shape, attachment view, or silhouette may touch, overlap, cross into, hide behind, or visually merge with another view. If the ears are long or droop outward, scale all views smaller or use a wider canvas rather than letting views touch.

White or pale neutral background, high resolution, sharp focus, clean studio lighting, no text, no logos, no background objects.
```

## Hair Separate Mesh Reference

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image focused on the character's hair as a separate mesh element. Preserve the exact hair length, bangs, parting, layers, volume, strands, ponytails, braids, hair accessories, color gradients, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the hairstyle clearly from front, back, left side, and right side. Make sure the hair does not hide important head shape or ear attachment details.

Critical composition requirement: each hair view must occupy its own invisible lane or cell. Leave wide blank gutters between adjacent views. No hair mass, strand group, ponytail, braid, accessory, head shape, ear, or silhouette may touch, overlap, cross into, hide behind, or visually merge with another view. If the hair is wide, long, layered, or has accessories, scale all views smaller or use a wider canvas rather than letting views touch.

White or pale neutral background, orthographic-style views, high resolution, sharp focus, even lighting, no text, no labels, no logos.
```

## Hats / Head Accessories

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference image focused on the character's hat and head accessories. Preserve exact shape, size, colors, material, placement, and asymmetrical details from the source image. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the hat, headband, goggles, hair clips, flowers, horns, ribbons, jewelry, headset, mask, or other head accessories as separate modeling elements. Include front, back, left side, right side, and top views if possible.

Arrange each accessory view in its own invisible cell with clear blank gutters between views. No accessory, strap, ribbon, horn, mask edge, hair piece, or silhouette may touch, overlap, cross into, or visually merge with another view. Scale the views smaller or use a wider canvas if needed.

White or pale neutral background, high resolution, sharp focus, clean studio lighting, no text, no logos, no background objects.
```

## Head Close-Up - With Hair

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference close-up of the character's head with hair. Preserve the character's identity, face shape, eyes, nose, mouth, ears, hairline, hairstyle, eyebrows, markings, makeup, skin/fur texture, horns, cybernetics, piercings, accessories, colors, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the head and upper neck facing directly forward. Make the face centered, neutral expression, mouth closed, eyes forward.

If the character has long ears, lop ears, horns, or animal ears, include them fully and do not crop them. Make sure the ears attach correctly to the head and are not hidden by the hair.

White or pale neutral background, orthographic-style camera, high resolution, sharp focus, even studio lighting, no dramatic shadows, no text, no logos.
```

## Head Close-Up - Without Hair

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling reference close-up of the character's head without hair. Preserve the character's identity, face shape, eyes, nose, mouth, skin/fur color, markings, makeup, cybernetics, species traits, colors, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the same character's head and upper neck facing directly forward, but remove the hair so the skull shape, scalp, forehead, temples, ears, ear attachment points, horns, facial structure, and head proportions are visible.

If the character has animal ears, long ears, lop rabbit ears, horns, or other head anatomy, keep those visible and accurately attached. Do not crop the ears.

White or pale neutral background, orthographic-style camera, high resolution, sharp focus, clean even lighting, no text, no logos.
```

## Head Turnaround - With Hair

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling head turnaround of the same character with hair. Preserve the exact facial features, head shape, hairstyle, hair volume, bangs, hair parting, ears, horns, markings, makeup, cybernetics, accessories, colors, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the head and upper neck from front, back, left side, and right side views.

Critical composition requirement: each head view must occupy its own invisible vertical lane. Leave large blank gutters between adjacent views, at least 10-15% of the full canvas width where possible. No head, hair, ear, horn, neck, accessory, or silhouette may touch, overlap, cross into, hide behind, or visually merge with another view. If the character has long ears, lop ears, horns, wide hair, large hair accessories, or other extended shapes, make all four head views smaller or use a wider canvas rather than letting the views touch.

The left and right side views must not be mirrored copies. Preserve asymmetrical details correctly.

If the character has long ears or lop rabbit ears, show the full ear length in all relevant views. Make sure the ears are not cropped, hidden, fused together, or confused with hair.

White or pale neutral background, consistent scale, orthographic-style camera, high resolution, sharp focus, even studio lighting, no text, no labels, no logos.
```

## Head Turnaround - Without Hair

```text
Using [SOURCE IMAGE] as the primary character reference for [CHARACTER DESCRIPTION], create a clean 3D-modeling head turnaround of the same character without hair. Preserve the character's identity, face shape, eyes, nose, mouth, skin/fur color, markings, makeup, cybernetics, species traits, colors, and silhouette. Do not redesign the character. Use a plain white or very pale neutral background, high-resolution, sharp focus, even studio lighting, no shadows obscuring details, no dramatic pose, no perspective distortion, no text, no logos, no watermark.

Show the head and upper neck from front, back, left side, and right side views. Remove the hair so the skull shape, scalp, forehead, temples, back of head, ears, ear attachment points, horns, and facial structure are visible.

Critical composition requirement: each head view must occupy its own invisible vertical lane. Leave large blank gutters between adjacent views, at least 10-15% of the full canvas width where possible. No head, ear, horn, neck, facial profile, accessory, or silhouette may touch, overlap, cross into, hide behind, or visually merge with another view. If the character has long ears, lop ears, horns, or other extended shapes, make all four head views smaller or use a wider canvas rather than letting the views touch.

The left and right side views must not be mirrored copies. Preserve asymmetrical facial markings, cybernetics, scars, prosthetics, or ear details correctly.

If the character has long ears, lop rabbit ears, animal ears, or horns, keep them visible and accurately attached to the head. Do not crop the ears.

White or pale neutral background, consistent scale, orthographic-style camera, high resolution, sharp focus, even studio lighting, no text, no labels, no logos.
```

## Full Body Depth Map

```text
Create a depth map version of [SOURCE IMAGE], the uploaded full-body character reference image for 3D model generation.

Use the exact same character pose, camera angle, proportions, silhouette, and composition as the uploaded reference. Convert the image into a clean grayscale depth map: nearest surfaces are white, farthest surfaces are black, with smooth grayscale transitions between depths.

Preserve the full-body silhouette clearly, including hair, ears, tail, clothing layers, hands, fingers, feet, accessories, and prosthetics. Do not add texture, color, lighting effects, labels, outlines, or background objects. Use a plain black background behind the depth map. High-resolution, clean, smooth, accurate depth information.
```

## Head Depth Map

```text
Create a depth map version of [SOURCE IMAGE], the uploaded character head reference image for 3D model generation.

Use the exact same head pose, camera angle, proportions, silhouette, and composition as the uploaded reference. Convert it into a clean grayscale depth map: nearest facial surfaces are white, farthest surfaces are black, with smooth grayscale transitions.

Preserve the face, nose, eyes, lips, jawline, ears, horns, long ears, lop ears, hair volume, and neck silhouette clearly. Do not add color, texture, labels, outlines, lighting effects, or background objects. Use a plain black background. High-resolution, smooth, accurate depth information.
```

## Four-View Depth Map

```text
Create a grayscale depth map version of [SOURCE IMAGE], the uploaded four-view character turnaround.

Use the exact same front, back, left side, and right side A-pose views, preserving the same scale, proportions, pose, silhouette, and spacing. Convert each view into a clean depth map: nearest surfaces are white, farthest surfaces are black, with smooth grayscale transitions.

Critical composition requirement: preserve the same wide blank gutters and separated invisible lanes from the source turnaround. No front, back, left side, or right side depth silhouette may touch, overlap, cross into, hide behind, or visually merge with another view. If any silhouette becomes too close after conversion, scale all views smaller or use a wider canvas while preserving the exact view order and relative proportions.

Preserve readable silhouettes for hair, long ears, tail, hands, fingers, clothing layers, boots, accessories, and prosthetics. Do not add color, labels, outlines, texture, or background objects. Use a plain black background. High-resolution and mesh-generation-friendly.
```
