# Restore

## Purpose
Discard working tree changes or unstage files using the modern restore command.

## Commands
- `git restore <file>`
  Discard unstaged changes in a file.
  Use when you want to revert a file to the last committed state.
  Example: `git restore README.md`
- `git restore --staged <file>`
  Unstage a file while keeping its local edits.
  Use when the file should not be part of the next commit.
- `git restore --source=<commit> <file>`
  Restore a file from a specific commit.
  Use when recovering an earlier file version without resetting the whole branch.

## Notes
- `git restore` changes the working tree, so check `git status` first.
- Restoring a file overwrites local changes in that file.
