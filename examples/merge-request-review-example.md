# Example: Merge Request Review Input

This fictional example can be used with [Extract Merge Request Insights](../prompts/devops-tools/git/gitlab/merge-request/extract-mr-insights.md).

## Merge request metadata

- Title: Add idempotency protection to payment-status callback
- Description: Reject duplicate callback processing while returning the previously recorded outcome.

## Requirement

- REQ-101: Repeated delivery of the same callback identifier must not create an additional status transition.

## Changed files

- `src/callback-handler.cs` — checks for a recorded callback identifier before processing.
- `src/callback-repository.cs` — stores callback identifier and outcome.
- `tests/callback-handler-tests.cs` — adds duplicate-delivery scenarios.

## Validation context

- Unit test output was supplied and shows the new tests passing.
- No concurrency test evidence was supplied.
- No database migration or deployment information was supplied.

## Expected review emphasis

A useful response should identify the idempotency intent, connect the changed files to REQ-101, acknowledge the supplied unit-test evidence, and flag concurrency and deployment behavior as areas needing evidence. It must not claim those areas are defective without inspecting the implementation.
