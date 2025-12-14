---
tags:
  - cloudflare
  - outage
  - configuration
  - global
---

# Cloudflare Global Outage

## Summary
On July 17, 2020, a configuration change in Cloudflare's edge servers caused a global outage affecting millions of websites.

## Timeline
- **July 17, 2020, 13:42 UTC**: Configuration update deployed.
- **Immediate**: Edge servers begin crashing.
- **Minutes**: Widespread outages reported.
- **14:32 UTC**: Rollback begins.
- **15:00 UTC**: Services restored.

## Root Cause
A configuration change to optimize CPU usage inadvertently caused a high rate of crashes in edge servers due to a bug in the update process.

## Impact
- Cloudflare-protected websites down for ~30 minutes.
- Affected services like Discord, Shopify, and others.
- Global internet disruption.

## Resolution
- Rapid rollback of the configuration.
- Investigation and fix of the bug.

## Lessons Learned
- Thorough testing of configuration changes.
- Monitoring for rapid deployment issues.
- Importance of quick rollback capabilities.

## Official Postmortem Report
The official postmortem report from Cloudflare can be found [here](https://blog.cloudflare.com/cloudflare-outage-on-july-17-2020/).