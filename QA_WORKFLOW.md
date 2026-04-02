# Art Nouveau QA Workflow

## 1) 100-Point Rubric (Weighted)

Use this rubric to evaluate each generation before deciding whether to iterate, branch, or discard.

| Category | Weight | What to Evaluate | Scoring Guidance |
|---|---:|---|---|
| **Composition** | **25 pts** | Overall layout coherence, focal hierarchy, negative-space control, frame integration, and visual flow from primary subject to ornament. | 0–10: unstable composition; 11–18: workable but imbalanced; 19–25: clear hierarchy, elegant flow, intentional frame-to-subject relationship. |
| **Motif Fidelity** | **25 pts** | Presence and correctness of Art Nouveau motifs: botanical arabesques, whiplash curves, stylized flora, integrated ornament, and era-typical decorative logic. | 0–10: generic or off-style motifs; 11–18: partial motif alignment; 19–25: motifs strongly recognizable and internally consistent with period style language. |
| **Line Quality** | **20 pts** | Contour confidence, rhythm of thick/thin variation, continuity of curves, and decorative line discipline. | 0–8: noisy/broken/anatomically uncertain lines; 9–14: acceptable but inconsistent; 15–20: graceful, controlled, calligraphic linework. |
| **Palette Harmony** | **15 pts** | Color-family coherence, value separation, saturation discipline, and ornament/background balance. | 0–6: clashing or muddy palette; 7–11: mostly coherent but uneven; 12–15: unified palette with deliberate accents and period-appropriate restraint. |
| **Period Plausibility** | **15 pts** | Whether the image plausibly reads as late-19th/early-20th-century Art Nouveau print/illustration rather than modern fantasy/CG styling. | 0–6: clearly modern or anachronistic; 7–11: mixed signals; 12–15: convincing period read with minimal anachronism. |

### Scoring Bands

- **90–100 (Production-Ready):** Keep; only micro-polish.
- **75–89 (Promising):** Iterate targeted weaknesses.
- **60–74 (Salvageable):** Perform structured revision pass.
- **<60 (Reset Candidate):** Recompose from earlier prompt version or new seed.

---

## 2) Failure Taxonomy

Tag failures with one or more codes to improve diagnosis speed and revision quality.

### A. Style Drift

- **FD-01 Modern-Face Drift**
  - Symptom: Contemporary beauty/photo-model facial structure, makeup, or expression language.
  - Likely Cause: Overweighting modern portrait references or realism tokens.
  - Fix: Increase stylization and period print cues; lower photorealism terms.

- **FD-02 Over-Rendered Realism**
  - Symptom: Pore-level skin detail, cinematic shading, modern lens artifacts.
  - Likely Cause: High realism defaults, excessive detail enhancers.
  - Fix: Add flat-ink/lithographic constraints; reduce hyper-detailed rendering tokens.

- **FD-03 Genre Contamination**
  - Symptom: Anime/comic/fantasy/sci-fi elements displacing Art Nouveau grammar.
  - Likely Cause: Mixed prompt priors or broad style stacks.
  - Fix: Narrow style anchors; prune conflicting genre descriptors.

### B. Ornament & Motif Problems

- **FD-04 Motif Clutter**
  - Symptom: Decorative elements compete with focal subject, causing visual noise.
  - Likely Cause: Excess ornament density without hierarchy constraints.
  - Fix: Reduce ornament count; enforce primary/secondary/tertiary decorative tiers.

- **FD-05 Weak Border Hierarchy**
  - Symptom: Frame/border exists but lacks clear dominance structure and rhythm.
  - Likely Cause: Border request too generic or under-specified.
  - Fix: Specify border anatomy (outer frame, corner medallions, inner filigree spacing).

- **FD-06 Motif Mismatch**
  - Symptom: Floral/vine forms feel botanically random or non-period.
  - Likely Cause: No motif whitelist/blacklist.
  - Fix: Constrain to a short approved motif set (e.g., iris, poppy, ginkgo, vine scrolls).

### C. Structural / Draft Issues

- **FD-07 Flattened Composition**
  - Symptom: Subject, frame, and backdrop merge into one undifferentiated layer.
  - Likely Cause: Missing depth and hierarchy instructions.
  - Fix: Explicitly assign foreground/midground/background roles.

- **FD-08 Tangent & Collision Artifacts**
  - Symptom: Lines intersect awkwardly around face, hands, or typography zones.
  - Likely Cause: Overlapping ornament without clearance rules.
  - Fix: Add spacing rules around focal anatomy and text areas.

- **FD-09 Line Incoherence**
  - Symptom: Jagged, unstable, or inconsistent contour behavior.
  - Likely Cause: Aggressive sampling/noise or poor line-priority cues.
  - Fix: Emphasize clean contour continuity and controlled line rhythm.

### D. Color & Finish Issues

- **FD-10 Palette Discordance**
  - Symptom: Accent colors overpower base palette; values collapse.
  - Likely Cause: Too many unrelated color directives.
  - Fix: Limit to 3–5 core hues plus 1 accent family.

- **FD-11 Metallic/Neon Anachronism**
  - Symptom: Chrome, neon glow, or digital bloom effects.
  - Likely Cause: Modern render vocabulary leaking into prompt.
  - Fix: Ban neon/chrome/gloss effects; add matte print finish constraints.

- **FD-12 Finish Over-Polish**
  - Symptom: Airbrushed/highly post-processed look inconsistent with period prints.
  - Likely Cause: Excessive smoothing/upscaling/stylization passes.
  - Fix: Preserve print-like texture and edge character.

---

## 3) Iteration Protocol (Order of Operations)

Always modify the system in this order to avoid confounded changes:

### Step 1 — Composition Tokens (First Intervention)

1. Adjust layout directives before any color or detail changes.
2. Lock focal hierarchy:
   - Primary subject placement
   - Frame/border dominance
   - Ornament zoning (top/sides/bottom)
3. Re-run with same seed first to isolate compositional effect.

**Do not touch palette yet.**

### Step 2 — Palette Constraints (Second Intervention)

1. Keep revised composition tokens fixed.
2. Tighten palette instructions:
   - Define core hues (3–5)
   - Define one controlled accent family
   - Set saturation/value limits
3. Re-run using prior best seed and one exploratory seed.

**Do not increase ornament complexity yet.**

### Step 3 — Ornament Density & Detail (Third Intervention)

1. Keep composition and palette constraints fixed.
2. Adjust decorative density in small increments:
   - border complexity
   - floral count
   - line filigree frequency
3. Enforce border hierarchy and clear breathing space around focal regions.
4. Stop escalating detail if rubric score stalls across two iterations.

### Escalation Rules

- If total score drops **≥10 points** after a change, revert that change and branch from prior best.
- If the same failure code appears in **3 consecutive runs**, perform a prompt refactor (not micro-edits).
- If score remains in **60–74** band for **4 runs**, reset composition with a new seed family.

---

## 4) Run Log Template

Copy this block for each generation run.

```markdown
## Run ID: YYYYMMDD-###
- **Date (UTC):**
- **Seed:**
- **Prompt Version:**
- **Model / Checkpoint:**
- **Sampler + Steps:**
- **CFG / Guidance:**
- **Resolution / Aspect Ratio:**
- **Other Settings:**

### Rubric Scores
- **Composition (25):**
- **Motif Fidelity (25):**
- **Line Quality (20):**
- **Palette Harmony (15):**
- **Period Plausibility (15):**
- **Total (100):**

### Failure Codes Observed
- [ ] FD-01 Modern-Face Drift
- [ ] FD-02 Over-Rendered Realism
- [ ] FD-03 Genre Contamination
- [ ] FD-04 Motif Clutter
- [ ] FD-05 Weak Border Hierarchy
- [ ] FD-06 Motif Mismatch
- [ ] FD-07 Flattened Composition
- [ ] FD-08 Tangent & Collision Artifacts
- [ ] FD-09 Line Incoherence
- [ ] FD-10 Palette Discordance
- [ ] FD-11 Metallic/Neon Anachronism
- [ ] FD-12 Finish Over-Polish

### Revision Notes
- **What changed this run:**
- **Why this change:**
- **Expected effect:**
- **Observed effect:**
- **Next change (following protocol order):**
- **Keep / Iterate / Reset:**
```

---

## Quick QA Checklist

- [ ] Rubric completed with numeric total.
- [ ] Failure codes tagged (at least one if score <90).
- [ ] Revision follows protocol order (composition → palette → ornament).
- [ ] Seed and prompt version recorded.
- [ ] Clear next action decided (keep / iterate / reset).
