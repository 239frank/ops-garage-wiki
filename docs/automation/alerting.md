# Alerting

This page documents alerting ideas and notification patterns.

## Alert Types

| Alert | Purpose |
|---|---|
| Public exposure | Detect unexpected reachable services |
| Container status | Know when services stop or restart |
| Server health | Track system issues |
| Security events | Surface items worth review |
| Deal alerts | Notify when criteria are met |
| Workflow failures | Know when automation breaks |

## Alert Quality Rules

- Make the alert easy to read.
- Include the thing that changed.
- Include the action needed.
- Avoid noisy repeated messages.
- Use separate channels for separate alert types.
