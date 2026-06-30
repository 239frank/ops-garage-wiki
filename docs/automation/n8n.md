# n8n Workflows

n8n is used as a workflow automation platform for lab operations, alerts, API checks, and Discord notifications.

## Workflow Template

| Workflow | Purpose | Trigger | Output |
|---|---|---|---|
| Public Exposure Watch | Check public-facing endpoints | Schedule | Discord alert |
| Deal Radar | Monitor deal sources | Schedule | Discord post |
| Server Status | Check service availability | Schedule | Discord alert |
| Recently Added | Report new items from a service | Schedule/API | Discord post |

## Good Workflow Rules

- Keep one workflow focused on one job.
- Name nodes clearly.
- Keep credentials out of screenshots.
- Send alerts only when they are useful.
- Document the trigger, logic, and output.
