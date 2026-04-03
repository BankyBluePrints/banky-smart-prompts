# Create and Switch Branches

## Purpose
Create branches for isolated work and move between branches safely.

## Commands
- `git branch`
  List local branches.
  Use to see available branches.
- `git switch <branch>`
  Switch to an existing branch.
  Use when moving to work already in the repo.
  Example: `git switch main`
- `git switch -c <new-branch>`
  Create and switch to a new branch.
  Use when starting a feature or fix.
  Example: `git switch -c feature/report-export`
- `git branch -d <branch>`
  Delete a local branch that has already been merged.
  Use during cleanup after merge.

## Notes
- `git branch -d` refuses to delete unmerged branches.
- Use `git branch -D <branch>` only when you intentionally want to discard an unmerged local branch.
