# CrowdStrike Global IT Outage

## Summary
On July 19, 2023, a faulty software update from CrowdStrike caused a global outage affecting Windows systems worldwide, disrupting airlines, banks, and hospitals.

## Timeline
- **July 18, 2023**: Update deployed.
- **July 19, 4:09 UTC**: Blue screen errors begin.
- **Morning**: Widespread reports of crashes.
- **Afternoon**: CrowdStrike issues fix.
- **Evening**: Systems recovering.

## Root Cause
A content update for CrowdStrike's Falcon sensor contained a logic error that caused Windows systems to crash with a blue screen.

## Impact
- Affected ~8.5 million Windows devices.
- Disrupted airlines (e.g., Delta), banks, healthcare, and more.
- Economic losses in billions.

## Resolution
- CrowdStrike released a fix to remove the faulty update.
- Manual recovery for some systems.

## Lessons Learned
- Rigorous testing of updates.
- Faster rollback mechanisms.
- Communication during incidents.

## Official Postmortem Report
The official postmortem report from CrowdStrike can be found [here](https://www.crowdstrike.com/blog/falcon-update-for-windows-hosts-technical-details/).