# Auto-structure Meeting Notes (English)

## Use case
Turn rough meeting notes into a clean "Decisions / Actions / Deadlines" table.
Manual cleanup 25 min → Claude Code 30 sec.

## Prompt to paste into Claude Code

```
Please structure the following meeting notes into a table.

[Columns]
- Decision: What was decided in this meeting (past tense)
- Action (who does what): Tasks going forward, with owner
- Deadline: When the action should be completed

[Output format]
A Markdown table plus a 3-line summary of the discussion

[Meeting notes]
(paste your raw notes here)
```

## Expected output

```markdown
## Discussion Summary
- New project kickoff approved
- Initial budget of $3,000 agreed
- Mid-term review scheduled for end of May

## Actions

| Decision | Action (owner) | Deadline |
|----------|---------------|----------|
| Budget $3,000 approved | Write approval doc (Tanaka) | Apr 25 |
| PM is Yamada | First spec draft (Yamada) | May 2 |
| Mid-term review end of May | Schedule recurring meeting (Suzuki) | Apr 22 |
```

## Variations

- Need a Slack-friendly format? Add "Also provide a Slack-style summary"
- Need it in English + Japanese? Add "Also provide an English translation"
- Need it in Notion format? Add "Output as a Notion database table"

## Troubleshooting

If the notes are too short or too long, Claude Code will ask clarifying questions.
Respond with "More detail please" or "Make it shorter" to adjust.
