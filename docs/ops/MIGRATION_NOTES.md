# Migration notes

When adopting this framework on an existing bot fleet:
1. Keep in-progress cards; do not cancel/restart solely for migration.
2. Do not mix unrelated project objects on shared seats.
3. Standing authorization applies only inside a named attempt the human opened.
4. Pure review / SHA recheck does not consume RUNNING slots.
