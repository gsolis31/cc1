# Action Items

> **Default audience:** Team members
> **Default tone:** Direct, clear

Extract and organize actionable tasks from the provided Analysis Output. Follow the conventions in `_base.md`.

## Instructions

1. **Context Line** — Write 1–2 sentences explaining where these action items come from (e.g., "From the Q4 planning deck reviewed on 2025-01-15").
2. **Action Items Table** — Pull from **Action Items & Owners**, **Decisions & Conclusions** (which often imply follow-up tasks), and **Open Questions** (which may need someone to investigate). For each item, assign:
   - **Owner** — the person responsible (use name from analysis or mark as TBD)
   - **Task** — clear, specific description starting with a verb
   - **Deadline** — from the analysis or mark as TBD
   - **Priority** — High / Medium / Low, inferred from context and urgency signals
3. **Dependencies** — Note any items that depend on other items completing first, or on external inputs.

## Output Format

```
## Action Items — [Source/Project Name]
**Extracted from:** [file name or meeting/context]
**Date:** [today's date]

### Context
[1–2 sentence description of the source]

### Tasks

| # | Owner | Task | Deadline | Priority |
|---|-------|------|----------|----------|
| 1 | ...   | ...  | ...      | ...      |
| 2 | ...   | ...  | ...      | ...      |

### Dependencies
- Task [#] depends on [task/external input]
- ...

### Notes
- [Any additional context needed to act on these items]
```

## Tips
- Each task should be **specific and actionable** — start with a verb (e.g., "Draft the proposal," not "Proposal").
- If an owner is not clear from the analysis, mark as **TBD** and flag it.
- Default priority to **Medium** unless there are clear urgency signals (deadlines, escalation language, blockers).
- Group related tasks together when possible.

## Overrides
See `_base.md` for how to override audience, tone, length, or format.
