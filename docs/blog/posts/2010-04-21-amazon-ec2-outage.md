# Amazon EC2 Outage

## Summary
On April 21, 2010, a network reconfiguration error in Amazon's EC2 service caused a massive outage affecting numerous websites and services hosted on the platform.

## Timeline
- **April 21, 2010, 10:30 AM PDT**: Network maintenance begins.
- **11:00 AM**: Reconfiguration error occurs, isolating instances.
- **Afternoon**: Issues escalate, affecting multiple availability zones.
- **Evening**: Partial restoration begins.
- **April 22**: Full recovery.

## Root Cause
During routine network maintenance, a command to remove a small number of servers from a network configuration inadvertently removed all servers, causing a cascade of failures in the EBS (Elastic Block Store) and EC2 services.

## Impact
- Affected services included Reddit, Quora, Foursquare, and others.
- Millions of users experienced downtime.
- Financial losses estimated in millions.

## Resolution
- Amazon engineers manually reconnected servers.
- Improved monitoring and automation implemented.

## Lessons Learned
- Importance of testing maintenance procedures.
- Need for better isolation between availability zones.
- Enhanced communication during incidents.

## Official Postmortem Report
The official postmortem report from AWS can be found [here](https://aws.amazon.com/message/65648/).