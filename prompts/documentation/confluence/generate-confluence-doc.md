# Generate Confluence-Ready Documentation

## Purpose

Transform source material into a structured document suitable for review and later publication in Confluence.

## Inputs

- Document purpose and audience
- Confirmed source material
- Required document type or section structure
- Decisions, owners, dates, and links that must be preserved
- Known assumptions and open questions

## Prompt

```text
Create a Confluence-ready <DOCUMENT_TYPE> for <AUDIENCE> from the supplied source.

Source material:
<SOURCE_MATERIAL>

Required sections:
<REQUIRED_SECTIONS>

Produce:
- a clear title and summary;
- context and scope;
- structured technical or business detail;
- decisions and rationale;
- risks, dependencies, and constraints;
- assumptions and open questions;
- actions with owners and dates only when supplied;
- references to the original source.

Rules:
- Preserve confirmed facts and intended meaning.
- Separate facts, decisions, assumptions, and open questions.
- Do not invent owners, dates, approvals, metrics, links, or system behavior.
- Mark missing information as "To be confirmed".
- Use concise headings, tables, and lists where they improve readability.
- Do not include confidential information that is unnecessary for the document.
```

## Validation

Ask the document owner to verify accuracy, access classification, decisions, action ownership, and links before publication.
