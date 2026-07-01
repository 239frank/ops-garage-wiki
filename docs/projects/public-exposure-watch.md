# Public Exposure Watch

## Summary

Public Exposure Watch is an n8n workflow branch that checks DNS records, reverse proxy hosts, and Docker-published ports to identify potentially risky public-facing exposure in a home lab environment.

The goal is not to replace a full vulnerability management platform. The goal is to catch obvious changes and reduce the chance of forgetting about something that became publicly reachable.

## Problem

Self-hosted environments can grow quickly. Over time, it becomes easy to lose track of:

- Which DNS records exist
- Which reverse proxy hosts are configured
- Which containers publish ports
- Which services are reachable externally
- Whether a new service changed the exposure baseline

That creates risk because public exposure should be intentional, documented, and reviewed.

## Approach

The workflow builds a simple exposure review process:

1. Pull Cloudflare DNS records.
2. Pull reverse proxy host data.
3. Pull Docker-published port data.
4. Normalize the results.
5. Compare the current run against a stored baseline.
6. Classify findings.
7. Send a Discord report.
8. Write metrics for later dashboarding.

## Screenshots

### Workflow Overview

![n8n workflow overview](../assets/images/projects/n8n-discord/workflow-overview.png)

### Exposure Review Logic

![Public exposure function node](../assets/images/projects/n8n-discord/function-node.png)

### Discord Alert

![Discord public exposure alert](../assets/images/projects/n8n-discord/discord-alert.png)

## What This Demonstrates

- External exposure awareness
- DNS and reverse proxy review
- Docker port review
- Baseline comparison logic
- Operational alerting
- Practical home lab security monitoring
- Translating technical checks into readable reports

## Outcome

The workflow provides recurring visibility into public-facing exposure and makes it easier to notice unexpected changes.

## Lessons Learned

- Public exposure should be intentional.
- Baselines make recurring checks more useful.
- A simple check that runs consistently is better than a perfect check that never gets finished.
- Alert quality matters more than alert quantity.

## Public Safety Note

Screenshots on this page should be sanitized before publishing. Public IPs, private IPs, internal service names, webhook URLs, and media-related services should be blurred or removed.
