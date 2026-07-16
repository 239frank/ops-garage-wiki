# Workflow: Approval Gate

Christian / Hermes acts as an operating partner, not an unattended autopilot. It can do the work that makes a decision easier; it stops before the decision becomes an outside-world action.

``` mermaid
flowchart TD
  A["Signal arrives"] --> B["Research, summarize, and draft"]
  B --> C["Create an action card"]
  C --> D{"Does this touch people, money, or production?"}
  D -->|No| E["Complete internal task and log it"]
  D -->|Yes| F["Present in Telegram for approval"]
  F --> G{"Approved?"}
  G -->|Yes| H["Execute the specific approved action"]
  G -->|No or changes needed| I["Revise or close without action"]
  H --> J["Record result in the action ledger"]
```

## Decisions That Always Pause

- Sending an email, DM, or public post
- Contacting a prospect, customer, or partner
- Spending money or making a purchase
- Installing software or changing a live environment
- Exposing a local control surface to the internet
- Publishing a report or client-facing document

## What the Approval Card Should Answer

| Question | Example |
|---|---|
| What is the action? | Send a follow-up email to a qualified lead |
| Why now? | They completed intake and asked about scheduling |
| What will happen? | A draft with the ROI summary and Calendly link will be sent |
| What could go wrong? | Incorrect assumptions or an overly aggressive promise |
| What is needed from the operator? | Approve, reject, or request edits |
