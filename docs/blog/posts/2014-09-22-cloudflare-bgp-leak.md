# Cloudflare BGP Route Leak

## Summary
On September 22, 2014, a BGP route leak by Pakistan Telecom redirected a significant portion of Cloudflare's traffic through Pakistan, causing widespread internet disruptions.

## Timeline
- **October 2, 2014**: Pakistan Telecom announces incorrect routes for Cloudflare's IP ranges.
- **Immediate**: Traffic floods Pakistani networks, leading to blocking.
- **Hours**: Cloudflare mitigates by rerouting traffic.
- **Day**: Issue resolved after Pakistan Telecom withdraws routes.

## Root Cause
Pakistan Telecom leaked BGP routes for Cloudflare's address space (173.245.48.0/20), causing global traffic to be routed through Pakistan. This was likely an attempt to block content, but resulted in collateral damage.

## Impact
- Cloudflare's services slowed or became unavailable worldwide.
- Affected websites using Cloudflare CDN.
- Highlighted BGP vulnerabilities.

## Resolution
- Cloudflare used BGP communities to filter routes.
- Pakistan Telecom corrected the announcement.

## Lessons Learned
- BGP security needs improvement.
- Importance of route filtering and monitoring.
- Global internet routing is fragile.

## Official Postmortem Report
The official postmortem report from Cloudflare can be found [here](https://blog.cloudflare.com/route-leak-incident-on-october-2-2014/).