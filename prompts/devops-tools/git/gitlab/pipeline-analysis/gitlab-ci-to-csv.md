# GitLab CI to CSV

## Purpose
Extract structured data from one or more GitLab CI YAML files and convert it into clean CSV output.

## Prompt
```text
Analyze the provided GitLab CI YAML content and convert the relevant pipeline information into CSV.

Input:
- One or more GitLab CI YAML files
- Optional project names or file labels

Extract fields such as:
- Project
- Stage
- Job Name
- Trigger Type
- Manual or Automatic
- Needs / Dependencies
- Environment
- Artifacts
- Notes

Rules:
- Use placeholders if project names are not provided
- Keep one row per job unless multiple trigger types require separate rows
- Preserve field names consistently
- Mark missing or unclear values as "Not specified"
- Output only CSV unless a different format is requested
- Do not include extra explanation
```

## Notes
- Replace placeholders before use
- Adjust columns if your use case needs more job metadata
