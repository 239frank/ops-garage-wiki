# Workflow: Lead Engine

The lead engine turns an interested local operator into a prepared conversation, without pretending that automation should close the deal on its own.

``` mermaid
flowchart LR
  A["Discovery: website, Hermes, Google Places"] --> B["Call or intake form"]
  B --> C["Retell AI or form capture"]
  C --> D["Transcript and structured notes"]
  D --> E["n8n + OpenAI analysis"]
  E --> F["ROI worksheet and draft report"]
  F --> G{"Operator review"}
  G -->|Approved| H["Professional follow-up + Calendly"]
  G -->|Needs work| E
```

## What Happens

1. A prospect is discovered through the site, a targeted lead list, or local search.
2. They call the AI assistant or submit a short intake form.
3. The call is transcribed or the form is structured into a usable record.
4. The analysis layer looks for operational friction, likely automation opportunities, and potential ROI.
5. The system prepares the worksheet, report material, and a follow-up draft.
6. Frank reviews the finding before anything goes out.
7. The approved next step is a professional follow-up and a scheduling link.

## Current Components

| Component | Role |
|---|---|
| Retell AI | Captures the initial call and callback flow |
| n8n | Routes the intake, analysis, and reporting workflow |
| OpenAI analysis | Converts raw intake into an operational readout |
| Google Sheets | Stores leads and ROI calculations |
| Outlook | Holds draft follow-up communication |
| Calendly | Handles the approved conversation handoff |

!!! note "Why the review step matters"
    An ROI estimate is a conversation starter, not a promise. The operator reviews the context, the math, and the recommendation before it becomes client-facing.
