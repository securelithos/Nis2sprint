---
name: wrapup
description: End-of-day routine for Allan Company. Use when Allan says /wrapup, "Feierabend", "Backup" or ends a work session. Tidies the board, logs decisions and wins, and updates the backup.
---

# Wrap-up

1. **Board:** mark finished tasks Done, move dates that passed, make sure every open task has an owner and next step.
2. **Decisions:** add today's decisions with a one-line reason to `private/decisions.md`.
3. **Wins:** add today's wins to `private/decisions.md` under "Wins". Name them plainly; Allan finds it hard to count small wins.
4. **Brain diary:** ask Allan 2-3 short prompts (e.g. what are you worried about that you haven't said out loud? what did you decide over text? what do you now believe and why?). He dictates; nobody grades it. Save the raw text to `private/diary/YYYY-MM-DD.md` and pull decisions, wins and worries into their files. Skip if he says so.
5. **Questions:** add new open points to `private/calibration/questions.md`.
6. **Backup:** update the Claude Doc "Allan Company backup 2026-10-15" (https://claude.ai/code/artifact/d52972b2-f67e-4542-a2e8-2534b89e3a1b) with every file in `private/`, `output/` and the tracked setup that changed since the last backup. Append a dated section; do not rewrite earlier sections. Paste each changed file **whole** as a bold path label followed by a code block (that is what `/start` restores from); condensed notes alone are not enough.
7. **Git:** commit tracked changes locally. Push only if Allan has said so.
8. Tell Allan in 3-5 lines: what is done, the top 3 for tomorrow, and anything waiting on him.
