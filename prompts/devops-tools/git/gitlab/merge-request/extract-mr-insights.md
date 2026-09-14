# Extract Merge Request Insights

## Purpose

Produce a reviewer-focused assessment of a GitLab merge request without fabricating intent, test results, or repository behavior.

## Inputs

- Merge request title and description
- Diff or changed-file summary
- Linked requirement or work item, when available
- Pipeline, test, and review information
- Relevant repository conventions

## Prompt

```text
Review the following GitLab merge request using only the supplied evidence.

Merge request metadata:
<MR_METADATA>

Requirement or work item:
<REQUIREMENT_CONTEXT>

Changed files or diff:
<CHANGES>

Pipeline, tests, and comments:
<VALIDATION_CONTEXT>

Produce:
1. Purpose and scope
2. Main functional and technical changes
3. Affected components and interfaces
4. Requirement-to-change traceability
5. Risk assessment ranked High, Medium, or Low with evidence
6. Testing performed and important gaps
7. Compatibility, security, data, and deployment considerations
8. Questions or requested changes for the author
9. Recommendation: Ready, Ready with follow-ups, or Not ready

Rules:
- Distinguish confirmed facts from inference.
- Do not claim tests passed unless results are supplied.
- Do not assume unchanged files are unaffected when evidence is incomplete.
- Cite file paths or diff sections for material findings.
- State "Insufficient evidence" where a conclusion cannot be supported.
- Do not expose secrets or reproduce unnecessary sensitive content.
```

## Validation

Compare every major finding with the diff, MR discussion, pipeline results, and linked requirement before posting it as review feedback.
