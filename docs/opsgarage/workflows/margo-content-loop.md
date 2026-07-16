# Workflow: Margo Content Loop

Margo is the content engine for a steady LinkedIn rhythm. It is deliberately draft-first: the system creates the work, and the operator keeps editorial control.

``` mermaid
flowchart LR
  A["Monday, Wednesday, Friday schedule"] --> B["Select topic from content workbook"]
  B --> C["Draft post"]
  C --> D["Save to Draft_Posts"]
  D --> E["Telegram review"]
  E --> F{"Approve?"}
  F -->|Yes| G["Publish to LinkedIn"]
  F -->|No| H["Reject or revise"]
```

## Review Commands

- `/margo approve <draft_id>` sends the approved draft through the publishing flow.
- `/margo reject <draft_id>` keeps it out of the public queue.

## Guardrails

The schedule creates a dependable publishing habit, not permission to publish without context. Each draft is checked for accuracy, tone, specific claims, and whether it represents the work honestly.
