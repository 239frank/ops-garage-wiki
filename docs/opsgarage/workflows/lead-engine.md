# Workflow: Intake and Work Routing

This workflow shows how unstructured requests can become a prepared internal brief without turning automation into an unattended decision-maker.

``` mermaid
flowchart LR
  A["Request or intake"] --> B["Call or form capture"]
  B --> C["Structured record"]
  C --> D["Transcript and structured notes"]
  D --> E["n8n + OpenAI analysis"]
  E --> F["Brief and draft recommendation"]
  F --> G{"Owner review"}
  G -->|Approved| H["Appropriate next action"]
  G -->|Needs work| E
```

## What Happens

1. A request arrives through a call, form, or shared work queue.
2. The input is captured and structured into a usable record.
3. The analysis layer identifies relevant context, dependencies, and likely next steps.
4. The system prepares a brief, supporting material, and a draft recommendation.
5. A responsible owner reviews the work before anything leaves the internal workflow.
6. The approved next step is documented and routed appropriately.

## Current Components

| Component | Role |
|---|---|
| Form or call capture | Records the initial request and context |
| n8n | Routes structured intake, analysis, and reporting tasks |
| OpenAI analysis | Converts raw input into an operational readout |
| Structured workbook | Maintains work items and supporting calculations |
| Communication draft | Holds reviewable next-step language |

!!! note "Why the review step matters"
    A draft recommendation is a starting point, not a decision. The owner reviews the context, assumptions, and recommendation before it becomes an external action.
