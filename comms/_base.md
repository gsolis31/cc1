# Shared Communication Conventions

This file defines the defaults and override mechanism that all communication templates inherit.

## Default Tone & Audience by Comm Type

| Comm Type         | Default Audience            | Default Tone              |
|-------------------|-----------------------------|---------------------------|
| Status Update     | Team & stakeholders         | Professional, concise     |
| Action Items      | Team members                | Direct, clear             |
| Executive Summary | Leadership                  | Formal, high-level        |
| Meeting Notes     | Attendees & stakeholders    | Neutral, structured       |

## Override Section

Every comm template supports the following overrides. To customize, include an **Overrides** block in your prompt before or after the template:

```
### Overrides
- **Audience:** [who is this for?]
- **Tone:** [e.g., casual, formal, urgent, celebratory]
- **Length:** [e.g., short (1 paragraph), medium (half page), long (full page)]
- **Format:** [e.g., bullet points only, prose, table, email-ready]
```

If no overrides are provided, the template's stated defaults apply.

## Common Formatting Rules

All communications should follow these conventions unless overridden:

1. **Use bullet points** for lists of 3+ items — avoid long paragraphs.
2. **Keep paragraphs short** — 2–3 sentences max.
3. **Bold key names, dates, and metrics** on first mention.
4. **Use headers** to separate logical sections.
5. **Front-load the important information** — lead with the conclusion or headline, then support with details.
6. **Use plain language** — avoid jargon unless the audience expects it.
7. **Include dates in ISO format** (YYYY-MM-DD) alongside natural language where helpful.

## How to Use With Analysis Output

Each comm template expects the structured **Analysis Output** from `analyze.md` as input. The template instructions tell the AI which fields to pull from and how to transform them into the target communication format.

**Workflow:**
1. Upload your file(s) and run `analyze.md` to get the Analysis Output.
2. Pass the Analysis Output into your chosen comm template.
3. (Optional) Include an Overrides block to customize tone, audience, length, or format.
