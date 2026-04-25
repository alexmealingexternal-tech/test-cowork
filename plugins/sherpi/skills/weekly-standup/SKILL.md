---
name: weekly-standup
description: >
  Generate a weekly standup summary from recent git commits and open PRs.
  Trigger when the user asks for a standup, status update, or weekly summary.
tags: [productivity, standup, reporting]
---

Generate a concise weekly standup summary by reviewing:

1. Run `git log --oneline --since="7 days ago"` to get recent commits
2. Check open PRs with `gh pr list` if gh CLI is available
3. Summarise into three sections:
   - **Done** — completed work
   - **In progress** — open PRs or uncommitted changes
   - **Blockers** — anything stalled or needing input

Keep it under 10 bullet points total. Use past tense for Done, present for In Progress.
