# Log

## Purpose
Inspect commit history and understand what changed over time.

## Commands
- `git log`
  Show commit history for the current branch.
  Use for a full chronological review.
- `git log --oneline --graph --decorate`
  Show compact history with branch and merge structure.
  Use for day-to-day history inspection.
- `git log -- <path>`
  Show commit history for one file or directory.
  Use when tracing changes to a specific area.
  Example: `git log -- src/api`
- `git show <commit>`
  Show the details of one commit.
  Use when reviewing a specific change.

## Notes
- Pair `git log` with `git diff` when you need both history and file-level detail.
