# Debug GitLab Pipeline

## Purpose
Identify likely causes of GitLab pipeline failures and suggest practical debugging steps.

## Prompt
```text
Review the provided GitLab pipeline configuration, job logs, and error details to help debug the issue.

Provide:
1. Likely root cause
2. Affected job or stage
3. Why the issue is happening
4. Suggested fix
5. Steps to verify the fix

Rules:
- Prioritize the most likely causes first
- Base the answer on the provided YAML and logs
- Mention missing information if the input is incomplete
- Keep the response practical and concise
- Use GitLab CI terminology
- Do not include unrelated theory
```

## Notes
- Include failing job logs for better results
