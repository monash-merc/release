# Release Manager

The release manager drives the [monthly release] of GitLab as well as any
[patch]/[security] releases for that version.

[monthly release]: ../general/monthly.md
[patch]: ../general/patch.md
[security]: ../general/security.md

## Responsibilities

You as a release manager have a responsibility to protect the work of every
single person involved in the MyTardis Community.

This responsibility sometimes requires making difficult decisions. For example,
you might need to refuse including a feature or a change within a release.
You might need to decide on shipping a feature that is not working as expected
to allow for other features/fixes to be available. You might need to revert
someone's work because it was impacting the release schedule.

The decisions you make can have a cascading effect on all other release tasks,
so make sure that you collect as much data as you can within the time you have,
make an informed decision, and stick with it.

At all times, keep in mind that protecting MyTardis users and the stability of
MyTardis deployments are more important than accepting a change in a release to please
someone from your or another team.

When you start as a release manager, some of your responsibilities are:

* Creating preparation PRs for stable branches containing requested fixes
* Escalating to responsible parties in case a release task is slowed down or
  blocked by their area of responsibility
* Performing/coordinating QA tasks and making sure that everyone involved finishes their task

The monthly releases are a community-wide effort, and should not
fall entirely on the release manager's shoulders. More about that in the sections
that follow.

## Getting Started

It is the ### of the month and you need to get started with preparations for your
tasks.

Start with [Onboarding](../general/onboarding.md). Don't worry, we'll wait for you here.

### Release meta issue

Create a [new issue in the release/task project](https://github.com/mytardis/release/issues/new)
and select `monthly_release_issue` template.

The title of the issue should be `Release X.Y.0`, where `X.Y` is the version you
are working on.

This meta issue will serve as the main place where everyone can find issues
related to the release you will be working on.

Make sure that you are assigned to this issue.

Every time you create a new issue for one of the upcoming tasks, you should
link it to this meta issue.

### Training

Now is a good time to talk with the previous Release Managers. They should
be able to answer any question you have. If they don't know the answer, they should
direct you to a person who might know. Feel free to go as far as necessary to
get your answer. Do remember to document when you find that answer!

### Release Candidates

Release Candidate (RC) is a point in time snapshot of what will become a release.
Any RC that gets created can be considered for final release.

The most important and time-critical RC is the initial one created after feature freeze.

After the first RC gets deployed to GitLab.com, you should consider creating
a RC every day until the final release.

Why we hear you ask? More details can be found in [release candidates][release-candidates]
document.

### Deployment on Monash Test Stack

With the help of the Monash Instrument Integration team, the release manager is also
responsible for helping to deploy the latest version to the Store.Monash test stack. During the merge
window, the release manager needs to pay particular attention to migrations that
may block the deploy. For example, migrations that take a long time (e.g.,
adding a column with a default value to the issues table) should be reviewed
carefully.

### QA task

Quality assurance (QA) is how we reduce the possibility of shipping a broken feature.
Your responsibility is to create an issue that contains the changes included
in the release and mentioning the responsible parties.

Any task can be delegated to any member of the team who can perform it. When
delegating a task, be sure to mention a person directly rather than asking
something indirect like "Can someone help me do QA?".

If someone is unavailable to perform a task, ask someone else. Escalate if you are
not getting responses.

Find out more about QA task in a separate [qa documentation][qa].

### Patch Release

That was a lot of work, right? Well don't worry, you get to do it a few more times!

The bug reports will start to come in as users update to the latest version.
Your colleagues too will want to improve some things as well now that the
version is live. That's where patch releases come in.

The amount and scheduling of [patch releases][patch] is entirely at your discretion as
the release manager.

Exception is reserved for [security releases](../general/security.md), which should be
addressed immediately. However, that is a [bit of a different story](../general/security.md).

If a bug affects a large number of users and/or a critical piece of
functionality, it's fine to release a patch with only one fix. Sometimes a patch
will include five or more minor fixes. You should use your
best judgment to determine when a patch release is warranted. If you are not sure,
you can always ask for help on deciding at #releases. We strive to
continue releasing patches until all (or most) known regressions for that release are
addressed.

To help you understand what is expected from you when doing patch releases,
check out [Patch release documentation][patch]

[release-candidates]: ../general/release-candidates.md
[qa]: ../general/qa-checklist.md
[patch]: ../general/patch.md

---

[Return to Quick Start](../README.md#quick-start)
