# Banky Smart Prompts

A curated library of reusable, copy-ready prompts and practical Git references for software engineering, DevOps, documentation, programming, and productivity.

The collection favors explicit inputs, structured outputs, reusable placeholders, and human verification over vague one-line instructions.

## Start here

1. Browse the [prompt catalog](prompts/README.md).
2. Choose the prompt closest to your task.
3. Replace every `<PLACEHOLDER>` with relevant, non-sensitive context.
4. Remove sections that do not apply.
5. Review the generated result before using it in code, documentation, pipelines, or operational work.

Read the [prompting and safety guide](PROMPTING_GUIDE.md) before using the prompts with confidential, destructive, security-sensitive, or production-related work.

## Prompt catalog

| Category | Examples |
| --- | --- |
| [AI and general tasks](prompts/ai-tools/) | Explain, summarize, compare, structure, and troubleshoot |
| [Git and DevOps](prompts/devops-tools/git/) | Git reference, GitLab MR analysis, and pipeline inspection |
| [Documentation](prompts/documentation/) | Confluence-ready documents and CSV generation |
| [Programming](prompts/programming/) | Practical code-generation prompts |
| [Productivity](prompts/productivity/) | Turn rough ideas into actionable plans |

## Featured prompts

- [Extract GitLab merge request insights](prompts/devops-tools/git/gitlab/merge-request/extract-mr-insights.md)
- [Debug a GitLab pipeline](prompts/devops-tools/git/gitlab/pipeline-analysis/debug-pipeline.md)
- [Explain a GitLab CI configuration](prompts/devops-tools/git/gitlab/pipeline-analysis/explain-gitlab-ci.md)
- [Generate Confluence-ready documentation](prompts/documentation/confluence/generate-confluence-doc.md)
- [Generate practical Python code](prompts/programming/python/generate-python-code.md)
- [Convert an idea into an action plan](prompts/productivity/task-planning/idea-to-steps.md)

## What a good prompt contains

- **Purpose:** the problem it solves.
- **Inputs:** the context the user must supply.
- **Task:** the work the model should perform.
- **Output:** the required structure and level of detail.
- **Constraints:** boundaries, exclusions, and assumptions.
- **Validation:** how a human should check the result.

Use the [reusable prompt generator](templates/generate-reusable-prompt.md) to create new entries consistently.

## Examples

The [`examples/`](examples/) directory shows how placeholders can be filled with sanitized data. Examples are demonstrations, not authoritative technical output.

## Repository boundaries

This repository contains **prompts and reference material**, not autonomous agents or agent skills. Executable tools, permissions, orchestration, and lifecycle behavior belong in the owning application or agent project.

## Responsible use

- Never paste credentials, tokens, customer data, proprietary source code, internal URLs, or other restricted information into an unapproved AI service.
- Treat generated commands, scripts, configurations, and conclusions as drafts.
- Verify claims against source material and current product documentation.
- Inspect the working tree and target before destructive Git or filesystem operations.
- Use approved tools and follow the policies of the environment in which the prompt is executed.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for naming, structure, review, and confidentiality rules.

## License

Licensed under the [MIT License](LICENSE).
