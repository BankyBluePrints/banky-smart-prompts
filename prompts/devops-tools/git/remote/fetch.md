# Fetch

## Purpose
Download updates from a remote without changing your current branch.

## Commands
- `git fetch`
  Download updates from the default remote.
  Use before reviewing incoming changes or rebasing.
- `git fetch origin`
  Download updates from a specific remote.
  Use when you have multiple remotes configured.
- `git fetch --all --prune`
  Fetch all remotes and remove stale remote-tracking references.
  Use during cleanup in active repositories.
- `git diff HEAD origin/<branch>`
  Compare your current branch with a fetched remote branch.
  Use after fetch to inspect incoming changes.
  Example: `git diff HEAD origin/main`

## Notes
- `git fetch` is safer than `git pull` when you want to inspect changes before integrating them.
