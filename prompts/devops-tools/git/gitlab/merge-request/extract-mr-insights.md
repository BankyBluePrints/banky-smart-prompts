# Extract Merge Request Insights

## Purpose
Summarize a GitLab merge request into key changes, risks, and review points.

## Prompt
```text
Analyze the provided GitLab merge request details and produce a concise summary.

Include:
- Merge request title
- Goal of the change
- Main files or modules affected
- Key functional changes
- Risks or review concerns
- Testing or validation mentioned
- Recommended follow-up questions if needed

Rules:
- Keep the summary concise and structured
- Focus on reviewer-relevant information
- Use placeholders if metadata is missing
- Avoid repeating raw diff content unless necessary
- Do not include unnecessary explanation
```

## Notes
- Works well with MR description, diff summary, and comments
