# fitz-tracker — Lessons Learned

> Durable record of real failure modes, false assumptions, misleading metrics,
> split-brain situations, and traps likely to be repeated. Maintained by
> working sessions and audited by repo-navigator-nightly.

## 2026-05-22

### Failure modes
- None observed on target day. The repo received 5 generator-driven commits
  that all completed cleanly.

### False assumptions corrected
- None recorded for target day.

### Misleading metrics / UI / reports
- The tracker `index.html` reflects whatever fitz-rebuild last pushed. If the
  fitz-rebuild loop stalls or freezes mid-WO, this page will display a
  potentially stale snapshot. Do not read this page as live truth; cross-check
  against fitz-rebuild's autonomous-run state and per-WO validation reports.

### Split-brain incidents (UI / chat / DB / docs)
- None recorded for target day.

### Active traps / checks to rerun
- Any hand-edit of `index.html` in this repo will be overwritten on the next
  fitz-rebuild generator push. If a fix is needed in the page output, fix it in
  fitz-rebuild's generator (added 2026-05-22 via `4c85b75`).
- The `<meta http-equiv="refresh" content="300">` auto-refresh in
  `index.html` means viewers will reload every 300 seconds; this is not a
  bug if the file is briefly out of sync mid-push.
