# OPS-C · Standing authorization & pipeline (generic)

This patch changes **operations and dispatch only**, not scientific objects.

## Problems it solves
1. **Authorization bottleneck** — every open / review / close / next step waits on the human.
2. **Shaving residuals** — cards whose only output is a narrower condition set or renamed symbols.
3. **Serial gates** — theory → lead → human → evidence → lead → human → theory.
4. **Idle seats** — literature, adversarial review, interval checks unused while only two seats thrash.

## Positioning vs a single hard-push coder
Win on: multi-seat pipeline, load-bearing SHA chain, standing authorization with few human interrupts. **Do not** turn the lead into a slow approval gate.

## Rules
### C1 Standing authorization (per attempt)
Within a named attempt, the lead may automatically:
- read frozen sources for that attempt;
- open the next backlog card (unless a human stop order is active);
- auto-dispatch evidence review after a theory handoff;
- take the next backlog item after a gate close.

Interrupt the human only for: (a) evidence ceiling / scientific adjudication, (b) Goal or hash change, (c) cloud spend / push / secrets, (d) human says stop (overrides all automation).

### C2 Auto review relay
Theory handoff → evidence review without human ping. Pure review does not consume RUNNING slots.

### C3 No residual-shaving cards
Every card must state which claim / gap / judgment it can change, or the stop condition. Otherwise mark DEFER.

### C4 Side lines stay open
Literature, interval certificates, and sims keep their own backlogs. Cap: 1 paper + 1 side line per project; review free.

### C5 Room hygiene
Group rooms: index, conflicts, close summaries only. ACKs and “started” stay quiet.

### C6 Idle seats
Adversarial review before close when useful; fill UNKNOWN literature with full-text pressure tools; seats without a usable id do not occupy roster slots.

## Red lines (always)
No push, no submit on the human’s behalf, no Goal/hash edits, no reading secrets, no unauthorized cloud spend.
