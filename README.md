__Note__: this will be moved to the MyTardis organisation once the documentation
is a little more formalised.

# MyTardis Release Process

This repository contains instructions for releasing new versions of
MyTardis.

The goal is to provide clear instructions and procedures for our entire release
process. This repository includes documentation which should help perform the role of [Release
Manager](quickstart/release-manager.md) as well as documentation that should help
other stakeholders in the release process.

The topics are divided per each type of release. Each type of release has a
general process overview and specific documentation for different stakeholders.

The process listed below contains very specific deadlines. If something can be done
before the deadline, there is no reason to wait. In special cases when there is
urgency (critical security release, lack of resources) it is *required* to be
more flexible (even inventive) in order to deliver tasks on time. Flexibility
does not apply when going over the deadline, so do not be late!

## Quick Start

- [Starting as Release manager](quickstart/release-manager.md)

## Guides

- [How to release new minor versions of MyTardis each month](general/monthly.md)
- [How to release patch versions of MyTardis](general/patch.md)
- [How to release security fixes for MyTardis](general/security.md)
- [How to pick specific changes into `stable` branches](general/pick-changes-into-stable.md)
- [How to create release candidates for new monthly versions of MyTardis](general/release-candidates.md)
- [How to perform manual QA testing](general/qa-checklist.md)
- [Guidelines for a new major release of MyTardis](general/major.md)
- [Pro tips](general/pro-tips.md)

## Further Reading

- ["Release Manager - The invisible hero"](https://about.gitlab.com/2015/06/25/release-manager-the-invisible-hero/) (2015-06-25)
- ["How we managed 49 monthly releases"](https://about.gitlab.com/2015/12/17/gitlab-release-process/) (2015-12-17)

## License

See [LICENSE](./LICENSE).

# Thanks to GitLab
We wish to acknowledge that the release process adopted by MyTardis is heavily
inspired by Gitlab and that much of this documentation is simply adpated from the
excellent [Gitlab release documentation](https://gitlab.com/gitlab-org/release/docs/).