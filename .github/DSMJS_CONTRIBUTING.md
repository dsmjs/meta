# Cross-Organization Contributing Details

Below are some details about some of the expectations and practices that we attempt
to stay consistent with across the projects throughout the organization.

## Development Environment Consistency

We have taken several steps to enable a consistent environment. We hope this makes
it easier to get from initial clone of our repositories and also makes getting
troubleshooting help from us more successful.

In addition, more details captured in version control makes it more reliable to
explore history, like using [`git bisect`](https://git-scm.com/docs/git-bisect)
to identify when a problem was introduced.

### nvm

* nvmrc

installation
* nvm
* avn

### package-lock.json

The decision around whether or not to use a lockfile has some big tradeoffs, so
which to use is not a simple choice. `npm` provides the ability to define dependencies
using [semver](https://semver.org/) ranges so that in-range updates can applied
without updating the range definition.

Choosing to use a lockfile prevents the in-range updates from being applied without
updating the lockfile. However, this is good from the perspective that all developers
have the exact same dependencies installed and

### `save-exact`

* packages can use ranges
* apps should use exact

## Dependency Management

* greenkeeper
* greenkeeper-keeper
* in theory, the lockfile is updated often enough

## Publishing New Versions

* semantic-release
* commit convention
* commitlint
* commitizen

## Coding Standards

* consistency is more important than any particular rules
* rules are decided by maintainers but we are open to feedback
* we prefer feedback from the computer rather than adding distraction to PR reviews
