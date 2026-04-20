---
type: meta
updated: 2026-04-20
---

# Brain Index

Map of Jay's memory. Read this first to orient, then pull specific files.

## Start every session

The `brain-bootstrap` skill handles session start. It reads:

1. `profile/identity.md`, `profile/framework.md`, `profile/preferences.md`
2. `state/current-hare.md`, `state/active-goals.md`, `state/shifts.md`
3. The active hare's `areas/<hare>.md`
4. The most recent session in `sessions/`

Writes happen at end of session through `session-synthesis`. Jay does not edit files directly.

## Structure

### profile/ (stable — who Jay is)
- `identity.md` — name, family, job, quick reference
- `framework.md` — The 5 Areas, Tortoise & Hare, path to fulfillment, core values, ownership model
- `preferences.md` — how we work together (comm style, decision-making, pace)

### state/ (dynamic — what's active now)
- `current-hare.md` — which Area is the primary focus and its target
- `active-goals.md` — specific, measurable goals tied to the current hare
- `shifts.md` — chronological log of belief/focus/situation changes

### areas/ (one file per Life Area — evolves over time)
- `health.md`
- `wealth.md`
- `relationships.md`
- `purpose.md`
- `legacy.md`

### projects/ (long-running work)
- `personal-ai-partner/` — this project; folder with overview, decisions, open-questions, milestones
- `business-ideas-log.md` — short-form log of ideas + interest scores

### rituals/ (repeatable patterns)
- `weekly-planning.md` — template + cadence + inputs/outputs
- `monthly-consolidation.md` — memory maintenance pass
- `session-workflow.md` — how to start and end each session

### sessions/ (append-only history)
- One file per session, named `YYYY-MM-DD-session-N.md`

### patterns.md (cross-cutting observations)
Insights that span multiple Areas — e.g., interactions between Health and Relationships.

### ingest/ (future external data)
- `health/` — MacroFactor, Apple Health exports, etc.
- `calendar/` — calendar data
- `email/` — email signals (if ever connected)

Empty for now. Structure reserved.

## Cross-referencing

- Use `topics: [...]` in frontmatter to tag cross-cutting content.
- Links between files use relative paths: `[health](areas/health.md)`.
- When working on one Area, scan `patterns.md` and grep for the topic across files before going deep.
