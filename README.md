# AI Prompt System for File Analysis & Communications

A modular set of instruction files you can feed to an AI (like Claude) to analyze uploaded files and generate specific types of communications.

## Quick Start

### Step 1: Analyze a file

Upload your file to Claude and paste the contents of `analyze.md` as your prompt. The AI will produce a structured **Analysis Output**.

**Example prompt:**
> [Upload your file]
>
> [Paste contents of analyze.md]

### Step 2: Generate a communication

Take the Analysis Output from Step 1 and paste it along with your chosen comm template.

**Example prompt:**
> Here is an analysis of a file:
>
> [Paste Analysis Output from Step 1]
>
> [Paste contents of comms/status-update.md]

### Step 3 (Optional): Customize with overrides

Add an overrides block to change the default tone, audience, length, or format:

```
### Overrides
- **Audience:** Engineering team only
- **Tone:** Casual, friendly
- **Length:** Short (3–5 bullets)
- **Format:** Slack message
```

## Available Templates

| Template | File | Best For |
|----------|------|----------|
| **Status Update** | `comms/status-update.md` | Regular progress updates to team & stakeholders |
| **Action Items** | `comms/action-items.md` | Extracting tasks with owners and deadlines |
| **Executive Summary** | `comms/executive-summary.md` | High-level summaries for leadership |
| **Meeting Notes** | `comms/meeting-notes.md` | Structured notes from meetings or discussions |

## Supported File Types

- Google Slides, Sheets, Docs
- PowerPoint, Excel, Word
- PDFs
- Images (photos, screenshots, diagrams)

## File Structure

```
├── README.md              ← You are here
├── analyze.md             ← Master file analysis instructions
└── comms/
    ├── _base.md           ← Shared defaults & override mechanism
    ├── status-update.md   ← Status/progress update template
    ├── action-items.md    ← Action item extraction template
    ├── executive-summary.md ← Executive summary template
    └── meeting-notes.md   ← Meeting notes template
```

## Tips

- You can combine templates — e.g., generate meeting notes *and* action items from the same analysis.
- For best results, do analysis and comm generation in separate steps so you can review the intermediate output.
- The override system lets you adapt any template without editing the files themselves.
