# Claude Code setup — head-coach-transfer (one time)

**Who:** Brent and Bernardo, and anyone who uploads changes to this Rock.
**Why:** Project chats READ this repo on their own, through public raw URLs. Nobody needs setup to read. To WRITE, each person needs their own Claude Code session connected to this repo. That is what this guide sets up.
**Time:** 5 min. Nothing gets installed on your computer.

## Step 0 — Shared GitHub account
Everyone uses the same shared Strong Standard GitHub account (the one on the membership email). No individual accounts, no collaborators. The credential is shared over a secure channel (team password manager) and never pasted in a chat, Slack, email, or this repo. If you don't have it, ask Bernardo over that channel.

## Step 1 — Open Claude Code on the web
Go to `claude.ai/code` in your browser and sign in with your Claude account.

## Step 2 — Connect GitHub (once)
Claude Code will ask you to connect GitHub and install the Claude GitHub App.

Sign in to GitHub with the **shared Strong Standard account**, not a personal one. If your browser already has a different GitHub account signed in, sign out first or use a private window.

When it asks which repositories to give access to, grant access to the whole F4LA organization. Granting only this repo works too, but then you repeat this step for every new Rock.

Note: Claude Code on the web connects one GitHub account at a time. If you had a personal GitHub connected, this replaces it.

## Step 3 — Select the repo
At the bottom of the Claude Code screen, pick `head-coach-transfer` and the `main` branch. You should see both before you type anything.

## Step 4 — Prove it works
Type this and send it:
> Pull the latest, append a line to `setup-checks.md` with my name, today's date and "setup OK", commit and push to main, and show me the commit hash.

Open `setup-checks.md` on GitHub and confirm your line is there. Then post in Slack: "Setup done, test push OK."

## Day to day (after setup)
1. Work in a Project chat. At close it hands you ready content (Decision Log rows, Project Brain edits).
2. Copy it, open `claude.ai/code` with this repo selected, paste it, and say "sube esto".
3. Claude Code does pull → apply → push on its own (the rules are in CLAUDE.md) and gives you the commit hash.
4. Paste that hash back into the chat to close it.
5. Separately, mark the task done in the Operations Dashboard. This repo does not track status.

## Two people write this repo
Brent and Bernardo both push here. Claude Code always pulls before editing, so normal work is safe. The one thing to watch: if you both close a task the same day, the second person's Decision Log ID must follow the first. Claude Code reads the top row to check, but if it flags a conflict, do not force it. Re-read the log and renumber.

## If something fails
- Push rejected or "permission denied" → the GitHub App lost access or you are signed into the wrong GitHub account. Redo Step 2 with the shared account.
- The repo does not appear in the selector → access was not granted to F4LA in Step 2. Redo Step 2.
- Claude Code reports a conflict → do not resolve it yourself. Screenshot it to Bernardo.
- Anything else → ask Claude Code what happened. If it is not solved in 5 minutes, Slack Bernardo.
