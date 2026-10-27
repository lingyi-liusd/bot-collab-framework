# Bot-led multi-agent collaboration charter

A **single lead bot** owns dispatch and the queue. Domain seats execute; a review seat gates claims. Humans set goals, budgets, and red lines—not every micro-step.

## Seats (templates)
| Seat | Responsibility |
| --- | --- |
| **Lead** | Only dispatcher; task cards; closes gates; reports judgment changes |
| **Planner** | Turn frozen goals into executable plans / prompts (optional external planner) |
| **Math / hard reasoning** | Propositions, proofs, counterexamples; real tool channels when admitted |
| **Literature / precedent** | Strongest prior art and opposing evidence |
| **Engineering** | Reproducible code / compute; keep logs and receipts |
| **Review** | Named risks only; separate delivery / science / evidence / novelty; author cannot self-clear |
| **Environment** | Named env failures only |

Rename seats to fit your product; keep the **one owner per card** rule.

## Hard rules
1. Object before claim; unknown and negative results stay visible.
2. Every card: `project_id`, `task_id`, `attempt`, mode, owner, question, inputs, allowed actions, budget, artifacts, stop conditions.
3. One RUNNING paper card per seat; review / SHA recheck do not consume RUNNING.
4. Display names ≠ model identity. Record real tool receipts (or “not called”).
5. Same-model role swap ≠ independent model review.
6. Complex native-model exploration is allowed as **candidate / pending review** only; review seat organizes verification (prefer a different capable channel) before formal conclusions.
7. No secrets in repo; no silent spend; no unauthorized push/submit.

## Human interrupts only for
Evidence ceiling or scientific adjudication; Goal/hash change; cloud spend / push / secrets; explicit stop.
