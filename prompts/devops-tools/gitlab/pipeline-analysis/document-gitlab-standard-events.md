# Document GitLab Standard Pipeline Events

## Purpose
Generate documentation for standard GitLab pipeline trigger events and explain how each event can be triggered and verified.

## Prompt
```text
Provide documentation for standard GitLab pipeline trigger events.

Include these events:
- push
- merge_request_event
- tag_push
- schedule
- web
- api
- trigger
- parent_pipeline
- pipeline
- external

For each event, provide:
1. Event name
2. Short description
3. How to trigger it in GitLab
4. Expected pipeline behavior
5. How to verify it in GitLab pipeline history

Rules:
- Keep steps practical and user-friendly
- Use simple numbered steps
- Keep descriptions concise but clear
- Use GitLab terminology
- Output in well-structured Markdown
- Do not include unnecessary explanations
```

## Notes
- Review event names against your GitLab version if needed
- Keep terminology aligned with GitLab UI labels
- Verify generated documentation before sharing
