---
type: project
updated: 2026-04-20
stable: false
---

# Decisions Log

Dated log of decisions made on this project. Future us will forget why we chose X over Y unless it's written down the day we decide.

Format: `## YYYY-MM-DD — Decision title` with Context / Decision / Rationale / Alternatives.

---

## 2026-04-20 — Pause product search, build personal AI partner first
**Context:** Session 4. Hunted SaaS categories, all rejected. Health stack already well-solved (MacroFactor etc.). Consumer vs B2B tension surfaced.
**Decision:** Not pursuing a product right now. Spend the coming months building the best possible personal AI partner.
**Rationale:** Builder archetype + Tony Stark vision made this the right next move. Product decisions from a stronger foundation later will be better.
**Alternatives considered:** Pushing through a SaaS category with grit (rejected — Jay doesn't fake interest). Pivoting straight to hardware (deferred).

## 2026-04-20 — Brain substrate: plain markdown + git, Notion as mirror
**Context:** Need memory that survives AI provider changes (Claude → local model hybrid in 3-6 months) and years of evolution.
**Decision:** Source of truth = markdown files in `~/claude-brain` on Jay's Mac, versioned in private GitHub repo. Notion kept as human-browsable mirror.
**Rationale:** Portability (any AI tool can read), durability (no provider lock-in), version history (audit trail), low complexity.
**Alternatives considered:** Stay in Notion (rejected — lock-in risk). iCloud folder only (rejected — no version history). Obsidian vault (considered — vanilla markdown more portable).

## 2026-04-20 — Hybrid AI topology: local + Claude
**Context:** Jay plans to add local models for lower-tier tasks within 3-6 months, with Claude as orchestrator.
**Decision:** Memory must be readable by any agent off the filesystem. No Claude-specific or MCP-specific storage patterns.
**Rationale:** Forces the brain to stay portable. Any future capable model with file access can operate on it.

## 2026-04-20 — Multi-source ingestion designed for later, conversations-first now
**Context:** Memory could be conversations-only or could ingest external signals (MacroFactor, calendar, email, WHOOP, etc.)
**Decision:** Structure anticipates external ingestion (empty `ingest/` folders reserved) but Phase 1 is conversations only.
**Rationale:** Don't over-engineer before the basics work. Easier to add later when we know what the brain looks like in use.

## 2026-04-20 — Project structure: folder-per-project for long-running work
**Context:** Single-file-per-project doesn't scale past a few weeks. Business ideas log is fine as one file; real builds need more.
**Decision:** Each long project gets a folder with `overview.md`, `decisions.md`, `open-questions.md`, `milestones.md`, and `artifacts/`.
**Rationale:** Decisions log is the critical piece — future us will forget rationale without it.

## 2026-04-20 — Weekly planning as first-class architectural feature
**Context:** Jay named weekly planning as a recurring ritual we'd do together.
**Decision:** `rituals/weekly-planning.md` is a dedicated template with defined inputs/outputs/cadence. Ritual artifacts append to `sessions/` and propagate into `state/active-goals.md`.
**Rationale:** Rituals are how systems stay honest. Calendar events drift; structured rituals don't.

## 2026-04-20 — Sensitivity flag + no passwords
**Context:** Brain lives on private GitHub. Not all content equally exposable.
**Decision:** `sensitive: true` frontmatter flag on extra-careful content (dating specifics, personal finance details). No passwords, ever.
**Rationale:** GitHub private is secure enough for most things. Flag gives finer-grained handling when needed.

## 2026-04-20 — Ownership correction
**Context:** Claude misread Session 3 and thought Jay wanted to own some engineering (Git decisions, etc.).
**Decision:** Corrected — machine tasks default to AI (Claude). Jay's deep work = vision, physical, relational, thinking. Engineering/plumbing is Claude's problem.
**Rationale:** Jay named the ownership model clearly: Jay owns Vision/Standards/Exceptions; Claude owns Process/Execution/Iteration/Process decisions.
