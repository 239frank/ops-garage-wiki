# Ops Garage Wiki
## Frank Garcia | Applied AI, Automation & IT Operations

A public technical portfolio documenting how I build, connect, and operate practical systems. The wiki brings together project write-ups, architecture decisions, workflow patterns, and lessons learned across AI-assisted operations, automation, cybersecurity, and self-hosted infrastructure.

**[Explore the published wiki →](https://ops-garage-wiki.pages.dev/)**  
**[Visit Ops Garage AI →](https://opsgarageai.com/)** · **[Browse the project portfolio](docs/projects/index.md)**

The published wiki is hosted on Cloudflare Pages. This repository contains its documentation source; OpsGarageAI.com is the separate business website.

## Start Here

For hiring managers, collaborators, and technical reviewers, these pages provide a quick view of the work:

| Project or practice | What it demonstrates |
| --- | --- |
| [n8n + Discord Automation](docs/projects/n8n-discord-automation.md) | Connecting operational data, repeatable workflows, scheduled reporting, and team notifications. |
| [AI Content Review Workflow](docs/opsgarage/workflows/margo-content-loop.md) | Structuring AI-assisted content work around review and approval. |
| [Workflow Design](docs/opsgarage/stories/lead-engine.md) | Turning unstructured information into a clear brief and next action. |
| [GRC LLM Lab](docs/projects/grc-llm.md) | Exploring local AI support for governance, risk, and compliance work. |
| [Compliance Evidence Practice](docs/opsgarage/stories/compliance-copilots.md) | Organizing evidence and preparing reviewable material for human decisions. |
| [Public Exposure Watch](docs/projects/public-exposure-watch.md) | Comparing public-facing infrastructure signals with documented baselines. |
| [Home Lab Operations](docs/projects/home-lab-ops.md) | Operating self-hosted infrastructure, containers, monitoring, and supporting services. |
| [Personal Wiki Build](docs/projects/personal-wiki.md) | Building and maintaining this version-controlled technical knowledge base. |

## What You Will Find

- **Applied AI and automation:** workflow design, AI-assisted analysis and drafting, approval patterns, n8n integrations, and Discord reporting.
- **Cybersecurity and compliance:** lab projects and working notes on control evidence, the Risk Management Framework, authorization, and security operations.
- **Infrastructure and operations:** Unraid, Docker, networking, monitoring, and troubleshooting practices.
- **Project evidence and documentation:** the problem, approach, tools, tradeoffs, and lessons behind individual builds.

The collection includes hands-on implementations, lab experiments, and design patterns. Individual pages describe their scope; prototypes and technical notes are not presented as production certifications or guaranteed business outcomes.

## How I Approach the Work

I focus on making systems useful, understandable, and maintainable:

1. Start with the operational problem and the people doing the work.
2. Connect the tools and data needed for a practical solution.
3. Keep review points, ownership, and failure handling visible.
4. Document the decisions so the system can be supported and improved.

See the [operating principles](docs/opsgarage/principles.md) and [approval design](docs/opsgarage/workflows/approval-gate.md) for more detail.

## About This Repository

The wiki is built with **MkDocs**, **Material for MkDocs**, and **Markdown**, versioned in **GitHub**, and published through **Cloudflare Pages**.

- `docs/` contains the source pages and supporting assets.
- `mkdocs.yml` defines navigation and site configuration.
- `requirements.txt` lists the Python documentation dependencies.
- `site/` contains generated static-site output.

For the documentation itself, start with the [published wiki](https://ops-garage-wiki.pages.dev/) or [portfolio index](docs/projects/index.md). For the business and its services, visit [Ops Garage AI](https://opsgarageai.com/).
