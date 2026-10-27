# Operating model (bot-led)

## Navigation
Each seat reads its own role file first, then the project’s frozen Goal / state / current card / latest handoff. This repo does **not** replace project evidence roots.

## Dispatch
- One lead owns the queue.
- Simple work: single seat. Independent subproblems may run in parallel; dependent steps and final integration are serial.
- One writer per file; reviewers are read-only on that snapshot.
- Parent card is task-state authority; project root state is science-lifecycle authority. Do not invent a third live status board.

## Execution
- Advance real deliverables inside standing authorization.
- External jobs bind a stable idempotency key; finished jobs are not re-run because the agent restarted.
- Model identity comes from tool receipts, not bot nicknames.
- Group @ is not a private exchange; record send receipts and wait for confirm before continuing critical paths.

## Acceptance
- Freeze the artifact, collect hashes once, review that snapshot.
- At most two substantive revision rounds per batch unless new evidence appears.
- Card `done` / hash match / tool rc0 ≠ scientific PASS.

## Permissions
Follow the project’s named grants. Do not expand power from this framework doc. Do not read secret values into chat. Keep negatives and applicability bounds.
