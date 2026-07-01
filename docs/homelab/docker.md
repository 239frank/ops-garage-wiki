# Docker Stack

## Summary

This page tracks containerized services, ports, purposes, and rebuild notes.

Docker is one of the main ways the lab supports repeatable services and project work.

## Container Operations

![Docker container list](../assets/images/projects/homelab/docker-containers.png)

## Container Inventory Format

| Container Type | Purpose |
|---|---|
| Automation | Runs scheduled workflows and notifications |
| Monitoring | Supports dashboards, metrics, and visibility |
| Security / GRC | Supports security labs and compliance experiments |
| Infrastructure | Supports reverse proxy, databases, and supporting services |
| Development | Hosts prototypes, tools, and project applications |

## What Good Documentation Captures

For each important container, document:

1. What the container does.
2. Which ports it uses.
3. Where appdata is stored.
4. What credentials or secrets exist outside screenshots.
5. How to restart or rebuild it.
6. What breaks most often.
7. What logs matter.

## Professional Value

Container documentation shows operational maturity. It proves that the environment is not just running by accident; it can be understood, maintained, and rebuilt.
