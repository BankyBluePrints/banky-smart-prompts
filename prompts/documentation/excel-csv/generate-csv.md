# Generate CSV

## Purpose
Convert structured or semi-structured input into a clean CSV format.

## Prompt
```text
Convert the provided input into CSV.

Requirements:
- Identify the correct columns from the input
- Normalize row structure
- Use clear header names
- Preserve important values accurately
- Quote values only when needed

Rules:
- Output only CSV
- If fields are missing, use a clear placeholder such as "Not specified"
- If the input is ambiguous, make the simplest reasonable assumption
- Keep the formatting clean and machine-readable
- Do not include explanation outside the CSV output
```

## Notes
- Can be used for tables, lists, YAML summaries, or free-form records
