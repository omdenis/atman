---
name: atman-checkin
description: >
  OPEN a focused work-block on an atman system (the meta-system, a project, any
  systems/<name>/). Reads the LATEST handoff (handoffs are a folder; newest = entry
  point) + fresh events, runs session-open to frame, then starts strictly at the
  handoff's bridge action — so you fly in with zero blank-page friction. This is the
  OPEN half; atman-checkout is the CLOSE. "handoff" is the artifact you READ here, not
  this command. Use when working in the atman vault (~/atman, systems/<name>/) and the
  user says "checkin", "/atman-checkin", "open the block", "start a system session",
  "открой блок", "чекин", "начнём блок", "sandhya open". Decisions live in atman.
---

# atman-checkin — OPEN a work-block  *(sandhya, open half)*

> The **handoff** is a baton: written at **checkout**, *read here* at checkin.
> Checkin is the OPEN. The close is [`atman-checkout`](../atman-checkout/SKILL.md).

Goal: full context restored in ~2 minutes, **zero blank page.** You should never
open a file and think "…what now?" — the handoff tells you; you just act.

## Steps

1. **Resolve the system.** Which `systems/<name>/`? (atman by default if working on
   the methodology/machinery itself.)
2. **Open the latest handoff.** Handoffs live in `systems/<name>/sessions/handoff/`
   as dated files. **The newest file is the entry point** — read it. It carries:
   where I stand, critical context (the WHY), next steps, and a final **bridge** line.
3. **Read fresh events** since the last checkout — scan `bin/events/`,
   `bin/decisions/`, `bin/observations/` and the system's own folders for anything
   new the handoff may predate.
4. **Frame the block** — run [`session-open`](../session-open/SKILL.md): optional
   micro catalog-scout to widen vision, then 2–4 clarifying questions, then restate
   what this block is.
5. **Print the block frame** (always — this is the first thing the user sees after
   `checkin`). A short reminder of *how we operate here*, so you drop into the right
   mode before acting:

   **🎯 Focuses of the block**
   - **Work on the working system** — not goals/vibration; systems are the unit. An
     idea without a carrier-system goes to quarantine, not the work.
   - **Ship the next +1** — one real capability of the system, max value-per-effort.
   - **Building > planning > designing > talking-about.**
   - **Session, not project** — a journey, not a volume to finish; the end is decided
     at any moment, not by a task list.

   **📐 Principles** — list the **current** atman principles live: glob
   `bin/principles/*.md` and show each one's `## Принцип` one-liner (don't hardcode —
   the set grows). Today's set includes immediate-capture, friction-as-filter,
   dated-files+changelog-inside, decision-context, config-as-projection. Plus the
   methodology spine: event-sourcing (append-only, `supersedes`, projections are
   ephemeral) × work-system lens × decision-journal (`expected_outcome` +
   `confidence` + `review_at`).

   Keep it tight — a scannable header, not an essay.
6. **Start strictly at the bridge.** Do the one concrete next action the handoff ends
   with. Don't re-plan — past-you already decided. **Act first.**

## Then — BUILD (the block itself)

Goal: ship the next **+1** to the system — a real capability, not meta-work.

- **Work the upgrade queue.** "What to work on" = the system's `system.md` upgrade
  queue + the handoff's next-step. Pick the most value-per-effort and build it.
  Building > planning > designing > talking-about.
- **Capture as you go (immediate-capture).** Every decision / observation / idea /
  experience goes *immediately* to a vault event file. "Not written to a file = does
  not exist." Decisions get `expected_outcome` + `confidence` + `review_at`.
- **Brain-dumps are events, not the work.** Dump tangents as `idea`/`observation`
  events (or to `_inbox`) and return to building. Fuel, not hijack.
- **No double-entry.** You capture now so checkout never has to re-type "what I did".

When you wind down, run [`atman-checkout`](../atman-checkout/SKILL.md) to close.

## Anti-patterns

- **Blank-page open** — opening a system with no handoff to read. If there's none,
  checkout failed last time; that's the bug.
- **Re-planning at the bridge** — the previous you already chose the next move. Act.
- **Meta-work instead of +1** — building registries/analytics *about* the system
  instead of the next real capability *of* it.
