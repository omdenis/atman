---
name: atman-checkout
description: >
  CLOSE a focused work-block on an atman system (systems/<name>/). Synthesizes the
  block's captured events into ONE review (a projection — never hand-write "what I
  did"), then WRITES a new dated handoff (handoffs are an append-only folder) ending
  in a Hemingway bridge, so next time atman-checkin flies in cold-free. This is the
  CLOSE half; atman-checkin is the OPEN. "handoff" is the artifact you WRITE here. Use
  when working in the atman vault and the user says "checkout", "/atman-checkout",
  "close the block", "wrap up", "закрой блок", "чекаут", "заканчиваю", "sandhya
  close". Decisions live in atman.
---

# atman-checkout — CLOSE a work-block  *(sandhya, close half)*

> The **handoff** is a baton: *written here* at checkout, read at the next
> [`atman-checkin`](../atman-checkin/SKILL.md). Checkout is the CLOSE.

Goal: leave the system in a state your next self can re-enter instantly.

## Steps

1. **Synthesize, don't re-type.** Roll up the block's captured events into ONE
   **review** event (what happened, what was decided, the WHY). This is a *projection*
   over events you already captured — do NOT hand-author a fresh "what I did" log. If
   the events are thin, that's a signal you under-captured during BUILD — fix the
   capture, not the report.
2. **Write a NEW dated handoff** to `systems/<name>/sessions/handoff/`
   (`YYYY-MM-DD--handoff--<slug>.md`) — **append-only, never overwrite** the old one
   (newest = the next checkin's entry point). It must contain:
   - **Where I stand** — current state of the system.
   - **Critical context (WHY, not just WHAT)** — intent and rejected paths a cold
     reader would otherwise re-derive painfully.
   - **Next steps** — ordered, the first one concrete.
   - **The bridge** — the final line (see below).
3. **Leave the Hemingway bridge** — the heart of zero-friction re-entry.

## The Hemingway bridge — best practices

Hemingway stopped writing mid-sentence, when he knew what came next, so the next
day's start was effortless. Same here: **end the block while the next move is obvious
and partly in motion**, so checkin needs zero deciding.

Pick the form that fits what you were doing (choose; mix if useful):

- **Half-done action** — leave the next micro-step literally started: a file open at
  the right spot, a sentence half-written, a stub. Re-entry = *finish*, not decide.
- **First command / file:line** — the exact thing to touch next (`path:line`, a
  command). Re-entry = *act before thinking*, momentum first.
- **The live question** — the open question you were chewing on, written down.
  Re-entry = resume the *thinking thread*. Best when the next move is a decision, not
  a keystroke.

Rules for a good bridge:
- **One concrete first action**, never a vague "continue working on X".
- Stop *before* you're drained, with momentum left.
- Capture the *why-now* if it's non-obvious, so future-you trusts it.

## The 1–2 forming questions (ask the user)

Before writing the bridge, ask up to two quick questions:

1. **"What's the single next action when you sit down again?"** (→ the bridge line)
2. **"What would future-you forget that matters?"** (→ the critical-context block)

Keep it to 1–2 — a sharper handoff, not a debrief.

## Anti-patterns

- **Hand-writing the day's report** — re-typing what events already hold. Synthesize.
- **Vague bridge** — "keep going on the loop" gives next-you nothing. Be concrete.
- **Overwriting the handoff** — handoffs are append-only dated files; the newest is
  the entry, the older ones are history.
