# How Allan Company remembers

| Layer | What | Where | Lifetime |
|---|---|---|---|
| Working memory | The current conversation | this session | Gone when the session ends or is summarised |
| Short-term | What is happening now: tasks, check-ins, today's brief, weight log | `private/tasks/board.md`, `private/wellbeing/checkins.md`, `private/health-log.md`, `output/briefings/` | Days to weeks; cleaned up by `/wrapup` |
| Long-term: facts | Who Allan is and what is true | `private/health-profile.md`, `private/health-history-2024.md`, `private/career/profile.md`, `private/career/applications/*`, `private/wellbeing/notes.md`, `private/university/*` | Until corrected |
| Long-term: direction | Goals and decisions with reasons | `private/goals.md`, `private/decisions.md` | Reviewed monthly |
| Rules and roles | How the company works | `CLAUDE.md`, `.claude/agents/`, `.claude/skills/` | Changed deliberately |
| Open questions | What we do not know yet | `private/calibration/questions.md` | Answered in `/calibrate` |

## Where it is stored safely
- Rules and roles (tracked files): git branch, pushed only when Allan says so.
- Everything in `private/` and `output/` never goes to git. Its backup is the Claude Doc "Allan Company backup" (updated by `/wrapup`), later Google Drive.
- A new session starts by reading `CLAUDE.md`, then the board, goals and the profiles it needs.

## Rules
- Facts carry their source: Allan said / document / AI suggestion / unclear. Conflicts go to `private/career/import-log.md` or the questions file, never silently overwritten.
- Newest confirmed fact wins; the old one stays in the history line.
