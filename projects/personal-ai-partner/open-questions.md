---
type: project
updated: 2026-04-20
stable: false
---

# Open Questions

Things we haven't answered yet. Answered questions get promoted into `decisions.md` and removed from here.

## Architecture

- How does the Notion mirror stay in sync with the markdown? Manual (Claude updates on structural changes) vs. automated (script or Notion API push)? Default start: manual. (Open — may become moot if Notion gets fully deprecated.)
- When the local model hybrid arrives in 3-6 months, how do we hand off tasks between Claude and the local model? What's the interface / routing logic?
- Do we ever want device access beyond Jay's Mac (mobile)?
- Communication model for how Jay and Claude actually exchange updates — deferred from Session 6. Now that writes are Claude-only, what's the back-and-forth interface between sessions look like?

## Weekly planning

- Day/time/cadence specifics — Jay to decide on first run.
- Format of the ritual output: narrative vs. structured goals/commitments/reflections? Default: structured, evolve.
- Does Jay want to see the plan before it's committed, or just talk it through?

## Ingestion (Phase 3+)

- First external data source — likely MacroFactor since Health is the hare. What's the pipeline?
- Calendar integration — Google Calendar? Apple Calendar?
- Email ingestion — yes/no/limited?

## Discipline

- ~~End-of-session synthesis: how tight? 2 minutes of verbal confirmation vs. a written summary Jay approves?~~ Resolved Session 6: `session-synthesis` skill surfaces the proposed diff in plain language, Jay confirms or corrects, then Claude writes and outputs the commit command. No silent writes.
- What counts as "sensitive enough" for the `sensitive: true` flag? Need concrete examples beyond dating/financials.

## The product question (deferred)

- When/how do we revisit "is there a product in here?" Jay said months. Is there a trigger — a feature-complete state, a time-box, a feeling?
