# GRC LLM

## Summary

The GRC LLM project explores how a local AI assistant can support compliance workflows such as control review, evidence organization, SAR review, POA&M support, and RMF/ATO documentation.

The emphasis is on workflow support, not replacing human judgment. The system is designed to help organize information, summarize control language, and assist with compliance-focused analysis.

## Problem

GRC and RMF work often involves large amounts of documentation:

- Control language
- Assessment procedures
- System descriptions
- Evidence files
- SAR notes
- POA&M entries
- Risk decisions
- Authorization package material

That information can be difficult to search, summarize, and compare manually. A local assistant can help speed up review and organization when the source material is controlled and the output is checked by a human.

## Approach

The lab focuses on a local workflow where compliance material can be uploaded, searched, summarized, and reviewed.

Core use cases include:

1. Reviewing control language.
2. Mapping evidence to control requirements.
3. Summarizing SAR or assessment notes.
4. Organizing POA&M-related information.
5. Asking compliance-focused questions against uploaded reference material.
6. Drafting plain-language summaries for review.

## Tools and Concepts

- Local LLM environment
- Open WebUI
- Docker / Unraid deployment
- GPU-assisted local processing
- Markdown-based control packets
- RMF / ATO workflow concepts
- NIST SP 800-53 study
- Evidence organization
- Source-grounded review

## What This Demonstrates

- GRC workflow understanding
- Local AI experimentation
- Compliance documentation awareness
- Control interpretation
- Evidence mapping concepts
- Practical AI use with human review
- Ability to connect emerging technology to real governance workflows

## Outcome

This project demonstrates a practical approach to using local AI as a compliance support tool. The value is in organizing information, speeding up review, and helping create better summaries while keeping human judgment in the loop.

## Screenshot Opportunities

| Screenshot | What It Proves |
|---|---|
| Open WebUI interface | Shows local AI environment |
| Uploaded source/document view | Shows source-based workflow |
| Example control question | Shows compliance-focused use case |
| Example response | Shows review and summarization capability |
| Container/deployment view | Shows self-hosted implementation |

## Screenshot Folder

Save screenshots here:

`docs/assets/images/projects/grc-llm/`

Recommended filenames:

- `open-webui.png`
- `source-documents.png`
- `control-question.png`
- `example-response.png`
- `deployment-view.png`

## Public Safety Notes

Use generic sample controls and non-sensitive documents for public screenshots. Do not show private system names, internal packages, official documents, usernames, keys, tokens, or sensitive environment details.
