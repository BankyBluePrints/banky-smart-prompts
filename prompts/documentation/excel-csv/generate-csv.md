# Generate CSV

## Purpose

Convert structured or semi-structured input into valid, consistently shaped CSV without silently inventing missing values.

## Prompt

```text
Convert the supplied data into CSV.

Input:
<SOURCE_DATA>

Required columns:
<COLUMN_LIST_OR_INFER>

Missing-value representation:
<EMPTY_OR_PLACEHOLDER>

Rules:
- Preserve source values accurately.
- Use one consistent header row and column order.
- Create one row per logical record.
- Escape fields according to standard CSV rules.
- Quote fields containing commas, quotes, or line breaks.
- Represent missing values using the specified convention.
- Do not infer or calculate values unless explicitly requested.
- If record boundaries or columns are ambiguous, describe the ambiguity before generating the CSV.
- Output the final CSV in a fenced csv block with no commentary inside the block.
```

## Validation

Check row counts, column counts, escaping, encoding, and a sample of source-to-output values before importing the CSV.
