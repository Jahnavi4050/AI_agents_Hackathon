# The Morris Worm Incident

## Summary
On November 2, 1988, Robert Tappan Morris released the first internet worm, which spread rapidly across the early internet, infecting thousands of computers and causing significant disruption.

## Timeline
- **November 2, 1988**: The worm is released from a computer at MIT.
- **Hours later**: The worm begins spreading exponentially, infecting VAX and Sun machines running BSD Unix.
- **November 3, 1988**: The worm is contained after Eugene Spafford analyzes and shares the code.

## Root Cause
The worm exploited three vulnerabilities:
1. A buffer overflow in fingerd.
2. A debug mode backdoor in sendmail.
3. Weak passwords allowing rsh/rexec access.

A programming error caused the worm to reinfect machines, leading to resource exhaustion.

## Impact
- Infected approximately 6,000 out of 60,000 internet-connected computers (10% of the internet at the time).
- Caused system slowdowns, crashes, and unavailability.
- Estimated cost: $10-100 million in cleanup and lost productivity.

## Resolution
- Systems were patched and cleaned manually.
- The internet community developed better security practices.

## Lessons Learned
- Highlighted the need for internet security standards.
- Led to the creation of CERT (Computer Emergency Response Team).
- Emphasized responsible disclosure and ethical hacking.
