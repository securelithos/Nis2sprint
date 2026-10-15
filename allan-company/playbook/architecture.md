# Allan Company: the stack (where the agents live)

Status 2026-10-15. Plain files, so the company is portable.

| Layer | What it is | Today | Later |
|---|---|---|---|
| 1. Interface | Where Allan talks to the company | Claude app (iPhone, web) into this Claude Code cloud session; mail inbox `allanadjei+adolfo@gmail.com` | Slack or Telegram ("Loop Alley"), Remote Control on the laptop |
| 2. Runtime / orchestrator | The program that runs the agents | Claude Code in a cloud container. The main session is Adolfo; sub-agents run as separate workers with their own context | Scheduled tasks (cloud), a local runtime on the laptop, possibly a multi-model orchestrator |
| 3. Company definition | Who does what, rules, routines | `CLAUDE.md` (constitution, loaded at every start), `.claude/agents/*.md` (one file per role: name, description, tools, model), `.claude/skills/*/SKILL.md` (routines loaded on demand) | The same files; they are the portable core |
| 4. Models | The brains | Anthropic Haiku, Sonnet, Opus, chosen per agent (`model:`) | Mixed providers through a router; local open models for sensitive data |
| 5. Tools (MCP) | Hands: what agents can touch | Gmail, Google Calendar, Google Drive (read), Claude Docs, GitHub, web search and fetch. MCP is an open standard; many runtimes and models can use the same tool servers | Drive write, Slack, a database, phone reminders |
| 6. Memory and data | What the company knows | Markdown files: `private/` (personal, never in git) and tracked files; backup in the Claude Doc | GitHub for tracked files, Drive for private backups, a database (e.g. Postgres via Supabase) as an index over mail, diary, decisions, with search |
| 7. Triggers | What starts work without Allan | Allan's messages, the proactive pass, the mail inbox | Scheduled routines (morning brief, retro), webhooks (new file in a folder) |
| 8. Governance | What keeps it safe and defensible | Action limits green / yellow / red, ISMS-lite, decisions log, action log, git history, backups | Monthly audit in /retro, access reviews |

## Moving one level up (model-agnostic)
- Keep knowledge and rules in plain files or a database, not inside one vendor's chat.
- Keep tools behind MCP so any runtime can reuse them.
- The only vendor-specific parts today are the agent `model:` lines and the Claude Code features (sub-agents, skills, scheduled tasks). A router layer (one API in front of several providers) would let one role run on another model.
- Good reasons to mix: cost (routine work on cheap models), privacy (health and credit data on a local open model), resilience (a second provider when one is down). Price: more setup, more to secure, quality differences.

## Evidence and exception paths (finance comment, 2026-10-15)
"Defined roles, permission boundaries, evidence capture and exception paths before automating; a human must see what happened, intervene quickly and defend the outcome." Our mapping: roles (agent files), permission boundaries (action limits), evidence (decisions log, action log, git), exception paths (incident response in ISMS-lite, friction log), intervention (Allan approves red actions; everything yellow is reversible).

## Open research (not verified here)
Platforms named in the discussion (Paperclip, HyperAgent, Hermes Agent, Supabase as data layer): compare on runtime, model support, memory, tools, security and cost before choosing anything. Task T61.
