# Allan Company roadmap and idea backlog

Ideas Allan collects. Status: idea / planned / building / live. Nothing here is a commitment until it moves to the board.

## North Star
Allan stops being the first domino and the bottleneck. Agents know the goal, have the tools and permissions, and know what normally triggers their work, so they solve, plan for failure and escalate only decisions (proactivity level 5, see CLAUDE.md).

## Ideas

| # | Idea | Why | First small step | Status |
|---|---|---|---|---|
| 1 | **Org chart with C-level roles** (e.g. Chief Health Officer with nutrition, training and sleep under it; Chief Learning Officer = University dean; Chief Dreaming Officer for vision and moonshots; CFO for money and FIRE) | Clear ownership; roles that only make sense for one person's life | Draft below; decide later | idea |
| 2 | **Step 0 charter for every role**: North Star, tools and permissions, triggers ("what normally starts this work"), proactive scan | What any agent needs before it can act on its own | Added to `.claude/agents/_template.md`; roll out to all roles | building |
| 3 | **Brain diary**: daily dictated entry (worries, wins, decisions, what I now believe and why, questions, feedback), agents read it | The uncodified context that decides answers; makes the company queryable | Part of `/wrapup` now, saved to `private/diary/` | building |
| 4 | **Diary page**: an HTML form like "Brain, meet diary" (prompt of the day, categories, streak, autosave), stored so agents can read it | Faster capture, streak motivation | Artifact with a shared store, after the habit works in chat | idea |
| 5 | **Queryable company**: one index over profiles, applications, diary, decisions, goals | "What did I decide about X and why?" answered in seconds | `memory/README.md` map exists; add a `/ask` routine later | idea |
| 6 | **Slack or Telegram**: mobile capture (voice notes into the diary), morning brief push, approve/decline buttons for the approval batch | Fewer app switches; approvals on the go | Check options and cost after the CISM exam; the Claude app with dictation already covers capture | idea |
| 7 | **Triggers**: e.g. a recording or PDF lands in a folder -> transcript, summary, filed (interview transcripts, lab reports) | The "easy half" of autonomy | Needs Drive write access or a watched folder | idea |
| 8 | **Scheduled routines**: morning brief, weekly retro, application follow-ups after 14 days | Work happens without Allan starting it | Waiting on Allan's yes per routine | planned |
| 9 | **Weekly retro with the whole team** (`/retro`) | Optimise processes together; find where Allan is the bottleneck | Skill added; run in the Sunday weekly review | building |
| 11 | **Friction watcher** (like Allie's "Toby" under the Chief of Staff): watches the workforce work and logs friction, repeated questions and missing access in `private/friction-log.md`; feeds `/retro` | Shows where the system, not Allan, is the bottleneck | Adolfo logs friction from today on | building |
| 12 | **Directors per domain with named agents** (Allie: 6 directors, 34 agents, Chief Dreaming Officer "Phoebe" who asks of every output: how do we 10x it?) | Scale without cost; one owner per domain | Name directors when the org chart is decided | idea |
| 13 | **Phone integration**: reminders and nudges on the phone (calendar alerts, later Telegram or similar) | Tools reach Allan where he is | After GitHub and Drive are sorted | idea |
| 14 | **ISMS-lite for the company**: process register with owners, asset inventory, risk register, BIA, BCP, incident response, audit | Run the company like a well-governed organisation | Skeleton in `private/governance/isms-lite.md` | building |
| 15 | **Workforce stages** (Allie: one agent -> proactive agent -> two agents routing -> workforce with mission control, parallel work, right model per agent). We are between 2 and 3; mission control = board + proactive pass | Grow one capability at a time | Model per agent set 2026-10-15; next: scheduled routines, then parallel runs | building |
| 16 | **"Loop Alley" channel**: one place (Slack/Telegram) where Allan asks the workforce and gets an answer now | Fast answers without opening a session | With idea 6 | idea |
| 10 | Personality test result in the knowledge base | Agents read context correctly, fewer misreadings | Allan sends the result | idea |

## Org chart draft (idea 1)

- **CEO: Allan**
- **Chief of Staff / Concierge: Adolfo**: routing, approvals, memory, proactive pass
- **Chief Health Officer: Josef**: health coach; under it nutrition, training, mobility and sleep
- **Chief Wellbeing Officer**: wellbeing coach
- **Chief Career Officer**: career coach (applications, interviews, career strategy)
- **Chief Learning Officer / Dean: Mao**: Allan University (advisor, tutor, librarian, critic, roommate)
- **Chief Financial Officer**: budget, credit repair, FIRE plan (to come with the finance import)
- **Chief Information Officer / Editor**: morning brief, research
- **Chief Dreaming Officer**: keeps the moonshots alive (UAE Director, EUR 500k, FIRE), connects today's tasks to them, questions small thinking
- **Operations**: personal assistant (mail, calendar, errands)
