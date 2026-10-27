---
name: research-war-room
description: >-
  Use when coordinating the multi-seat research desk (literature, theory, V2X,
  writing, sim, evidence) with file-only handoffs and a human gate before any
  outbound action.
---
# Research war room

## Layout
- **Lead** (Grok Bot): plans, assigns, accepts only paths+receipts; never ghostwrites science.
- **Literature**: precedent × object matrix; abstract vs full-text grades; gaps ≠ novelty.
- **Domain seats** (fleet theory / V2X / sim): propositions, experiments, receipts.
- **Writing**: narrative from verified claims only; no self-adversarial scoring.
- **Evidence**: claim ledger; delivery ≠ scientific establishment; sole adversarial_review author.
- **Submission**: cover / checklist / revision_response DRAFT; never submit or push.

## Shared folder convention
`paper/` drafts · `evidence/<date>_vN/` receipts · `completion_receipt.json` · never overwrite closed packs; copy to new version dirs.
Each seat writes only under its own subfolder or clearly named artifact; do not rewrite another seat's signed file—open a new version path instead.

## Dispatch checklist (派活 6 项)
Every assignment from Lead to a seat must name all six:
1. **Task** — one verb + object
2. **Background** — Goal · attempt ID · why now
3. **Deliverable** — exact file path(s) to create
4. **Acceptance** — success criteria (measurable / path+SHA)
5. **Deadline** — wall-clock or "before next gate"
6. **Paths** — inputs to read (read-only)

Forbidden actions always restated when non-obvious (no push / no new experiment / no Goal edit).

## Report-back checklist (回报 4 项)
Every seat reply that claims done must include:
1. **Paths** — created/updated files (absolute or workspace-relative)
2. **Three-line summary** — result · residual risk · next hand
3. **Self-check** — which acceptance bullets met / unmet
4. **Open items** — blockers needing human or another seat
Prefer body SHA16 for claim files; if the file embeds its own hash line, note "whole-file vs body" separately.

## Handoff message template
Goal · attempt ID · inputs (paths) · success criteria · forbidden actions · report-back format (paths + 3-line summary + self-check + open items).

## Human gates
Push · journal submit · email/Slack to others · cloud spend · changing Goal/contract/hash · reading secrets — all require the human in chat.
Desktop / sign-in only in 1:1 with Lead—not in group rooms.

## One job per seat
Do not merge producer and verifier in one reply. Cap repair cycles at one unless the human extends.
Overlapping inbound (mail / WeChat / X): entry seat summarizes and routes; does not execute domain work.

## Long-running work (Wake on Done)
For authorized long sims or offline batches: seat runs work, writes `completion_receipt.json` via sim-completion-receipt, then Lead (or a routine) wakes on receipt path—not on chat chatter. Do not invent new cloud spend or expand batch size without human authorization.

## Load-bearing chain
Each room tracks one chain file under `_工作站/承重链/`. After a gate passes, name the next hand explicitly; silence after pass is not allowed for Lead.
