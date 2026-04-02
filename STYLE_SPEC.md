# STYLE_SPEC.md

Canonical visual specification for generating Art Nouveau / Le Style Mucha imagery.

## 1) Visual DNA (must keep)
- Flowing **whiplash** curves and asymmetrical organic movement.
- Decorative integration of figure, border, and background motifs.
- Botanical symbolism: vines, lilies/irises/poppies, leaves, seedpods.
- Poster-era stylization: flattened shapes, elegant silhouettes, rhythmic ornament.
- Period-sensitive palette with restrained contrast and optional metallic accents.

## 2) Composition grammar
1. Establish a curvilinear gesture map.
2. Place dominant subject (often central figure or emblem).
3. Add framing architecture (halo, arch, medallion, panel border).
4. Weave secondary motifs to reinforce flow direction.
5. Apply restrained texture/patina (print-like, not photo-noise heavy).

## 3) Figure treatment
- Elongated proportions, graceful pose, serene expression.
- Hair as compositional line system (waves, spirals, strands as ornament).
- Drapery should echo curve rhythm and frame lines.

## 4) Color and material language
- Preferred families: sage, olive, muted teal, burgundy, ochre, cream, umber.
- Keep highlights selective; avoid modern neon unless intentionally stylized.
- Surface feel: lithographic/poster print or softly aged paper.

## 5) Hard constraints
- Avoid photorealistic lighting and hyper-sharp CGI aesthetics.
- Avoid random modern UI/iconography unless translated into period ornament.
- Avoid clutter: every ornament must support flow or symbolism.

## 6) Quality checklist
- Does the eye follow a continuous curve path?
- Are motifs nature-derived and stylistically coherent?
- Is typography (if any) integrated into ornament system?
- Does the piece read as period-inspired rather than generic fantasy?
## Purpose
This document defines a **model-agnostic visual grammar** for generating or evaluating Art Nouveau imagery with high fidelity to the late-19th/early-20th-century poster tradition and specifically to **Mucha-like** compositional logic.

Use this as a production spec, prompt scaffold, and QA rubric.

---

## 1) Visual Pillars

### 1.1 Line
- Prioritize flowing, calligraphic contour lines with controlled taper.
- Use line hierarchy:
  - Primary contour for silhouette and major drapery arcs.
  - Secondary line for hair strands, botanical veins, and jewelry filigree.
  - Tertiary micro-line only for texture accents.
- Curves should feel continuous and rhythmic; abrupt angular breaks are rare and intentional.
- Enclose major forms with confident outlines; avoid sketchy, broken comic inking.

### 1.2 Silhouette
- Readability at thumbnail scale is mandatory.
- Figure silhouette should be elegant, elongated, and balanced around a central vertical axis.
- Hair mass and drapery must contribute to silhouette rhythm (S-curves, crescents, plume-like expansions).
- Negative space should be designed, not incidental.

### 1.3 Ornament
- Ornament is structural, not pasted on: it should lock into pose, halo geometry, and border.
- Repetition with variation: recurring motifs (petals, whiplash curls, bead chains) with slight transformations.
- Symmetry is often approximate or bilateral with organic drift.

### 1.4 Palette
- Prefer restrained historical palettes:
  - Warm creams, parchment, muted ochres, dusty rose, olive/sage greens, soft teal, terracotta, antique gold.
- Keep saturation moderate; reserve high chroma for focal accents.
- Use harmonized analogous clusters rather than modern neon complements.
- Limit total key hues to preserve poster coherence.

### 1.5 Lighting
- Flat-to-gently-modeled tonal treatment; avoid cinematic high-contrast realism.
- Luminous but diffuse lighting; no hard specular hotspots unless in jewelry accents.
- Form is described by value transitions and line, not photoreal rendering.

### 1.6 Texture
- Surface should evoke printmaking/lithographic character:
  - Subtle grain, paper tooth, slightly irregular fill edges.
- Avoid hyper-detailed skin pores, lens noise, or 3D material realism.
- Texture density should never overpower line clarity.

### 1.7 Typography Treatment
- Typography is integrated into composition architecture (cartouche, arch, ribbon, panel header).
- Letterforms should feel period-compatible: decorative serif or stylized display forms.
- Type is subordinate to figure, but visually bonded through line weight and ornament.
- Text blocks should align to geometric anchors (arc, column, centered axis).

### 1.8 Framing
- Frame and image are interdependent.
- Use borders, medallions, arches, and compartmental panels to organize narrative.
- Outer frame weight should contain ornament without boxing it into rigidity.
- Circular/oval nimbus structures should support head placement and hierarchy.

---

## 2) Distinction Rules: Art Nouveau vs Generic Vintage Poster

### 2.1 Must Include
- Whiplash line dynamics and vegetal arabesque flow.
- Integration of figure + ornament + frame as one system.
- Stylized botanical motifs (not generic floral clip art).
- Controlled decorative flattening with deliberate contour emphasis.
- Halo/medallion or equivalent radial geometry around the primary subject.
- Historic poster-like value control (readable masses, restrained contrast).

### 2.2 Must Avoid
- Purely retro pin-up styling without botanical structural motifs.
- Deco-only geometry (hard zigzags, chrome streamlining) replacing organic flow.
- Photorealistic rendering pipelines (camera blur, HDR, lens flare, pores).
- Random Victorian clutter lacking motif grammar.
- Grunge distress overlays that obscure contour hierarchy.
- Generic “vintage filter” color grading without line/ornament discipline.

---

## 3) Motif Grammar

### 3.1 Halos (Nimbus Systems)
- Role: establish sanctified focal hierarchy and rhythmic center.
- Preferred constructions:
  - Concentric circles with alternating ornamental bands.
  - Sunburst petal rings.
  - Coin-like medallion with bead or laurel perimeter.
- Placement: centered or slightly elevated behind head; tangent control with hair mass is intentional.
- Constraints:
  - Must not overpower facial readability.
  - Ring spacing should be even or intentionally graduated.

### 3.2 Arabesques
- Build with long, continuous spline-like paths.
- Origin points should be anchored to frame corners, shoulders, or botanical stems.
- Use mirrored echoes sparingly to avoid mechanical repetition.
- Terminal forms: tendril curls, leaf tips, bead knots, petal hooks.
- Rule of flow: at least one major arabesque should guide eye back to face.

### 3.3 Botanical Forms
- Prefer species-implied stylization (iris, lily, poppy, chrysanthemum-like masses, ivy, vine).
- Botanical anatomy should be simplified but plausible:
  - Clear stem logic, leaf attachment, petal layering.
- Use plants as compositional vectors:
  - Vertical stems for stability.
  - Arcing vines for rhythm.
- Avoid random bouquet scatter with no directional logic.

### 3.4 Jewelry
- Jewelry should echo motif language (filigree curls, pearls, enamel-like insets).
- Typical forms:
  - Pendants, tiaras, chokers, drop earrings, brooches.
- Material cues are graphic (line + flat highlight), not photoreal metallic.
- Place jewelry at rhythm nodes: throat, brow, sternum, wrist.

### 3.5 Drapery
- Drapery lines should harmonize with hair and arabesques.
- Folds are broad and lyrical rather than sharply faceted.
- Use drapery to create directional sweeps into focal areas.
- Avoid chaotic micro-fold realism.

### 3.6 Border Architecture
- Border types:
  - Rectilinear frame with rounded internal corners.
  - Arch-top poster frame.
  - Circular medallion enclosure.
  - Multi-panel vertical scaffold.
- Include modular ornament bands (beads, floral repeats, ribbon tracery).
- Structural hierarchy:
  - Outer containment line.
  - Mid ornamental band.
  - Inner image window.
- Border should guide visual entry and exit, not merely decorate margins.

---

## 4) Composition Templates

### 4.1 Bust Portrait Template
- Camera/framing:
  - Subject framed from chest to head.
  - Eye line near upper third.
  - Mildly frontal or 3/4 turn; avoid extreme perspective.
- Required supports:
  - Halo/nimbus behind head.
  - Hair mass expanding laterally into ornament field.
  - Upper border typography compartment.
- Use when emphasizing face, hair design, and symbolic flora.

### 4.2 Full-Figure Panel Template
- Camera/framing:
  - Full body within a tall vertical panel.
  - Slightly low or neutral viewpoint; avoid dramatic foreshortening.
- Body flow:
  - Contrapposto or gentle sway to generate S-curve.
  - Drapery and vines should extend movement across full height.
- Architecture:
  - Side columns or vertical ornament rails.
  - Base motif pedestal (floral or emblematic).

### 4.3 Circular Medallion Template
- Camera/framing:
  - Subject centered in circular crop; bust or half-figure.
  - Tangent discipline at circle edge (no accidental clipping).
- Ornament:
  - Ringed border with repeated motifs.
  - Radial motifs must be evenly distributed with minor hand-made variance.
- Ideal use: emblematic portrait, symbolic season/month allegories.

### 4.4 Triptych Panel Template
- Camera/framing:
  - Three vertically aligned compartments (or three adjacent narrow panels).
  - Central panel dominates; flanking panels support theme.
- Figure logic:
  - Either one figure in center + motifs/secondary figures on sides,
    or thematic progression across all three.
- Cohesion constraints:
  - Shared palette across panels.
  - Repeated motif family with controlled variation.
  - Border system unifies all panels as one artifact.

---

## 5) Mucha Fidelity Checklist (Pre-Acceptance Scoring)

Score each item 0, 1, or 2:
- **0** = missing/incorrect
- **1** = partially present
- **2** = strongly present

Maximum score: **40** (20 items).
Suggested acceptance threshold: **32+**, with no critical failures.

### 5.1 Core Form & Line
1. Contour lines are fluid, intentional, and hierarchically weighted.
2. Silhouette reads clearly at small scale.
3. Hair and drapery contribute to overall rhythmic flow.
4. Figure pose avoids stiff mannequin symmetry unless deliberately iconic.

### 5.2 Ornament Integration
5. Ornament is compositionally integrated (not sticker-like).
6. Halo/nimbus geometry supports focal hierarchy.
7. Arabesques guide eye movement toward the face/focal point.
8. Border architecture and interior motifs are stylistically unified.

### 5.3 Motif Fidelity
9. Botanical motifs are stylized yet anatomically plausible.
10. Jewelry echoes the same ornamental grammar.
11. Drapery folds are lyrical and coherent with line language.
12. Motif repetition includes variation rather than copy-paste sameness.

### 5.4 Color & Light
13. Palette is restrained, harmonized, and period-appropriate.
14. Contrast supports readability without modern cinematic extremes.
15. Lighting remains diffuse/graphic rather than photoreal.
16. Accent colors are used intentionally at focal nodes.

### 5.5 Print-Like Surface & Type
17. Texture suggests lithographic/paper character without noise overload.
18. Typography (if present) is period-compatible and structurally placed.
19. Edges/fills preserve a crafted poster feel, not digital airbrush realism.
20. Overall piece reads as Art Nouveau first, not generic “vintage.”

### Critical Failure Flags (auto-reject)
- Photoreal face/render pipeline dominates line/ornament language.
- No halo/medallion/focal geometry and no equivalent Art Nouveau structural substitute.
- Deco/modernist hard geometry displaces organic whiplash flow.
- Border/ornament disconnected from the figure and composition.

---

## 6) Practical Usage Notes
- For generation: use pillars + motif grammar + one composition template + checklist.
- For review: score with checklist before acceptance.
- For iterative correction: target the lowest-scoring sections first (usually line hierarchy, halo integration, and palette restraint).
