# Public Exposure Watch

## Purpose

A lightweight external exposure check that helps identify whether public-facing services are unexpectedly reachable.

## Problem

Self-hosted labs often grow over time. Subdomains, proxy hosts, ports, DNS records, and exposed services can become hard to track. A simple recurring check helps catch surprises.

## Approach

The workflow checks selected public endpoints and reports whether they appear reachable, blocked, redirected, or unexpected.

## Tools Used

- n8n
- HTTP request nodes
- Discord alerts
- Cloudflare DNS / proxy concepts
- Reverse proxy awareness
- Basic exposure review process

## Screenshots

Save screenshots here later:

```text
docs/assets/images/projects/public-exposure-watch/
```

Example Markdown once screenshots are added:

```md
![Exposure watch alert](../assets/images/projects/public-exposure-watch/discord-alert.png)
```

## Outcome

This project demonstrates basic external attack surface awareness and practical automation.

## Lessons Learned

- DNS, proxy, and firewall rules need periodic review.
- A simple alert can prevent a forgotten exposure.
- Public services should be intentional, documented, and monitored.
