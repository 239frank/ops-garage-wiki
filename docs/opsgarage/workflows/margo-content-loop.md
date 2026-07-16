# Workflow: Content Review

This is a draft-first content workflow. The system helps create the work, and the responsible editor keeps editorial control.

``` mermaid
flowchart LR
  A["Content schedule"] --> B["Select topic from content workbook"]
  B --> C["Draft post"]
  C --> D["Save to Draft_Posts"]
  D --> E["Telegram review"]
  E --> F{"Approved?"}
  F -->|Yes| G["Publish through the approved channel"]
  F -->|No| H["Reject or revise"]
```

## Guardrails

The schedule creates a dependable publishing habit, not permission to publish without context. Each draft is checked for accuracy, tone, specific claims, and whether it represents the work honestly.
