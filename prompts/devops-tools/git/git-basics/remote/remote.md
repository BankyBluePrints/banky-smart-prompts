# Remote

## Purpose
Manage remote repository connections such as `origin` and additional upstream remotes.

## Commands
- `git remote -v`
  List remotes and their fetch and push URLs.
  Use when checking where your repository syncs.
- `git remote add <name> <url>`
  Add a new remote.
  Use when connecting to another repository source.
  Example: `git remote add upstream https://github.com/org/project.git`
- `git remote rename <old> <new>`
  Rename an existing remote.
  Use when standardizing remote names.
- `git remote remove <name>`
  Remove a remote entry.
  Use when a remote is no longer needed.

## Notes
- Verify remote URLs before pushing to avoid sending commits to the wrong repository.
