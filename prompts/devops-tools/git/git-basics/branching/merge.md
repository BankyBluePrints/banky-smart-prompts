# Merge

## Purpose
Combine changes from one branch into another.

## Commands
- `git merge <branch>`
  Merge the specified branch into the current branch.
  Use when integrating completed work.
  Example: `git merge feature/api-cleanup`
- `git merge --no-ff <branch>`
  Create an explicit merge commit even if a fast-forward is possible.
  Use when you want branch history to remain visible.
- `git merge --abort`
  Cancel an in-progress merge and return to the pre-merge state.
  Use when conflict resolution should be abandoned.

## Notes
- Run merges from the target branch, such as `main` or your release branch.
- Resolve conflicts carefully before completing the merge.
