# Contributing

## Add a prompt

1. Select the narrowest relevant category under `prompts/`.
2. Use a lowercase, hyphen-separated filename that describes the task.
3. Start from [`templates/generate-reusable-prompt.md`](templates/generate-reusable-prompt.md).
4. Use placeholders instead of personal, employer-specific, or confidential content.
5. Include inputs, expected output, constraints, and validation guidance.
6. Add the prompt to the nearest category README and, when broadly useful, to the root catalog.

## Quality checklist

- The purpose is specific and distinguishable from existing prompts.
- Required inputs are explicit.
- Missing information is not silently invented.
- Expected output is structured.
- Safety and destructive-action boundaries are included when relevant.
- Product-specific facts are not presented as timeless when they can change.
- Examples use fictional or sanitized information.
- Links and Markdown render correctly.

## Scope

Keep this repository focused on copy-and-run prompts and concise supporting references. Executable agents, skills, application code, secrets, generated reports, and organization-specific procedures belong elsewhere.
