# Creating Release Candidates

Release Candidates (RCs) are pre-release versions of the next major version of
MyTardis. The first RC, appropriately called RC1, is typically created
on the ###. This is because we have a feature freeze, and new features can only
be merged into the release up to the ###.

Every release will have 1 or more RCs, and there is no limit on the final number.

Usually RC1 has the most number of migrations that should be deployed into
production as soon as possible. Release managers should prioritize getting RC1
deployed. If there are showstopping issues with RC1 (e.g. failed migrations,
critical bugs that prevent logins, etc.), a new RC2 should be created
that contains the **minimal set of changes** needed to deploy the
package. Avoid picking more patches that may slow down the release, especially
those that contain new migrations.

## Guides

- [Creating RC1](#creating-rc1)
- [Creating subsequent RCs](#creating-subsequent-rcs)

### Creating RC1

#### Step 1: Update the ["Admin install" guide]

1. Depending on changes in the upcoming release, you may need to add or remove
   sections.

2. Create a PR against `develop` with the changes and ping a maintainer to merge.
   Make sure you label the PR with `Pick into series-X.Y` label.

3. Follow the ["Pick into stable" guide][cherry-picked] to create a
   PR again the `series-X.Y` branch. Ping a maintainer to merge this too.

["Admin install" guide]: https://github.com/mytardis/mytardis/blob/develop/docs/admin/install.rst

#### Step 2: Update the dependencies license list

#### Step 3: Tag the RC1 version

#### Step 4: Integrating changes from `develop` into `series-X.Y`

Once the `series-X.Y` branch is created, it is the sole source of future
releases for that version. From the 8th, fixes will be either be [cherry-picked] into pull request that targets `series-X.Y` or a pull request specifically
targeting `series-X.Y` (instead of `develop`) should be opened.

Note: Developers are responsible for notifying the release manager that a pull
request is ready to be moved into `series-X.Y`.

---

### Creating subsequent RCs

#### Step 1: Bring changes to the `stable` branches

[Cherry-pick][cherry-picked] pull requests into `stable` branch.
Keep in mind that after RC1 only regressions and security fixes should be
cherry-picked into `stable` branch.

#### Step 2: Tag the RC version


[cherry-picked]: pick-changes-into-stable.md

---

[Return to Guides](../README.md#guides)
