# Security Releases general information

At GitLab, we have two types of security releases: **non-critical** and **critical**.

## Non-critical security releases

Every 28th of the month, we are releasing patch versions of GitLab containing
non-critical security fixes.
This date has been chosen as it gives enough time to release regular patch
releases after standard release on the 22nd of the month. This date also allows
us to create and test fixes internally as the next development cycle (starting on
the 8th) starts.

### General process overview

Release manager follows the process defined for
[non-critical security release](release-manager.md#non-critical).
Release manager also makes sure that all the deadlines (described below) are
respected. Any delay needs to be escalated to Director of Backend and Security.

Developers need to follow the the process defined for
[non-critical security release](developer.md#non-critical).

Quality engineers need to follow the process defined for [non-critical security
release](quality.md#non-critical).

Security engineers need to follow the process defined for [non-critical security
release](security.md#non-critical).

### Release deadlines

Anything that can be carried out before the deadline, should be done.
Anything that is not done by the deadline requires immediate escalation to
people responsible of security release process.
Dates in this section can be considered as non-negotiable deadlines.

Regular security release contains security fixes that are ready for merge
**by 23:59 Pacific time on the 23rd** of the month. Both the fixes for the
current release and *all* of the backports need to be ready for merge and have
green tests.

If fixes and backports are not ready by that date, they will
have to go into the next security release.
**Exceptions can't be made** because verifying and creating security releases
are time consuming and any delay puts regular releases in danger.

Current release and all backports need to be tagged and packages created
**by 23:59 PT on the 24th**. This is also the deadline for creating the initial
blog post.

Once the packages are ready and up until **23:59 Pacific time on the 26th** of the
month, Quality Assurance tasks need to be carried out on *all* created releases to
verify that the fixes are indeed working as intended. During this period,
the tests should be executed on separate infrastructure created to carry out these tests.
Staging/canary/production are should remain open for regular releases.

Deploy to staging and canary environments should be carried out by **23:59 Pacific time
on the 27th** the latest.
Deploy to production has to be completed by **07:00 Pacific time on the 28th**.
Package promotion has to be coordinated with the blog post release. 1 hour before
the scheduled blog post announcement, package promotion should be done. This is
required because package promotion takes time to propagate.

Blog post, tweet and the email announcement should be complete by **10:00 Pacific time on the 28th**.
