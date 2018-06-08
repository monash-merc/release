# Major release

MyTardis occasionally releases a new major version (e.g. from 3.X to 4.X).

A major release allows us to make breaking changes, for instance removing or
changing (deprecating) existing APIs and functionalities.

## Handling deprecations

Deprecations should be announced and if necessary replaced one or more releases
in advance of the major release.

For instance, when going from API v1 to v2, v2 will have to be active for at
least a single release before deprecating v1. In practice, it's very unfriendly
to deprecate an API over a single month and a longer time period might be chosen
(such as one major release for a new API version, or a span of a number of
releases).

## New functionalities and APIs

New functionalities and APIs can freely be added at any time and should not be
ported back.

## Frequency

At this time, there is no particular frequency to the occurrence of major
releases.

## Creating awareness

People need to be aware of changes and deprecations. For each major or breaking
change, consider:

- updating all documentation
- making customers aware in blog and release posts
- training the service engineers in the change, but also in how to help
  customers transition
- optionally: reaching out to customers and/or external applications


