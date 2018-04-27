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

## Releasing monthly stable version

- [General process overview](general/monthly/process.md)
- [Release manager in monthly release](general/monthly/release-manager.md)
- [Developer in monthly release](general/monthly/developer.md)
- [Quality engineer in monthly release](general/monthly/quality.md)
- [Product manager in monthly release](general/monthly/product-manager.md)

## Releasing patch versions

- [General process overview](general/patch/process.md)
- [Release manager in patch release](general/patch/release-manager.md)
- [Developer in patch release](general/patch/developer.md)
- [Quality engineer in patch release](general/patch/quality.md)

## Security release

- [General process overview](general/security/process.md)
- [Release manager in security release](general/security/release-manager.md)
- [Security engineer in security release](general/security/security-engineer.md)
- [Developer in security release](general/security/developer.md)
- [Quality engineer in security release](general/security/quality.md)

## Guides

- [How to release new minor versions of MyTardis each month](general/monthly.md)
- [How to release patch versions of MyTardis](general/patch.md)
- [How to release security fixes for MyTardis](general/security.md)
- [How to pick specific changes into `stable` branches](general/pick-changes-into-stable.md)
- [How to create release candidates for new monthly versions of MyTardis](general/release-candidates.md)
- [How to perform manual QA testing](general/qa-checklist.md)
- [How to push to multiple remotes at once](general/push-to-multiple-remotes.md)
- [How to remove packages from packages.gitlab.com](general/remove-packages.md)
- [How to push a new omnibus tag version](general/omnibus-tag.md)
- [Required permissions to tag and deploy a release](general/permissions.md)
- [Guidelines for a new major release of MyTardis](general/major.md)
- [Pro tips](general/pro-tips.md)
- [Release template files](.github/issues)
- [How to pick changes for Omnibus MyTardis](general/pick-to-omnibus-gitlab.md)

## Further Reading

- ["Release Manager - The invisible hero"](https://about.gitlab.com/2015/06/25/release-manager-the-invisible-hero/) (2015-06-25)
- ["How we managed 49 monthly releases"](https://about.gitlab.com/2015/12/17/gitlab-release-process/) (2015-12-17)

## License

See [LICENSE](./LICENSE).

# Thanks to GitLab
We wish to acknowledge that the release process adopted by MyTardis is heavily
inspired by Gitlab and that much of this documentation is simply adpated from the
excellent [Gitlab release documentation](https://gitlab.com/gitlab-org/release/docs/).