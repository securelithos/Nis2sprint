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
| 17 | **Watchdog** (`/watchdog`): calendar conflicts, missing dates, unanswered mail, due follow-ups, cross-functional gap analysis (CV vs profile, imports vs Gmail, plan vs calendar, board vs goals); insight -> action -> prepared draft | "Dashboards are dumb": tell me what to do tomorrow and write the script | Skill live 15.10; first run found the CISM exam missing from the calendar and no study plan after 21.10 | live |
| 18 | **Loop channel for family or helpers** (like Allie's team asking her AI): e.g. Lars or family ask "is Allan free Saturday?" with strict limits on what can be shared | Assistant behaviour like a real PA | Only after Telegram/Slack exists; define what is shareable first | idea |
| 19 | **Build the factory, then the product** (Allie): the company's primitives are reusable: memory, approvals, watchdog, charters, routines, backup, ISMS-lite, retro, model mapping. Every new project starts from them | Each next thing ships faster; the measuring is the foundation layer | Keep primitives generic and documented | building |
| 20 | **Idea Lab / startup accelerator** under the Chief Dreaming Officer: inbox -> screen -> scorecard -> cheap test -> Allan decides (go / park / kill). A scout role finds ideas on a schedule (friction log, diary, news, job-search patterns, conversations) | Hand the finding of ideas to the company; keep the billion-dollar option alive | `private/ideas/inbox.md` with pipeline and scorecard | building |
| 21 | **Weekly signals** in /retro: insight -> action -> prepared draft, no judgement; wellbeing items have no scale | Benchmark of own productivity without turning life into a score | Line added to /retro | building |
| 22 | **Model check**: when a new model appears, run three standard tasks (a brief, a CV edit, a calendar plan) and compare before switching an agent | Vendors test first; we meet a model on day one | Add to the monthly /retro | idea |
| 23 | **Brief delivery**: rendered Claude Doc per day plus a push on the iPhone (calendar alert or scheduled-task notification in the Claude app) | Brief readable and delivered without opening a session | Decision T54 | planned |
| 24 | **Inbox channel by mail**: Allan dictates a mail on the phone to `allanadjei+adolfo@gmail.com`; Adolfo picks it up in every run (only mails sent from Allan's own account count) | Commands from outside without new infrastructure | Rule in CLAUDE.md and /watchdog; Allan tests (T56) | building |
| 25 | **Wispr Flow** for dictation everywhere (diary, inbox mails, chat) | Speak, don't type | Allan tests (T57) | idea |
| 26 | **Claude in Slack or Remote Control** for a real "Loop Alley" and for driving a session on Allan's own computer (`claude remote-control`, Claude Desktop) | Ask the company from anywhere; reach local files | After GitHub and Drive are sorted | idea |
| 27 | **Usage playbook** (`playbook/usage-tips.md`): rules to stay under limits, rated and applied | Lower cost, fewer limit hits | Live | live |
| 10 | Personality test result in the knowledge base | Agents read context correctly, fewer misreadings | Allan sends the result | idea |

## Org chart draft (idea 1)

- **CEO: Allan**
- **Chief of Staff / Concierge: Adolfo**: routing, approvals, memory, proactive pass
- **Chief Health Officer: Josef**: health coach; under it nutrition, training, mobility and sleep
- **Chief Wellbeing Officer**: wellbeing coach
- **Chief Career Officer**: career coach (applications, interviews, career strategy)
- **Chief Learning Officer / Dean: Mao**: Allan University (advisor, tutor, librarian, critic, roommate)
- **Chief Financial Officer** (also owns the VC allocation of Allan's own capital): budget, credit repair, FIRE plan (to come with the finance import)
- **Chief Information Officer / Editor**: morning brief, research
- **Chief Dreaming Officer** (name to come): keeps the moonshots alive (UAE Director, EUR 500k, FIRE, startup), connects today's tasks to them, questions small thinking. Owns the Idea Lab (scout, analyst; more when needed)
- **Operations**: personal assistant (mail, calendar, errands)
