# Generate a Reusable Prompt

## Purpose

Create a consistent, copy-ready prompt for a repeatable task.

## Prompt

````text
Create a reusable prompt for this task:

<TASK>

Intended users:
<AUDIENCE>

Expected source material:
<INPUTS>

Required result:
<OUTPUT>

Use this Markdown structure:

# <ACTION-ORIENTED TITLE>

## Purpose
<THE SPECIFIC PROBLEM THIS PROMPT SOLVES>

## When to use
<APPROPRIATE SITUATIONS AND IMPORTANT EXCLUSIONS>

## Inputs
- <REQUIRED INPUT>
- <OPTIONAL INPUT>

## Prompt
```text
<COPY-READY PROMPT WITH DESCRIPTIVE PLACEHOLDERS>
```

## Validation
<HOW A HUMAN SHOULD VERIFY THE GENERATED RESULT>

Requirements:
- Keep the task and expected output unambiguous.
- Use descriptive placeholders instead of organization-specific values.
- Tell the model to distinguish facts, assumptions, and missing evidence.
- Include security, privacy, destructive-action, or production safeguards when relevant.
- Do not make the prompt model-specific unless the task requires a particular capability.
- Keep examples sanitized and fictional.
- Make the prompt easy to copy from rendered Markdown.
````

## Validation

Review the generated prompt against [CONTRIBUTING.md](../CONTRIBUTING.md) and [PROMPTING_GUIDE.md](../PROMPTING_GUIDE.md) before adding it to the catalog.
