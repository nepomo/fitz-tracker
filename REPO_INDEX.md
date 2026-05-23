# Repo Index — fitz-tracker

## Status
**Active** (write-only mirror of the Fitz Excel Rebuild autonomous loop; 5
target-day commits 2026-05-22 from the fitz-rebuild public-tracker generator).

## Purpose
Publish a single static `index.html` page that displays the current state of
the Fitz Excel Rebuild autonomous loop — last closed Work Order, next Work
Order, live engines (model + reasoning per phase), and the "All closes" table.
The fitz-rebuild repo writes here; consumers read.

## Production Entry Points
- `index.html` — the only published artifact. Renders standalone in a browser;
  auto-refreshes every 300 seconds.

## Apps / Lanes / Modules
- None in this repo. Generator lives in the
  [`fitz-rebuild`](../fitz-rebuild) repo (added 2026-05-22 in commit `4c85b75`).

## Important Scripts
- None in this repo. Build / push happens in fitz-rebuild.

## Important Tests
- None in this repo.

## Docs and Runbooks
- [README.md](./README.md) — current objective, state, contract, blockers, next actions.
- [LESSONS_LEARNED.md](./LESSONS_LEARNED.md) — traps and split-brain risks.
- [CHANGELOG.md](./CHANGELOG.md) — per-day refresh log.
- [AGENTS.md](./AGENTS.md) — durable-memory rule.

## Reports
- None in this repo.

## Scratch / Prototypes / History
- None in this repo.

## Source of Truth Notes
- This repo is a downstream mirror. Anything that disagrees between
  `index.html` here and fitz-rebuild's autonomous-run state, perpetual
  orchestrator log, or per-WO validation reports — fitz-rebuild wins.

## What's Confusing
- Six commits within ~5 hours can look like rapid churn, but they are just
  generator pushes after fitz-rebuild events. They do not represent any work
  in this repo.

## Durable Memory
- [README.md](./README.md) — current objective, state, contract, blockers, next actions
- [LESSONS_LEARNED.md](./LESSONS_LEARNED.md) — real failure modes and traps
- Last refreshed by repo-navigator-nightly: 2026-05-22
