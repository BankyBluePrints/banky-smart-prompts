# General-Purpose Prompt Starters

## Purpose

Provide compact starting prompts for common tasks when a more specialized repository prompt is not available.

## Required practice

- Replace all placeholders.
- Provide the source material needed for the task.
- Ask the model to identify missing information instead of inventing it.
- Verify factual, technical, or consequential output before use.

## Explain a concept

```text
Explain <TOPIC> for <AUDIENCE_LEVEL>.

Include:
- a plain-language definition;
- one relevant analogy;
- one concrete example;
- common misconceptions;
- key takeaways.

State any assumptions and do not invent facts when context is missing.
```

## Structure raw notes

```text
Convert <RAW_NOTES> into a structured <DOCUMENT_TYPE>.

Requirements:
- preserve confirmed facts and decisions;
- separate assumptions and open questions;
- remove repetition without losing meaning;
- use descriptive headings and concise language;
- list information that needs confirmation.
```

## Diagnose an issue

```text
Analyze this issue using only the supplied evidence.

Context:
<CONTEXT>

Observed behavior:
<OBSERVED_BEHAVIOR>

Logs or errors:
<LOGS_OR_ERRORS>

Provide:
1. Evidence summary
2. Ranked possible causes
3. Safe diagnostic checks
4. Recommended fix, if supported
5. Verification steps
6. Remaining uncertainty

Do not claim a confirmed root cause unless the evidence supports it.
```

## Compare alternatives

```text
Compare <OPTION_A> and <OPTION_B> for <USE_CASE>.

Evaluate:
- suitability;
- benefits and limitations;
- implementation and operating cost;
- security and reliability;
- migration or lock-in risk.

State the assumptions, recommend an option, and explain when the recommendation would change.
```

## Summarize source material

```text
Summarize <SOURCE_MATERIAL> for <AUDIENCE>.

Include:
- central message;
- key facts and decisions;
- risks or caveats;
- unresolved questions;
- concise next actions, if present.

Do not add claims that are absent from the source.
```

## Draft a professional message

```text
Draft a <MESSAGE_TYPE> for <AUDIENCE> about <PURPOSE>.

Tone: <TONE>
Length: <LENGTH>
Required facts: <FACTS>
Requested action: <ACTION>

Keep it direct and professional. Do not invent dates, commitments, names, or approvals.
```
