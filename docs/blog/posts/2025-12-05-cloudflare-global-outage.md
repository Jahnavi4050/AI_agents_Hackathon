---
tags:
  - cloudflare
  - outage
  - global
  - configuration
---

# Cloudflare Global Outage

# Cloudflare Global Outage

## Summary
On December 5, 2025, Cloudflare experienced a global outage affecting all services for approximately 2 hours, impacting millions of websites and applications worldwide.

## Timeline
- **December 5, 2025, 14:30 UTC**: Automated configuration deployment begins.
- **14:35 UTC**: Initial reports of service degradation.
- **14:45 UTC**: Full outage confirmed across all Cloudflare services.
- **15:00 UTC**: Emergency rollback initiated.
- **15:30 UTC**: Partial services restored.
- **16:30 UTC**: Full resolution achieved.

## Root Cause
A faulty configuration change in Cloudflare's core routing infrastructure caused a cascading failure that propagated globally. The automated deployment system failed to validate the configuration properly before applying it to production.

## Impact
- Complete outage of Cloudflare's CDN, DNS, and security services.
- Millions of websites inaccessible during the outage window.
- Major impact on e-commerce, streaming services, and online businesses.
- Estimated financial losses in the hundreds of millions globally.

## Resolution
- Immediate rollback to the previous stable configuration.
- Implementation of enhanced validation checks in the deployment pipeline.
- Temporary traffic rerouting through backup systems.

## Lessons Learned
- Strengthen configuration validation before production deployments.
- Implement more robust automated testing for critical infrastructure changes.
- Develop better monitoring and faster rollback capabilities for global systems.

## Official Postmortem Report
The official postmortem report from Cloudflare can be found [here](https://blog.cloudflare.com/5-december-2025-outage/).
