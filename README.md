# bot-collab-framework

**Bot-led multi-agent collaboration framework** — rules, seat templates, task cards, and operating patches for teams where a **lead bot** dispatches work to specialized seats (math, literature, engineering, review, planner, environment).

This repository is **process infrastructure**, not a research dataset. It does **not** include scientific evidence, papers, goals, or project secrets.

## Why
Human time should go to goals and scientific decisions—not micro-approving every card open, review ping, and “next step.” Standing authorization + multi-seat relay + SHA load-bearing chain keep throughput without silent power expansion.

## What’s inside
| Path | Contents |
| --- | --- |
| `docs/TEAM_CHARTER.md` | Charter & seat map |
| `docs/00_common_bot_rules.md` | Shared hard rules (objects before claims, …) |
| `docs/01_research_lead.md` | Lead / dispatcher duties |
| `docs/OPERATING_MODEL.md` | Day-to-day operating model |
| `docs/COMPLEX_NATIVE_REVIEW.md` | Candidate outputs → mandatory independent-style review |
| `docs/ops/` | OPS A/B noise control, two-phase review, OPS-C standing auth |
| `docs/skills/` | Cursor-style skill packs (lead, review, literature, writing, …) |
| `roles/` | Example persona JSON seeds |
| `templates/TASK_CARD.md` | Minimal task card + handoff block |

## Quick start
1. Copy `templates/TASK_CARD.md` for each piece of work; fill `attempt` and stop conditions.
2. Appoint one **Lead**; other seats only act when named on the latest attempt.
3. Keep project evidence **outside** this repo (your own evidence root + SHA).
4. Adapt `roles/` names to your product; keep “display name ≠ model identity.”
5. Optional: load `docs/skills/*/SKILL.md` into your agent skill directory.

## Non-goals
- Not a task board / database / process lock.
- Not permission to spend, push, or submit.
- Not a claim that any scientific result is proven.

## Provenance
Derived from an internal Grok Bot / agent-workstation deployment (RB-20261026 + OPS patches), **scrubbed** of project-specific backlogs, evidence paths, and private machine config.

## License
MIT — see `LICENSE`.
