# Generate Python Code

## Purpose

Generate a small, testable Python solution for a clearly defined task.

## Inputs

- Task and expected behavior
- Input and output format
- Python version and execution environment
- Dependency constraints
- Representative examples and edge cases

## Prompt

```text
Implement the following task in Python.

Task:
<TASK>

Input format:
<INPUT_FORMAT>

Expected output:
<OUTPUT_FORMAT>

Constraints and edge cases:
<CONSTRAINTS>

Environment:
- Python version: <VERSION>
- Allowed dependencies: <DEPENDENCIES>

Provide:
1. Brief approach
2. Complete code
3. Tests covering normal, boundary, and invalid input
4. Example execution
5. Assumptions and limitations

Rules:
- Prefer the standard library unless a dependency is justified.
- Validate untrusted input and handle failures explicitly.
- Do not embed secrets, credentials, private URLs, or machine-specific paths.
- Avoid destructive filesystem, network, or system actions unless explicitly required and clearly guarded.
- Keep functions focused, names descriptive, and comments limited to non-obvious reasoning.
- Do not claim the code was executed unless execution evidence is provided.
```

## Validation

Run the tests in the target Python version, review dependency and security implications, and verify behavior with representative real inputs before adoption.
