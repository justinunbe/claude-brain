---
type: ritual
updated: 2026-04-20
stable: false
---

# Session Workflow

How Claude (or any agent) starts and ends a working session with Jay. This ritual is now operationalized by three skills: `brain-bootstrap` (start), `brain-pull` (mid-session), `session-synthesis` (end). The descriptions below are the ritual's spec — the skills are the implementation.

## Start — handled by `brain-bootstrap`

Read, in order:
1. `profile/identity.md`, `profile/framework.md`, `profile/preferences.md`
2. `state/current-hare.md`, `state/active-goals.md`, `state/shifts.md`
3. The active hare's area file (`areas/<hare>.md`)
4. The most recent session in `sessions/`

Topic-specific sessions (weekly planning, project deep-dive, etc.) also read the relevant ritual or project files.

Greet briefly; reference one specific thing to prove context loaded. No recitation.

## During — handled by `brain-pull`

- When Jay says something significant, note it silently. If it contradicts existing content, flag it gently.
- When the conversation pivots to a topic or Area that wasn't loaded at start, pull the relevant file(s) before responding from memory.
- When a decision is made, draft the decision wording in working memory for the end-of-session write.

## End — handled by `session-synthesis`

Last 2-3 minutes of every session:

1. Surface the top 2-5 things about to be written to memory. Plain language, not formatted.
2. Jay confirms, corrects, or discards each.
3. Write confirmed items to the right files (append to sessions, promote enduring facts into profile/state/areas as appropriate).
4. Update `state/shifts.md` if anything shifted.
5. Mark open threads for next session.
6. Output the commit + push command for Jay to run in Terminal.

## Discipline

- Sessions append — never overwrite.
- `state/` and `areas/` are mutable; git preserves history.
- No silent writes. Everything canonical is confirmed by Jay.
- Jay does not edit .md files directly. All writes flow through `session-synthesis`.
- Jay does not push independently. Commits happen through commands you give him at session end.
- Anything Jay flags as sensitive gets `sensitive: true` in frontmatter.
