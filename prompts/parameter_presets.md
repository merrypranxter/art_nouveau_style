# Parameter Presets by Model Family (Art Nouveau)

These are starting points; tune by subject complexity and model behavior.

## SDXL (base + optional refiner / modern checkpoints)

### Portrait
- **CFG**: 5.0–6.5
- **Steps**: 30–45
- **Sampler**: DPM++ 2M Karras (or equivalent)
- **Resolution**: 1024×1280 or 832×1216
- **Aspect Ratio**: 4:5 or 2:3
- **Stylization strategy**: Strong style tokens in positive prompt, medium-length negative prompt.

### Poster / Decorative Panel
- **CFG**: 6.0–7.5
- **Steps**: 35–50
- **Resolution**: 1024×1536 (poster), 1024×1024 (panel)
- **Aspect Ratio**: 2:3, 3:4, or 1:1
- **Notes**: Use explicit "reserved text cartouche" language for cleaner text zones.

### Allegorical Scene
- **CFG**: 5.5–7.0
- **Steps**: 40–55
- **Resolution**: 1216×832 or 1344×768
- **Aspect Ratio**: 3:2 or 16:10
- **Notes**: Increase steps if symbol density is high.

---

## Midjourney (v6+ style workflows)

### General Prompt Controls
- **Stylize (`--stylize`)**: 250–750 for decorative richness
- **Chaos (`--chaos`)**: 0–12 (keep low for consistency)
- **Quality (`--quality`)**: 1 (or 2 for final passes)
- **Weird (`--weird`)**: 0–20 (optional experimentation)

### Suggested Ratios
- Portrait: `--ar 4:5`
- Poster: `--ar 2:3`
- Panel: `--ar 3:4` or `--ar 1:1`
- Scene: `--ar 16:10` or `--ar 3:2`

### Prompt Pattern
`[subject + motif], Art Nouveau, flowing arabesque lines, decorative lithograph poster aesthetics, [palette], [ornament controls] --stylize 500 --ar 2:3 --chaos 5`

---

## Flux-like Workflows (Flux, guidance-distilled models, node-based UIs)

### Baseline
- **Guidance / CFG-equivalent**: 2.5–4.5
- **Steps**: 20–36 (often fewer needed than SDXL)
- **Resolution**: Start 1024-long-edge, upscale later
- **Aspect Ratio**: Match motif (portrait 4:5, poster 2:3, panel 1:1/3:4)

### Practical Notes
- Flux-like models often respond better to concise prompts with strong nouns/adjectives.
- Keep negatives short and high-impact.
- If ornament collapses, add one explicit structure phrase: `"ornamental border with floral repeats"`.

---

## Cross-Model Tuning Heuristics

- **Too realistic?** Lower realism terms, raise stylization language, add flat-tone and lithograph cues.
- **Too busy?** Reduce symbol count and limit palette to 3–4 anchors.
- **Too flat/boring?** Add one depth cue (foreground vines, midground figure, halo background).
- **Inconsistent faces/hands?** Reduce complexity and generate portrait + ornament in two passes.
