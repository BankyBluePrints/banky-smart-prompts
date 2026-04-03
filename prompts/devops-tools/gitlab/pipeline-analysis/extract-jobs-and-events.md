# Extract Jobs and Events from Multiple GitLab CI Files

## Purpose
Extract job details from multiple GitLab CI configurations and generate a combined structured output.

## Prompt
Analyze the provided GitLab CI configuration files.

Each file corresponds to a project:
- File 1 → <PROJECT_1_NAME>
- File 2 → <PROJECT_2_NAME>
- File 3 → <PROJECT_3_NAME>
...
- File N → <PROJECT_N_NAME>

Extract:
Project Name, Stage, Job Name, Job Exists, Is Manual, Trigger Event, Enabled

Rules:
- Map each file to its corresponding project name
- Extract stage and job name from each GitLab CI configuration
- If a job is not present in a project, write "Job does not exist"
- If job uses "when: manual", mark Is Manual = Yes, else No
- Extract trigger events from rules / only / except / workflow
- If trigger event is unclear, write "Review required"
- Create separate rows if one job supports multiple trigger events
- Create one row per (Project + Job + Trigger Event)
- Combine all projects into a single CSV/table output
- Output must be structured and concise
- Do not add explanations

## Notes
- Replace placeholders before use
- Extend mapping if more files are provided
- Ensure correct file-to-project mapping
- Verify results before applying changes