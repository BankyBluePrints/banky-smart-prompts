# Tag

## Purpose
Create and manage tags for releases or important points in history.

## Commands
- `git tag`
  List existing tags.
  Use when reviewing available release markers.
- `git tag <tag-name>`
  Create a lightweight tag on the current commit.
  Use for simple internal markers.
  Example: `git tag v1.2.0`
- `git tag -a <tag-name> -m "<message>"`
  Create an annotated tag with metadata.
  Use for release tags that should carry author and message information.
- `git push origin <tag-name>`
  Push one tag to the remote.
  Use after creating a release tag.
- `git push origin --tags`
  Push all local tags to the remote.
  Use when multiple tags must be published.

## Notes
- Confirm the target commit before tagging, especially for release versions.
