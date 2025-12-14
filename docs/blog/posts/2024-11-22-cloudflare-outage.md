---
tags:
  - cloudflare
  - outage
  - dns
  - global
---

# Cloudflare BGP Route Leak (November 22, 2024)

## Summary
On November 22, 2024, Cloudflare experienced a significant BGP route leak incident that disrupted internet connectivity for multiple networks worldwide, affecting routing for approximately 3,000 prefixes.

## Timeline
- **November 22, 2024, 08:45 UTC**: BGP route leak begins from a customer network.
- **09:00 UTC**: Cloudflare detects anomalous routing announcements.
- **09:15 UTC**: Investigation starts, identifying the source as a customer BGP configuration error.
- **09:30 UTC**: Cloudflare begins filtering the leaked routes.
- **10:00 UTC**: Most affected networks recover connectivity.
- **11:00 UTC**: Full resolution achieved after customer corrects their configuration.

## Root Cause
A customer misconfigured their BGP router, causing it to announce Cloudflare's IP prefixes (including 1.1.1.1) to their upstream providers. This created route leaks that disrupted global internet routing for affected networks.

## Impact
- Approximately 3,000 IP prefixes were affected by the route leak.
- Multiple networks worldwide experienced connectivity disruptions.
- Some users reported issues accessing Cloudflare-protected websites.
- The incident lasted about 2 hours from detection to full resolution.

## Resolution
- Cloudflare implemented immediate route filtering to block the leaked announcements.
- Coordinated with the customer to correct their BGP configuration.
- Enhanced BGP monitoring and filtering systems to prevent similar incidents.

## Lessons Learned
- BGP route leaks can have significant global impact despite being caused by a single customer.
- Importance of robust BGP filtering and monitoring systems.
- Need for better coordination between providers and customers during routing incidents.
- Value of automated detection and mitigation systems for BGP anomalies.

