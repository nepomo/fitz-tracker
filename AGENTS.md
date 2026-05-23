# Agent Guidance — fitz-tracker

## Durable Repo Memory (non-negotiable)

Every active lane in this repo must keep `README.md` and `LESSONS_LEARNED.md` at the repo root — and at each active sub-lane root in monorepos — current with real evidence.

Refresh cadence:
- at least once per hour during active work
- at every major commit boundary
- before any handoff or stand-down if the lane state changed

`README.md` must hold: current objective, current state, durable contract / source of truth, blockers, next actions, key commits and migrations, out of scope.

`LESSONS_LEARNED.md` must hold: real failure modes, false assumptions, misleading metrics, split-brain situations between UI / chat / DB / docs, and traps likely to be repeated.

Do NOT leave the latest truth only in chat. If repo docs are stale, refresh them before continuing. The nightly sweep (`repo-navigator-nightly`) fails closed when it finds drift.

## Repo-specific note

This repo is a write-only mirror. The generator lives in
[`fitz-rebuild`](../fitz-rebuild) (added 2026-05-22 in commit `4c85b75`). Do
NOT hand-edit `index.html` here; the next generator push will overwrite it.
Any UI / template fix belongs in fitz-rebuild's generator, not this repo.
