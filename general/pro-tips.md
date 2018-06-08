# Pro tips

This is a collection of tips that previous [Release Managers](release-manager.md)
have found to be helpful during their reign. They are _suggestions_, not
requirements. Feel free to contribute your own!

## Use Git aliases

### Add `git cherry-pick` aliases

As merge requests get accepted into `develop`, you're responsible for making sure
they make it into the appropriate `stable` branch. Currently the preferred way
of doing this is via [Git cherry picks] of the merge commit. As you'll be doing
this a lot, it's helpful to have a [Git alias][git-alias] to cut down on typing.

```ini
# ~/.gitconfig
[alias]
  cp  = cherry-pick
  cpm = cherry-pick -m 1
```

```sh
$ git cp <COMMIT SHA>
$ git cpm <MERGE COMMIT SHA>
```

[git-alias]: https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases
[Git cherry picks]: https://git-scm.com/docs/git-cherry-pick

---

[Return to Guides](../README.md#guides)
