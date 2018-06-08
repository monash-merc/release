# Monthly Release

MyTardis releases a new minor version (`X.Y`) every month on the 22nd.

The [release manager] should begin the monthly release process *no earlier than* the 7th.
The last day to reliably get your code in the release is the 8th (AEST).

For an idea of the release process please see the [monthly template](https://github.com/mytardis/mytardis/blob/develop/.github/ISSUE_TEMPLATE/monthly_issue.md).

[release manager]: ../../quickstart/release-manager.md

## Process

### 1. Create an issue to track the release

In order to keep track of the various tasks that need to happen each day leading
up to the final release, we create an issue on the [MyTardis issue tracker] and
update it as we progress.

1. Create the issue labelled `monthly_issue[X.Y.0]` (where X.Y is the Major.Minor version)
   and apply the [`monthly_issue`](https://github.com/mytardis/mytardis/issues/new?template=monthly_issue.md) template.

1. You may want to **bookmark** the issue until it's closed at the end of the
   release cycle.

[MyTardis issue tracker]: https://github.com/mytardis/mytardis/issues

### 2. Complete the daily release tasks

Once the release schedule begins, each work day has something that needs to be
done. Perform the tasks and mark them as complete in the issue as you progress.

If you're not sure what to do for any task, [check the guides](../README.md#guides).

## Getting Help

Completing release tasks on time is very important. If you experience problems with any of
release tasks and you don't know who to ask then you should contact someone from the Monash team. The earlier we determine problem or delay in release - the easier it is to fix it.

## Priorities

Keep up with the release schedule. It's better to ship less but on time.
Revert code that delays the release.

---

[Return to Guides](../README.md#guides)
