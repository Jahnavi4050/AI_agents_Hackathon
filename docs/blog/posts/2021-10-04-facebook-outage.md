# Facebook Global Outage

## Summary
On October 4, 2021, a BGP configuration change caused Facebook, Instagram, and WhatsApp to go offline for several hours, affecting billions of users.

## Timeline
- **October 4, 2021, 11:39 UTC**: BGP configuration update.
- **Immediate**: Facebook's backbone network disconnected.
- **Hours**: Services down worldwide.
- **15:00 UTC**: Partial restoration.
- **October 5**: Full recovery.

## Root Cause
A maintenance command to assess backbone capacity accidentally removed the BGP routes, disconnecting Facebook's data centers from the internet.

## Impact
- Facebook, Instagram, WhatsApp unavailable for ~6 hours.
- Affected 3.5 billion users.
- Economic impact estimated at $100 million per hour.

## Resolution
- Manual reconfiguration of BGP.
- Restoration of routes.

## Lessons Learned
- Automation of critical network changes.
- Better testing and safeguards.
- Importance of redundant connectivity.

## Official Postmortem Report
The official postmortem report from Facebook can be found [here](https://engineering.fb.com/2021/10/05/networking-traffic/outage-details/).