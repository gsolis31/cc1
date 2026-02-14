# Meeting Notes

> **Default audience:** Attendees & stakeholders
> **Default tone:** Neutral, structured

Generate structured meeting notes from the provided Analysis Output. Follow the conventions in `_base.md`.

## Instructions

1. **Meeting Metadata** — Pull date, attendees, and agenda from the **File Metadata** and **Key Themes**. If not explicitly stated, infer from context or mark as unknown.
2. **Discussion Summary** — Organize the **Key Themes** and **Key Data Points** into a coherent summary of what was discussed. Group by topic or agenda item.
3. **Decisions Made** — Pull directly from **Decisions & Conclusions**. Each decision should be stated clearly and attributed if possible.
4. **Action Items** — Pull from **Action Items & Owners**. Use the same table format as the action-items template.
5. **Next Meeting / Follow-ups** — Pull from **Dates & Milestones** and any forward-looking **Open Questions**. Note the next meeting date if known.

## Output Format

```
## Meeting Notes — [Meeting Title/Topic]

### Metadata
- **Date:** [meeting date]
- **Attendees:** [list of attendees]
- **Agenda:** [list of agenda topics]

### Discussion Summary

#### [Topic/Agenda Item 1]
- [Key point]
- [Key point]

#### [Topic/Agenda Item 2]
- [Key point]
- [Key point]

### Decisions
- [Decision 1] *(decided by [person] if known)*
- [Decision 2]
- ...

### Action Items

| # | Owner | Task | Deadline |
|---|-------|------|----------|
| 1 | ...   | ...  | ...      |
| 2 | ...   | ...  | ...      |

### Follow-ups
- **Next meeting:** [date if known]
- [Open question or follow-up item 1]
- [Open question or follow-up item 2]
```

## Tips
- Keep discussion summaries **factual and neutral** — report what was said, not your interpretation.
- Attribute opinions and decisions to individuals when the source material makes this clear.
- If the source file is a presentation or document (not literal meeting notes), frame the output as notes *about* the content rather than pretending a meeting occurred.
- Keep action items crisp — they should be copy-pasteable into a task tracker.

## Overrides
See `_base.md` for how to override audience, tone, length, or format.
