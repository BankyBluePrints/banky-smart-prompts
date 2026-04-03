# Add and Commit

## Purpose
Stage changes and create commits with clear history entries.

## Commands
- `git add <file>`
  Stage a specific file.
  Use when you want to commit only selected changes.
  Example: `git add src/app.py`
- `git add .`
  Stage all tracked and untracked changes in the current directory tree.
  Use when all current changes belong in the same commit.
- `git commit -m "<message>"`
  Create a commit from staged changes.
  Use after reviewing what is staged.
  Example: `git commit -m "Fix login validation"`
- `git commit -am "<message>"`
  Stage modified tracked files and commit in one step.
  Use for quick commits when no new files need to be added.

## Notes
- `git commit -am` does not include new untracked files.
- Review staged changes with `git diff --cached` before committing when the change set matters.
