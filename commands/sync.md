---
description: One command for everything. Adapts based on time and context.
---

## Setup

1. Read `## File Locations` from CLAUDE.md/AGENTS.md for paths
2. Read NOW.md silently
3. Run: `date '+%A %B %d, %Y %H:%M'`

## Adapt Based on Time

| Time | Default Mode | Question |
|------|--------------|----------|
| Before 11am | Start | "What would make today a win?" |
| 11am - 6pm | Check | "What are you doing right now?" |
| After 6pm | End | "What happened today?" |

Ask the one question. Wait.

## Then

Infer what they need from their response:
- If they answer with a task -> they're starting, update MIT
- If they're venting or stuck -> help them, redirect if needed
- If they're reflecting -> it's an end-day, capture to Memory Log
- If they say "actually I want to plan tomorrow" -> switch modes

The time is a hint, not a rule. Their response determines the flow.

## Update

- NOW.md: MIT, Memory Log, or both depending on mode
- Only update what's meaningful

## Don't

- Ask multiple questions
- Be rigid about the time-based mode
- Force a reflection if they just want to check in
