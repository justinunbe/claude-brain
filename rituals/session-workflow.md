---
type: ritual
updated: 2026-04-20
stable: false
---

# Session Workflow

How Claude (or any agent) starts and ends a working session with Jay.

## Start

1. Read `state/current-hare.md` — what's active.
2. Read `profile/from-jay.md` — anything Jay dropped since last session. Mark items `[DONE YYYY-MM-DD]` after folding them in.
3. Read the last 1-2 files in `sessions/` — what we were working on.
4. If the session is topic-specific (weekly planning, health deep dive, etc.), grep for related topics across `areas/` and `patterns.md`.
5. Greet Jay briefly, acknowledge context. Don't recite the whole page — show you read it by referencing one specific thing.

## During

- When Jay says something significant, note it silently. If it contradicts existing content, flag it gently.
- When Jay asks about something that lives in the brain, read the file rather than guessing.
- When a decision is made, draft the decision for the relevant `decisions.md`.

## End (synthesis pattern)

Last 2-3 minutes of every session:

1. Surface the top 2-5 things I'm about to write to memory. Plain language, not formatted.
2. Ask Jay to confirm, correct, or discard each.
3. Write confirmed items to the right files (append to sessions, promote enduring facts into profile/state/areas as appropriate).
4. Update `state/shifts.md` if anything shifted.
5. Mark open threads for next session.
6. Commit to git with a short descriptive message.

## Discipline

- Sessions append — never overwrite.
- `state/` and `areas/` are mutable; git preserves history.
- When in doubt, ask Jay rather than inferring.
- Anything Jay flags as sensitive gets `sensitive: true` in frontmatter.
