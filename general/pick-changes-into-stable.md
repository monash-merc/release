## Pick specific changes into the `stable` branches

The latest RCs, and all patch releases are made up of one or more merge requests
that have been merged into the `develop` branch of MyTardis, and which
then need to be [cherry-picked] into the respective `stable` branches.

We merge into `develop` first instead of merging in a stable branch first because
`develop` moves faster than stable branches. Getting there first prevents the most
merge conflicts by more quickly having all developers fetch the changed code.

We cherry pick the single **merge commit** that results from accepting a merge
request and which may have been made up of more than one commit. This means we
only have to perform one pick per pull request and reduces the chances of
missing commits.

1. Make sure you have the latest changes in `develop`:

    ```sh
    git checkout develop
    git fetch upstream
    git merge upstream/develop
    ```

1. Check out the `stable` branch:

    ```sh
    # NOTE: This command is an example! Update it to reflect new version numbers.
    git checkout series-3.8
    ```

1. Checkout a new branch from the stable branch:

    ```sh
    git checkout -b patch-for-series-3.8
    ```

1. Cherry-pick the **merge commit** from `develop`. You should almost always be
   picking merge commits (i.e., a merge of a pull rquest) because there may be a
   series of commits in a pull request that must go together.

    ```sh
    # NOTE: This command is an example! Update it to reflect the actual SHA.
    git cherry-pick [merge commit sha] -m 1
    ```

    To learn why it's safe to use `-m 1`, please read [this StackOverflow
    answer](https://stackoverflow.com/a/12628579/223897).

1. Push the updated branch to your `origin` and create a pull request against the
   `stable` branch you are targeting e.g. `series-3.8`:

    ```sh
    # NOTE: This command is an example! Update it to reflect new version numbers.
    git push origin patch-for-series-3.8
    ```

1. Ping one of the other devs to review and merge your PR.

---

[Return to Guides](../README.md#guides)
