# Claude Brain

Jay's personal AI partnership memory. Plain markdown, portable, tool-agnostic. Designed to survive AI model changes and provider shifts. Any capable agent can read from here.

## Start here

- `index.md` — full map of this brain
- `profile/identity.md` — who Jay is (quick reference)
- `state/current-hare.md` — what's the active focus right now
- `sessions/` — history of working sessions, newest at the bottom

Every session is bootstrapped by the `brain-bootstrap` skill; mid-session lookups by `brain-pull`; end-of-session writes by `session-synthesis`. Monthly maintenance by `consolidate-memory`. Jay does not edit files directly — all writes come through these skills with his confirmation.

## Conventions

All files use YAML frontmatter:

- `type`: profile | state | area | project | ritual | session | pattern | meta
- `updated`: last modification date (YYYY-MM-DD)
- `confirmed`: last date Jay confirmed this is still accurate (mutable files only)
- `stable`: `true` = rarely changes; `false` = expected to evolve
- `sensitive`: `true` = extra care in consolidation; don't pull into cross-refs unless directly relevant
- `topics`: cross-cutting tags for retrieval, e.g. `[health, relationships]`

## Discipline

- Sessions are append-only. Never edit an old session file.
- `profile/`, `state/`, `areas/` are mutable; git preserves history.
- Profile = stable. State = dynamic. Areas = evolves. Rituals = templates.
- Monthly: run `rituals/monthly-consolidation.md`.
- Anything sensitive gets a `sensitive: true` flag and careful handling.
- No passwords. Ever.
