---
type: meta
updated: 2026-04-20
---

# Brain Index

Map of Jay's memory. Read this first to orient, then pull specific files.

## Start every session

1. `state/current-hare.md` — what's actively in focus
2. Latest 1-2 entries in `sessions/` — what we were working on
3. `profile/from-jay.md` — anything Jay dropped in the backchannel

## Structure

### profile/ (stable — who Jay is)
- `identity.md` — name, family, job, quick reference
- `framework.md` — The 5 Areas, Tortoise & Hare, path to fulfillment, core values, ownership model
- `preferences.md` — how we work together (comm style, decision-making, pace)
- `from-jay.md` — Jay's backchannel; raw notes/directives outside of sessions

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
