---
title: AWS S3 Outage
date: 2017-02-28
authors:
  - Internet Outage Archive
---

# AWS S3 Outage

## Summary
On February 28, 2017, an AWS engineer accidentally deleted servers during a debugging session, causing a widespread outage of the S3 service.

## Timeline
- **February 28, 2017, 9:37 AM PST**: Command executed to remove a small set of servers.
- **9:37 AM**: Due to a typo, the command affected more servers than intended.
- **11:00 AM**: S3 service begins failing.
- **Afternoon**: Partial recovery.
- **March 1**: Full restoration.

## Root Cause
An engineer ran a command to debug billing issues but mistyped the command, removing servers from multiple availability zones instead of one.

## Impact
- S3 unavailable for hours, affecting websites, apps, and data storage.
- Services like Slack, Trello, and Quora impacted.
- Economic losses in millions.

## Resolution
- AWS restored from backups and redundant systems.
- Improved safeguards against such commands.

## Lessons Learned
- Automation and human error prevention.
- Importance of testing in staging environments.
- Better access controls for critical operations.

## Official Postmortem Report
The official postmortem report from AWS can be found [here](https://aws.amazon.com/message/41926/).