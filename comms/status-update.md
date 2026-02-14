# Status Update

> **Default audience:** Team & stakeholders
> **Default tone:** Professional, concise

Generate a status update communication from the provided Analysis Output. Follow the conventions in `_base.md`.

## Instructions

1. **Headline Summary** — Write a single sentence or short paragraph that captures the most important takeaway. This should answer: "What's the current state?"
2. **Progress Since Last Update** — Pull from **Key Data Points**, **Decisions & Conclusions**, and **Dates & Milestones** in the Analysis Output. Highlight what has been completed or advanced.
3. **Blockers & Risks** — Pull from **Open Questions** and any items in **Action Items & Owners** that appear overdue or at risk. If none exist, state "No current blockers."
4. **Next Steps** — Pull from **Action Items & Owners** and any forward-looking items in **Key Themes**. List the immediate next actions with owners if known.

## Output Format

```
## Status Update — [Topic/Project Name]
**Date:** [today's date]

### Headline
[1–2 sentence summary of the current state]

### Progress
- [Completed or advanced item 1]
- [Completed or advanced item 2]
- ...

### Blockers & Risks
- [Blocker or risk 1]
- [Blocker or risk 2]
- ...

### Next Steps
- [ ] [Action] — **[Owner]** (by [date] if known)
- [ ] [Action] — **[Owner]**
- ...
```

## Tips
- Keep the total length under one page / one screen.
- Use checkboxes (`- [ ]`) for next steps to make them actionable.
- If the analysis covers multiple workstreams, group progress and next steps by workstream.

## Overrides
See `_base.md` for how to override audience, tone, length, or format.
