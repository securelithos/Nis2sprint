---
name: wrapup
description: End-of-day routine for Allan Company. Use when Allan says /wrapup, "Feierabend", "Backup" or ends a work session. Tidies the board, logs decisions and wins, and updates the backup.
---

# Wrap-up

1. **Board:** mark finished tasks Done, move dates that passed, make sure every open task has an owner and next step.
2. **Decisions:** add today's decisions with a one-line reason to `private/decisions.md`.
3. **Wins:** add today's wins to `private/decisions.md` under "Wins". Name them plainly; Allan finds it hard to count small wins.
4. **Questions:** add new open points to `private/calibration/questions.md`.
5. **Backup:** update the Claude Doc "Allan Company backup 2026-10-15" (https://claude.ai/code/artifact/d52972b2-f67e-4542-a2e8-2534b89e3a1b) with every file in `private/`, `output/` and the tracked setup that changed since the last backup. Append a dated section; do not rewrite earlier sections.
6. **Git:** commit tracked changes locally. Push only if Allan has said so.
7. Tell Allan in 3-5 lines: what is done, the top 3 for tomorrow, and anything waiting on him.
