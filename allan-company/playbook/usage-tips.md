# Playbook: using Claude without hitting limits

Collected 2026-10-15 from a "22 rules" post. Rated by Adolfo: **use** = sensible and we apply it; **adapt** = useful with a change; **check** = claim about limits or pricing we could not verify.

## How Allan Company applies them
| Rule | Rating | How we use it |
|---|---|---|
| Never switch models mid-chat; Claude rereads everything at full price | use | Pick the model at the start of a session. Cheap work goes to agents with their own model (they start with a small context). A switch loses the prompt cache. |
| Never go back to an old chat; ask for a short summary, start a new one | use | Our memory files *are* the summary: a new session reads CLAUDE.md, the board and the profiles. End sessions with /wrapup. |
| In Claude Code: one task, then /clear. Split the day into sessions (morning, afternoon, evening) | use | One topic per session; /wrapup before /clear. Long sessions get expensive because every turn rereads the context. |
| One topic per chat | use | Same as above. |
| Put all asks in one message | use | Fewer turns, fewer rereads. Allan already does this well. |
| Start a task with "ask me questions before you start" | use | Built into /advisor and the intake step of CLAUDE.md. |
| Plan in text first, ask for the file last | use | Plans and outlines in chat or a doc, files at the end. |
| Edit the part, never a full redo | use | Agents edit sections, not whole documents. |
| Never correct Claude; edit your prompt or start over | adapt | For one-shot outputs yes. In a working session, a short correction is fine; the rule goes into CLAUDE.md so it is not repeated. |
| Keep instructions under 2,000 words | adapt | CLAUDE.md is near that size; detail moves into agent files, skills and this playbook, loaded only when needed. |
| Load connectors on demand | use | Agents only list the tools they need. |
| Crop screenshots, turn PDFs into text | use | Lab reports, CVs and transcripts are stored as text in private/. |
| Upload reused files once (Project) | adapt | Our equivalent is private/ plus the Claude Doc backup. |
| Pause scheduled tasks you don't read | use | Every scheduled routine gets a review in /retro; unread ones are paused. |
| End quick questions with "No web search. No files." | use | For quick factual questions. |
| Speak, don't type; use Wispr Flow | use (test) | Allan tests Wispr Flow (T57). Dictation fits the brain diary. |
| Medium effort, never max | adapt | Default medium; high effort only for hard decisions (offers, health, strategy). |
| Ask Claude for images rarely | use | |
| Use Opus in every chat, never Fable | check | Opinion. Our mapping: Haiku routine, Sonnet default, Opus for heavy work (CLAUDE.md). |
| Save your one free reset for a bad day | check | Not verified; depends on the plan. |
| Sunday = max day, limits reset at 5 pm | check | Not verified; reset times depend on the account. |
| Send this to your team | - | |

## How-to: get the gist of a long video without watching it
1. **NotebookLM (best for keepers):** add the YouTube link as a source; ask for key points, a study guide or an audio overview. Works when the video has captions. Good for the principles library.
2. **YouTube's own transcript:** under the video description, "Show transcript"; copy it and paste it to Adolfo for a summary.
3. **Send the link to Adolfo** (chat or the +adolfo mail): Adolfo tries to fetch the captions and returns a summary in the level-5 style: the 5-10 key points, what matters for Allan's goals, what to do with it. If YouTube blocks the cloud, fall back to 1 or 2.
Summaries only; no full transcripts are stored or passed on.
