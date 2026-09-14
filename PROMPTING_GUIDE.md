# Prompting and Safety Guide

## Use placeholders deliberately

Replace placeholders such as `<TASK>`, `<FILE_CONTENT>`, and `<EXPECTED_OUTPUT>` before submitting a prompt. If required information is unavailable, instruct the model to identify the gap rather than invent a value.

## Provide evidence

Supply the smallest relevant source set: configuration, logs, diff, requirements, sample input, or documentation. Label each source clearly and distinguish authoritative input from background context.

## Protect sensitive information

Do not submit:

- passwords, keys, tokens, certificates, or connection strings;
- personal, customer, payment, or health data;
- confidential source code or internal documents to unapproved services;
- production data, private URLs, or organization-specific identifiers when a sanitized example is sufficient.

Follow the data-classification, retention, and AI-use policies of the environment where the prompt is used.

## Require uncertainty to remain visible

A reusable prompt should tell the model to:

- distinguish facts from assumptions;
- say when evidence is missing or contradictory;
- avoid inventing files, functions, requirements, results, approvals, or tool output;
- mark recommendations that require current product-documentation verification.

## Control risky actions

For code, command, Git, infrastructure, database, or deployment tasks:

1. Ask for analysis before mutation when the impact is unclear.
2. Prefer reversible steps.
3. Identify the exact target and affected files or resources.
4. Include verification and rollback guidance.
5. Require explicit human approval for destructive or production actions.

## Validate the response

Before using generated output:

- compare it with the supplied source;
- run tests, linters, parsers, or dry runs where available;
- check version-sensitive syntax against official documentation;
- review security, privacy, compatibility, and operational impact;
- confirm that commands target the intended repository, branch, environment, or resource.

## Keep prompts tool-aware but reusable

Use tool-specific terminology when the task depends on GitHub, GitLab, Confluence, Python, or another platform. Avoid unnecessary model-specific wording so the prompt can still work across capable assistants.
