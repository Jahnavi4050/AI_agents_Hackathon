# Dyn DNS DDoS Attack

## Summary
On October 21, 2016, a massive DDoS attack targeted Dyn, a major DNS provider, disrupting access to numerous high-profile websites and services.

## Timeline
- **October 21, 2016, 7:00 AM EDT**: First attack wave hits Dyn's infrastructure.
- **11:00 AM**: Second wave amplifies the attack.
- **Afternoon**: Services like Twitter, Netflix, and GitHub become intermittently unavailable.
- **Evening**: Attack subsides after mitigation.

## Root Cause
The attack used the Mirai botnet, consisting of compromised IoT devices. It exploited weak default passwords and sent UDP flood traffic to overwhelm Dyn's DNS servers.

## Impact
- Affected websites: Twitter, Netflix, Reddit, GitHub, Airbnb, etc.
- Millions of users unable to access services.
- Highlighted IoT security risks.

## Resolution
- Dyn implemented traffic scrubbing and rate limiting.
- Botnet operators arrested later.

## Lessons Learned
- DNS infrastructure is a critical vulnerability.
- IoT devices need better security.
- Importance of DDoS protection services.

## Official Postmortem Report
The official postmortem report from Dyn can be found [here](https://dyn.com/blog/dyn-analysis-summary-of-friday-october-21-attack/).