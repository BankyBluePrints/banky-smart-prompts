# Debug GitLab Pipeline

## Purpose

Diagnose a failed GitLab pipeline from configuration and job evidence, prioritizing safe investigation before changes.

## Inputs

- Relevant `.gitlab-ci.yml` and included configuration
- Failing pipeline source and branch or tag
- Failed job name, stage, and logs
- Recent configuration or dependency changes
- Runner, image, environment, and variable context when relevant

Remove tokens, secrets, credentials, private URLs, and sensitive values from logs before sharing them.

## Prompt

```text
Diagnose this GitLab pipeline failure using only the supplied configuration and logs.

Pipeline context:
<PIPELINE_CONTEXT>

CI configuration:
<CI_CONFIGURATION>

Failed job logs:
<SANITIZED_JOB_LOGS>

Recent changes:
<RECENT_CHANGES>

Provide:
1. Evidence summary
2. Most likely root cause and confidence
3. Other plausible causes
4. Safe diagnostic checks in recommended order
5. Minimal proposed fix
6. Verification plan
7. Rollback approach
8. Missing evidence

Rules:
- Cite the relevant job, rule, include, variable, or log line.
- Do not invent variable values, runner behavior, artifacts, or job results.
- Distinguish configuration issues from runner, dependency, permission, or environment failures.
- Prefer read-only checks and reversible fixes.
- Do not recommend exposing protected or masked variables.
- Flag version-sensitive GitLab behavior for official-documentation verification.
```

## Validation

Test the fix on a non-production branch or isolated pipeline where possible. Confirm the intended pipeline sources still run and unintended sources remain blocked.
