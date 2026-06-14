# Tripo3D Image Prep Skills

Codex skills for creating image-generation prompts that turn character, creature, and tabletop terrain references into cleaner image inputs for 3D mesh workflows.

These skills do not create 3D objects directly. They help prepare reference images, turnarounds, rendered miniature sheets, and depth-map prompts that can be used with tools such as Tripo3D or other image-to-3D workflows.

## Included Skills

### `tripo3d-character-reference`

Creates prompt packs for clean character reference images intended for 3D mesh generation.

It supports:

- Single full-body A-pose character sheets.
- Four-view A-pose turnarounds.
- Body base, clothing, hands, feet, tail, long ears, hair, head, and accessory references.
- Depth-map prompt variants.
- Strong spacing rules so turnaround views do not touch or visually merge.
- Preservation of identity, proportions, clothing, accessories, markings, ears, tails, prosthetics, and silhouette from the source image.

### `heroic-mini-mesh-reference`

Creates prompt packs for tabletop RPG miniatures and terrain mesh references.

It supports:

- Heroic-scale tabletop mini styling.
- Pose-preserving front views and four-view turnarounds.
- Character and creature minis with appropriately sized tabletop bases.
- Terrain references without miniature bases.
- Depth maps by default for mesh detail.
- Optional rendered references when requested.
- Paint-friendly depth-map eyes that preserve eye shape without carving iris or pupil detail into the mesh.

## Installation

Clone this repository, then copy the skill folders into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R skills/* ~/.codex/skills/
```

Restart Codex or open a new Codex session so the skills can be discovered.

## Usage

Invoke a skill by name in Codex.

Example:

```text
Use $tripo3d-character-reference to create a four-view character turnaround from my uploaded image.
```

Example:

```text
Use $heroic-mini-mesh-reference to create depth-map prompts for a heroic-scale tabletop mini from my uploaded character image.
```

For the heroic mini skill, ask for `rendered` if you want both rendered references and matching depth-map prompts:

```text
Use $heroic-mini-mesh-reference to create rendered and depth-map turnaround prompts for this character.
```

## Repository Layout

```text
skills/
  heroic-mini-mesh-reference/
    SKILL.md
    agents/openai.yaml
    references/prompt-library.md
  tripo3d-character-reference/
    SKILL.md
    agents/openai.yaml
    references/prompt-library.md
```

Each skill is self-contained. `SKILL.md` contains the workflow instructions Codex loads when the skill is used, while `references/prompt-library.md` contains the longer reusable prompt library.

## Notes

- These skills are designed for image-to-image workflows using a single uploaded source image as the primary reference.
- Generated outputs should be reviewed before being used for mesh generation or 3D printing.
- Results may need iteration, especially for asymmetrical outfits, non-human anatomy, complex accessories, or unusual poses.
- Make sure you have the rights to use any character art or reference images you upload.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
