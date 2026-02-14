# Executive Summary

> **Default audience:** Leadership
> **Default tone:** Formal, high-level

Generate an executive summary from the provided Analysis Output. Follow the conventions in `_base.md`.

## Instructions

1. **Bottom Line Up Front (BLUF)** — Start with the single most important takeaway. This should be 1–2 sentences that a busy executive can read and immediately understand the situation. Pull from **Narrative Summary** and **Decisions & Conclusions**.
2. **Key Findings** — Distill the **Key Themes** and **Key Data Points** into 3–5 bullet points. Focus on what matters at a strategic level — skip operational detail.
3. **Implications** — What do the findings mean for the organization? Synthesize from **Decisions & Conclusions** and **Open Questions**. Connect findings to business impact.
4. **Recommended Actions** — Pull from **Action Items & Owners** and your own synthesis. Frame recommendations in terms of decisions leadership needs to make, not tasks for individual contributors.

## Output Format

```
## Executive Summary — [Topic/Project Name]
**Date:** [today's date]
**Prepared for:** [audience, default: Leadership]

### Bottom Line
[1–2 sentence BLUF]

### Key Findings
- [Finding 1]
- [Finding 2]
- [Finding 3]
- ...

### Implications
- [Implication 1]
- [Implication 2]
- ...

### Recommended Actions
1. [Recommendation 1]
2. [Recommendation 2]
3. ...
```

## Tips
- Keep the total length to **half a page or less**.
- Avoid jargon and technical detail — translate into business language.
- Quantify wherever possible (e.g., "revenue increased 15%" not "revenue went up").
- If the analysis covers multiple topics, lead with the one that has the highest business impact.
- Frame open questions as risks or decision points, not unknowns.

## Overrides
See `_base.md` for how to override audience, tone, length, or format.
