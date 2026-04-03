# Reset

## Purpose
Move `HEAD` and optionally unstage or discard changes.

## Commands
- `git reset <file>`
  Unstage a file while keeping its working tree changes.
  Use when you added something by mistake.
  Example: `git reset src/app.py`
- `git reset --soft HEAD~1`
  Remove the last commit but keep all changes staged.
  Use when the last commit message or content should be redone.
- `git reset --mixed HEAD~1`
  Remove the last commit and keep changes unstaged.
  Use when you want to recommit in a different shape.
- `git reset --hard HEAD~1`
  Remove the last commit and discard all associated local changes.
  Use only when you are certain the discarded work is not needed.

## Notes
- `git reset --hard` is destructive and permanently removes local uncommitted work from the working tree.
- Avoid resetting shared branch history unless you understand the impact on collaborators.
