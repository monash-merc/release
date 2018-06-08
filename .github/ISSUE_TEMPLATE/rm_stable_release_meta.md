## General Process for Release Managers

This issue serves as one place to find all information needed for the
release on the 22nd. This issue should be used to link related issues
associated with the release such as individual Release Candidate issues
and exception requests.

### High-level tasks

- [ ] Create the `Pick into X.Y` group label if it doesn't exist: [https://github.com/mytardis/mytardis/labels](https://github.com/mytardis/mytardis/labels).
  * Note: Replace `X.Y` with the version you are working on.
- [ ] Create new issues in the [MyTardis issue tracker] for the release, following the [Monthly], [Patch] or [Security] guides.
- [ ] Create a `series-X.Y` branch for the new release.
- [ ] Follow the initial steps for [creating the first RC](https://gitlab.com/gitlab-org/release/docs/blob/master/general/release-candidates.md#creating-rc1):
  - [ ] Create a PR on `develop` updating the "Admin install" guide.
  - [ ] [Pick][cherry-pick] the changes to the "Admin install" into a PR against
  the `series-X.Y` branch.
  - [ ] Ensure the above PRs are merged prior to creating the RCs.


[MyTardis issue tracker]: https://github.com/mytardis/mytardis/issues
[Monthly]: https://github.com/mytardis/release/blob/develop/general/monthly.md
[Patch]: https://github.com/mytardis/release/blob/develop/general/patch.md
[Security]: https://github.com/mytardis/release/blob/develop/general/security.md
[Pick]: https://github.com/mytardis/release/blob/develop/general/pick-changes-into-stable.md

## Individual Release Candidate preparation issues

Issues relating to the preparation of a Release Candidate should be created
separately and linked in this issue.
