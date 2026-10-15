---
name: retro
description: Weekly team retrospective for Allan Company. Use when Allan says /retro or during the Sunday weekly review. Reviews how the company worked this week and where Allan was the bottleneck.
---

# Retro

1. Read the board, `private/decisions.md`, the week's diary entries and check-ins. Note the weekly signals, without judgement (trends, not scores to beat): tasks done vs planned, application funnel movement, training done, sleep and mood trend, wins. Wellbeing items have no scale to beat.
2. Report in five short parts:
   - **Results:** what got done, wins.
   - **Bottlenecks (find, value, pick):** list every bottleneck in the actual work (friction log, tasks that waited on Allan, repeated questions); price each fix (time or money saved per month, risk removed); pick the one high-value fix and ignore the rest this week.
   - **What broke or repeated:** errors, wrong facts, things asked twice.
   - **Proactivity:** examples of each role acting at level 3-5 this week, and one place it should have.
   - **Proposals:** at most three process changes (new trigger, scheduled routine, charter change, permission change), each with trade-off and plan B.
3. Allan approves, changes or rejects each proposal. Apply the approved ones to CLAUDE.md, the agent files or `roadmap.md`, and log them in `private/decisions.md`.

## Promotion review (autonomy follows track record)
Once a month, per agent: count corrections by Allan, wrong facts, missed items and actions that needed an undo. Zero or very few over four weeks: propose moving one action from yellow to green (or red to yellow). Repeated errors: propose tightening. Allan decides; log it in `private/decisions.md`.


## Board meeting (weekly, as a file, not a live chat)
Agents cannot talk to each other, so the "meeting" is a shared page. Each area contributes three lines to `private/governance/board-meeting.md`: what worked, what slowed us down, one proposal. Adolfo adds cross-links ("health's sleep note matters for university's study blocks", "assistant's slot rule helps career") and picks at most three proposals for Allan's yes. Keep it short: tokens are the cost.

## Usage check
Once a week note, in one line each: weekly usage level (from /usage or /cost), number of sessions, models used, and the single biggest consumer. Savings are estimated, never claimed to the token; the point is to spot waste early.
