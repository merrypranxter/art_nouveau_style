# Art Nouveau Style Kit

A compact repository for generating Art Nouveau / Le Style Mucha-inspired images with consistent visual language.

## Repository purpose
This repo converts prior PDF context into clean, reusable markdown guidance for:
- style consistency,
- prompt generation,
- motif selection,
- and repeatable image-creation workflow.

## File map
- `STYLE_SPEC.md` — Canonical style rules and quality checklist.
- `PROMPT_PACK.md` — Ready-to-use prompt templates + negatives + iteration knobs.
- `MOTIF_DICTIONARY.md` — Motif vocabulary with symbolic intent.
- `docs/summary_*.md` — Per-source summaries of the three original context PDFs.

## Start here (new image workflow)
1. Read `STYLE_SPEC.md` to lock visual constraints.
2. Choose motifs from `MOTIF_DICTIONARY.md` that match your subject.
3. Pick a template in `PROMPT_PACK.md`.
4. Fill placeholders (`subject`, `pose`, `motifs`, `palette`, `theme`).
5. Generate an image, then refine using the iteration knobs.
6. Re-check against the style checklist in `STYLE_SPEC.md` before final export.

## Notes
The original source PDFs were archival context and have been replaced by concise canonical markdown docs for easier maintenance.
