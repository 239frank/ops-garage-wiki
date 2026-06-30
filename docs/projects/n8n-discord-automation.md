# n8n + Discord Automation

## Purpose

A workflow automation system that uses n8n to collect useful data and send clean notifications to Discord.

## Problem

A lot of home lab and personal ops work involves checking the same things repeatedly: server status, deal alerts, newly added media, exposure checks, and workflow results. Manual checking wastes time.

## Approach

Use n8n as the workflow engine and Discord as the notification layer.

Examples:

- Scheduled checks
- API pulls
- Filtering and scoring
- Normalized output
- Discord channel alerts
- Separate channels for different alert types

## Tools Used

- n8n
- Discord webhooks
- JavaScript function nodes
- Scheduled triggers
- Docker / Unraid
- API integrations

## Screenshots

Save screenshots here later:

```text
docs/assets/images/projects/n8n-discord/
```

Example Markdown once screenshots are added:

```md
![n8n workflow](../assets/images/projects/n8n-discord/workflow.png)
```

## Outcome

This project shows practical automation skills: turning repeated checks into reliable workflows with readable outputs.

## Lessons Learned

- Good alerts need filtering.
- Separate channels keep noise under control.
- Normalizing messy data is usually the hardest part.
- A workflow is only useful if it reduces human checking.
