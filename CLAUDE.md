# CLAUDE.md — head-coach-transfer repo

This repo is the single source of truth for the R5 Head coach role transfer Rock's plan and reasoning. It holds three live documents:
- `decision-log.md` — every decision, one row each, append-only.
- `project-brain.md` — the current state of the project.
- `master-plan.md` — the full task layout. Changes only via a logged decision.

Task status and every date live in the Operations Dashboard, never in this repo.

Your job: receive change content (usually pasted from a Project chat) and apply it safely. The person pastes text and says "upload this" / "sube esto". You handle all Git mechanics — they never should.

## Non-negotiable workflow
1. Always `git pull` on `main` BEFORE touching any file. No exceptions.
2. Apply the change with targeted edits only. Never rewrite or regenerate a whole document — edit exactly what was handed to you and nothing else. If the pasted content conflicts with what's already in the file (e.g. a decision ID already taken), STOP and tell the person before editing.
3. Always commit and push immediately after editing. An unpushed change does not exist for the team.
4. After pushing, report the commit hash and a one-line summary of what changed.

## Rules per document
### decision-log.md
- New rows go at the TOP of the table, directly under the header.
- Never edit or delete an old row, except changing Status to "Replaced by D-XXX" when superseded.
- IDs are sequential. Read the top row to confirm the last used ID — never invent one. If the pasted ID isn't the next sequential ID, flag it before committing. This repo starts at D-006, so the next new row is D-007.
- Columns: ID | Date | Decision | Context (2–3 lines max) | Who | Status.
- Note: D-105 appears in `master-plan.md` and belongs to the dashboard repo, not this log. It is not a dangling reference and needs no row here.

### project-brain.md
- Update only the sections that changed.
- Always update the "Last updated" line (date + who) in the same edit.

### master-plan.md
- Only accepts changes backed by a Decision Log row. If asked to change it without a D-XXX, ask for the decision ID first.
- After applying any change here, remind the person in your report: **the JSON fragment has to be regenerated in the Rock Planner and sent to the Sprint project**, or the dashboard keeps running the old plan.

## Scope
Only the three live documents plus repo infrastructure (`CLAUDE.md`, `README.md`, `setup-claude-code.md`, `setup-checks.md`). Do not add other artifacts — deliverables live in Google Drive, and the dashboard's plan file lives in its own repo, on purpose.

## Never write a date or a status
If pasted content contains a start date, a finish date, or a task status, do not commit it. Say plainly that those belong to the dashboard and ask for the line without them. This Rock has no go-live date and no milestone deadlines, so there is no legitimate date to carry here beyond a Decision Log row's own date.

## Commit messages
Short and specific, referencing decision IDs when applicable. Examples: `Add D-007 (scope locked)` · `Brain: M1 done` · `D-004 marked Replaced by D-011`.
