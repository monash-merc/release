# Security Releases

Security vulnerabilities in MyTardis and its dependencies are to be addressed
with the highest priority.

Security releases are naturally very similar to [patch releases](patch.md), but
on a much shorter timeline. The goal is to make a security release available as
soon as possible, while ensuring that the security issue is properly addressed
and that the fix does not introduce regressions.

Depending on the severity and the attack surface of the vulnerability, an
immediate patch release consisting of just the security fix may be warranted.
For less severe issues, it may be acceptable to include the fix in a future
patch.

## What to include

A security release, even one for the latest monthly release, should _only_
include the changes necessary to resolve the security vulnerabilities. Including
fixes for regressions in a security patch increases the chances of breaking
something.

The only exception to this policy is [release candidates](release-candidates.md).
If the monthly release process is in progress as we're preparing for a security
release, it's acceptable for a new RC to include both security fixes and
regression fixes. Care should be taken to coordinate the publishing of an RC
package with the other security patches so as to not disclose the security
vulnerabilities publicly before we're ready to disclose them.

Be sure NOT to pre-announce which MyTardis versions are affected, since that may
allow malicious users to narrow the search space.


## Process

Please follow the guide for [patch releases](patch.md), but expedite the processes
wherever possible.

---

[Return to Guides](../README.md#guides)
