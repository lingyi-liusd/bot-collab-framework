---
name: adversarial-peer-review
description: >-
  Use when running a harsh peer-style review on a research draft before revision
  or submission: score major/minor issues, recommend Accept/Major/Minor/Reject
  with confidence, and keep existence-level wording.
---
# Adversarial peer review

## Goal
Produce a reviewer-quality report that stress-tests claims, evidence, and venue fit. Prefer under-claiming.

## Inputs
- Manuscript paths (main tex/md + supplement + claim map)
- Venue rules (e.g. T-ITS Short ≤6 pages, abstract ≤100 words)
- Known open items (missing calib, constructive attack, etc.)

## Steps
1. Read the paper and evidence map before scoring tone.
2. List **Major (M#)** and **minor (m#)** with page/section anchors.
3. For each Major: what the authors claim · what evidence actually shows · minimal fix vs experiment needed.
4. Check forbidden escalations: safety endpoints, method novelty, generalization, causal language without design.
5. Give one recommendation: Accept / Minor / Major / Reject, lean direction, confidence /5.
6. Separate **wording fixes** (do now) from **new experiments** (need owner auth).
7. Write `adversarial_review.md` next to the pack; do not auto-revise unless the owner said so.

## Output shape
Summary (3 lines) · recommendation · Majors table · minors · claimability delta · suggested next pack version.

## Hard bans
No fake citations · no raising novelty status · no push/submit · no Goal/contract/hash edits.
