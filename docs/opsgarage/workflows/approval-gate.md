# Workflow: Approval Gate

An approval gate makes decisions easier without turning automation into an unattended autopilot. It can do preparatory work; it stops before the decision becomes an outside-world action.

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
- Contacting an external stakeholder
- Spending money or making a purchase
- Installing software or changing a live environment
- Exposing a local control surface to the internet
- Publishing a report or stakeholder-facing document

## What the Approval Card Should Answer

| Question | Example |
|---|---|
| What is the action? | Send a reviewed project update |
| Why now? | The relevant information has been gathered and checked |
| What will happen? | A concise summary and the appropriate next steps will be sent |
| What could go wrong? | Incorrect assumptions or an incomplete recommendation |
| What is needed from the operator? | Approve, reject, or request edits |
