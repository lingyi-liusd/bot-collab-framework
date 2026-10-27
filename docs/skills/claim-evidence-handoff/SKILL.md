---
name: claim-evidence-handoff
description: >-
  Use when a research draft must be checked claim-by-claim against original
  evidence before any external claim, revision, or submission wording.
---
# Claim–evidence handoff

## When
Any memo, manuscript paragraph, or experiment summary that will be treated as a scientific claim.

## Roles
- **Producer** (domain or writing seat): draft only from an evidence packet.
- **Verifier** (evidence seat): recomputes from originals; never trusts the draft's arithmetic or confidence.
- **Owner** (human): one repair cycle max, then decide.

## Packet fields (required)
Attempt ID · input version · source paths (S1…) · claim IDs (C1…) · numerator/denominator/arithmetic · recommendation · unresolved · next owner.

## Producer steps
1. Label every source path or file hash as S#.
2. Emit claims C# with only supported facts; show calc for every rate or Δ.
3. Separate observed differences from causal/statistical conclusions.
4. Mark method novelty / safety / generalization as NOT_ESTABLISHED when unsupported.
5. Hand the original packet + draft to the verifier. Do not publish, push, or submit.

## Verifier steps
1. Read originals before the draft.
2. For each C#: supported | incorrect | unresolved; cite S#; correct text if possible.
3. Check cohorts, denominators, windows, missing data, and overclaim.
4. Return one consolidated correction list.
5. After one revision, verify only changed claims; stop and escalate unresolved to the human.

## Hard bans
No fabricated citations · no elevating NOT_ESTABLISHED · no treating two agreeing bots as proof · no rewriting Goal/contract/hash without owner order.
