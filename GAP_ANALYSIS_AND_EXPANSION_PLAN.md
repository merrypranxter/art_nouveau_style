# Gap Analysis & Expansion Plan (Art Nouveau / Mucha Kit)

This document captures what was under-specified and breaks upgrades into small, shippable tasks.

## Observed Gaps

1. **Prompt architecture lacked strict token ordering**
   - Existing templates were strong, but they did not enforce a consistent prompt slot order for reproducibility across teams.

2. **Insufficient subject-specific variants**
   - Portrait/poster templates existed, but there were no dedicated mini-grammars for product ads, tarot cards, book covers, album art, and branding lockups.

3. **Typography details were minimal**
   - Prior docs referenced typography compatibility but did not define title/subtitle/caption hierarchy, tracking, ornaments around glyphs, or spacing rules.

4. **Gesture and anatomy stylization were not formalized**
   - Figure guidance existed, but not body-ratio targets, hand pose archetypes, or profile angle constraints.

5. **No explicit anti-drift repair recipes**
   - We had failure codes, but not fast “if X appears, patch with Y” intervention snippets.

6. **No layout blueprint dimensions**
   - Composition templates did not include practical percentage bands (header, figure zone, footer cartouche, breathing margins).

7. **No production packaging checklist**
   - Export/print prep existed at high level but not a compact preflight sequence for batch production.

## Expansion Tracks (Small Tasks)

### Track A — Prompt Precision
- A1: Add canonical prompt slot syntax and order rules.
- A2: Add domain-specific mini templates (tarot, label, cover, poster ad).
- A3: Add micro-variation controls (line, motif density, finish).

### Track B — Visual Systems
- B1: Add typography system guide.
- B2: Add composition blueprints with zone percentages.
- B3: Add figure/anatomy stylization table.

### Track C — QA & Repair
- C1: Add failure-to-fix quick patch library.
- C2: Add run triage matrix (when to iterate, fork, or reset).
- C3: Add batch preflight checklist.

### Track D — Ops Workflow
- D1: Add task board with granular work packets.
- D2: Add “definition of done” for each packet.
- D3: Add cadence suggestion for iterative pushes.

## Recommended Push Cadence
- Keep each push to **1–2 packets** maximum.
- Run QA rubric after each packet.
- Do not mix composition changes with palette changes in the same packet.
