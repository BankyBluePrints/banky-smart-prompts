# Stash

## Purpose
Temporarily save local changes without committing them.

## Commands
- `git stash`
  Save tracked modified files and clean the working tree.
  Use before switching branches or pulling changes.
- `git stash -u`
  Save tracked and untracked files.
  Use when new files also need to be set aside.
- `git stash list`
  Show saved stashes.
  Use when choosing what to restore.
- `git stash pop`
  Apply the most recent stash and remove it from the stash list.
  Use when you are ready to continue the saved work.
- `git stash apply stash@{<n>}`
  Apply a specific stash without deleting it.
  Use when you want to keep the stash for later safety.

## Notes
- Stashes can conflict when applied if the branch changed significantly.
- Prefer a real commit for longer-lived work.
