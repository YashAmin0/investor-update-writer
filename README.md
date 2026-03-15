# investor-update-writer

A Claude skill that turns raw founder notes — metrics, wins, problems, asks — into a polished investor update email.

## What It Does

- Writes monthly, quarterly, or pre-raise investor updates
- Supports two formats: standard long-form and angel-friendly short (5 bullets, 60 seconds)
- Leads with the most important number, not pleasantries
- Puts bad news early with a plan attached
- Always includes a specific, actionable ask
- Cuts vanity metrics (downloads, social followers, press without conversions)
- Keeps the update readable in under 90 seconds

## Installation

### Step 1 — Find your skills directory

Skills live in `~/.claude/skills/` (global) or `.claude/skills/` (project-local).

```bash
ls ~/.claude/skills/
```

If the folder doesn't exist, create it:

```bash
mkdir -p ~/.claude/skills
```

### Step 2 — Copy the file

```bash
cp investor-update-writer.md ~/.claude/skills/investor-update-writer.md
```

> Use `~/.claude/skills/` to make it available in every project, or `.claude/skills/` inside a specific repo to keep it project-local.

### Step 3 — Use it

In any Claude Code session:

```
/investor-update-writer
```

Claude will ask for the period, metrics, wins, challenges, and asks — then write the update.

## What to Have Ready

- **Period covered** — month, quarter, or custom window
- **Key metrics** — MRR/ARR, growth rate, churn, burn, runway
- **Wins** — specific deals closed, milestones hit, product shipped
- **Challenges** — what's not working and what you're doing about it
- **Ask** — intros, hiring help, advice, or capital

Missing some of these? The skill works with whatever you provide.