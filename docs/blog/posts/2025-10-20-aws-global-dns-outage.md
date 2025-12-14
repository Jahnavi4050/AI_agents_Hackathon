---
tags:
  - aws
  - outage
  - dns
  - global
---

# AWS Global DNS Outage

## Summary
On October 20, 2025, Amazon Web Services experienced a global DNS resolution outage affecting Route 53 and other AWS services that depend on DNS, causing widespread connectivity issues for applications hosted on AWS.

## Timeline
- **October 20, 2025, 11:00 UTC**: DNS configuration update deployed globally.
- **11:15 UTC**: Initial reports of DNS resolution failures.
- **11:30 UTC**: Widespread impact confirmed across multiple regions.
- **12:00 UTC**: AWS declares incident and begins investigation.
- **13:00 UTC**: Root cause identified as corrupted DNS zone data.
- **14:00 UTC**: Manual recovery procedures initiated.
- **15:30 UTC**: DNS services gradually restored.
- **17:00 UTC**: Full resolution achieved.

## Root Cause
A software bug in AWS's DNS management system caused corruption of DNS zone data during a routine maintenance operation. The corrupted data propagated globally before validation checks could detect the issue.

## Impact
- Global DNS resolution failures for AWS-hosted domains.
- Inaccessibility of websites and applications using Route 53.
- Cascading effects on services dependent on DNS (load balancers, CloudFront, etc.).
- Significant disruption to internet services worldwide.

## Resolution
- Emergency data restoration from backups.
- Implementation of additional validation layers in DNS management.
- Temporary use of secondary DNS systems during recovery.

## Lessons Learned
- Enhanced validation of DNS data before global propagation.
- Improved monitoring of DNS health across all regions.
- Development of faster recovery procedures for DNS infrastructure.
