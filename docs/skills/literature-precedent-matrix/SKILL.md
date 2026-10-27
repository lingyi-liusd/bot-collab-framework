---
name: literature-precedent-matrix
description: >-
  Use when mapping prior work against a research claim or manuscript object:
  build a precedent × object table with abstract vs full-text grades, and never
  treat search gaps as novelty proof.
---
# Literature precedent matrix

## Goal
Produce a **precedent × project-object** comparison table for a stated proposition. Separate what was searched from what was read.

## Inputs required
- Proposition / claim IDs (C#)
- Object definition (dataset, metric, attack, control loop, venue)
- Allowed sources (arXiv, IEEE Xplore, Semantic Scholar, HF papers, local PDF folder)
- Hard bans from the project (no Goal rewrite, no fabricated citations)

## Steps
1. Write 3–5 search strings; record date, engine, and hit counts.
2. Triage hits into **candidate / related / out-of-scope**; keep a discard reason for each discard.
3. For each keep: grade **abstract-only** vs **full-text read**. Unobtained full text = `fulltext: unavailable`.
4. Fill a table with columns: prior work · venue/year · object overlap · method overlap · metric/endpoint · what they claim · what we can claim relative to them · evidence path or DOI.
5. Emit `gap` rows only as **open search gaps**, never as novelty proofs.
6. Hand the matrix + source list to the evidence seat before writing Related Work prose.

## Output paths
`evidence/<date>_lit/` with `search_log.md`, `precedent_matrix.md`, and optional PDF copies. Never overwrite a closed pack.

## Hard bans
Hit count ≠ papers read · search gap ≠ novelty · no invented citations or years · method novelty stays `NOT_ESTABLISHED` until evidence seat upgrades it.
