# head-coach-transfer — Strong Standard

Shared memory of the R5 Rock: head coach role defined, improved and transferred to Brent. This repo (branch `main`) is the single source of truth for the three project documents. The Rock Plan document in Drive is a frozen baseline and points here.

**Rock owner:** Brent. **Support:** Bernardo, who owns tasks in this Rock. **Sprint:** S4-2026.

## The three documents
| File | What it is | Update rule |
|------|-----------|-------------|
| decision-log.md | Every decision, one row, append-only. Supersedes all other documents. | New rows at the top. Never edit old rows (except marking "Replaced by D-XXX"). |
| project-brain.md | Living state: phase, done, in progress, blocked, next. | Updated at the close of any chat that changes status. |
| master-plan.md | Full task layout: tasks, owners, types, dependencies, execution order. | Only when the plan itself changes: logged as a decision first, and the JSON fragment regenerated after. |

## What is NOT here
Task status and all dates live in the Operations Dashboard. Deliverables live in Google Drive. This repo holds the plan and the reasoning, nothing else.

## Workflow
- **Chat start:** every Project chat reads the three files directly via their public raw URLs — no GitHub API, no token.
- **Chats never write:** a chat produces the content of a change and hands it back; the person uploads it with their own Claude Code session, which does pull → edit → push on `main` following `CLAUDE.md`.
- Documents are pure Markdown — no HTML, no GitHub Pages.
