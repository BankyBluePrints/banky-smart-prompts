# Explain GitLab CI

## Purpose
Explain a GitLab CI YAML file in simple terms so users can understand stages, jobs, and execution flow.

## Prompt
```text
Explain the provided GitLab CI YAML configuration in clear, practical language.

Cover:
- Overall pipeline purpose
- Stages and execution order
- Key jobs and what each job does
- Important rules, only/except, or workflow logic
- Variables, artifacts, dependencies, and environments if present
- Potential risks, confusing areas, or assumptions

Rules:
- Use GitLab terminology
- Keep the explanation concise but useful
- Use headings and short bullet points
- If something is unclear, say "Needs review"
- Do not rewrite the YAML unless requested
```

## Notes
- Best used with complete `.gitlab-ci.yml` content
