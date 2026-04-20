---
type: ritual
updated: 2026-04-20
stable: false
---

# Monthly Consolidation Pass

Once a month, a reflective pass over the brain to keep it honest. The `consolidate-memory` skill handles the technical side; this file is the checklist.

## Cadence

First weekly planning session of each calendar month, or ad hoc when something is clearly drifting.

## Checklist

### Staleness

- [ ] Scan all mutable files for `confirmed` dates older than 60 days. Surface them to Jay for quick confirmation.
- [ ] Check `state/current-hare.md` — still accurate? Any shift needed?
- [ ] Review `state/active-goals.md` — archive completed items, clarify vague ones.

### Contradictions

- [ ] Compare newer session notes with older profile/area files. Any drift? Flag for reconciliation.

### Pruning

- [ ] Merge duplicate facts across files.
- [ ] Prune stale items that no longer apply.
- [ ] Update `index.md` if structure shifted.

### Growth

- [ ] New cross-cutting patterns for `patterns.md`?
- [ ] Project folders still the right shape? Split or combine if needed.

### Record

- [ ] Log the consolidation itself in `sessions/` so we can see the cadence holding.

## Output

- Git commit showing what was updated / pruned.
- Any items requiring Jay's confirmation surfaced at the next weekly planning.
