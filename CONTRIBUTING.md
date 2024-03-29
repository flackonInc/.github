# Guidelines for contributing to this repository

Whenever working on a new change, always branch out and keep publishing your changes from time to time to avoid data loss.
We try to follow linear commit history, so always use rebase instead of merge.

## Branch naming conventions

Naming a branch depednds on the changes you are working on and the type of changes.

1. Following branch naming patterns are recommended:

| Type | Pattern | Example | Notes |
|------|---------|---------|-------|
| New features | `feature/<feature-name>` | `feature/intorduce-xyz-delivery` | Used for changes that can be categorised as new features |
| Bug Fix | `fix/<fix-name>` | `fix/auth-error` | Used for changes that can be categorised as bug fixes |
| Hotfix (urgent bug fixes) | `hotfix/<fix-name>` | `hotfix/docusign-regression` | Used for changes that can be categorised as hotfixs |
| Security Updates/Fixes | `security/<solution-name>` | `security/suppress-server-headers` | Used for changes that can be categorised as security fixes or enhancements |
| Maintenance | `maintenance/<maintenance-name>` | `maintenance/run-integration-tests-in-workflows` | Used for changes that can be categorised as internal maintenance that would help in long term |
| Development | `<author>/<details>` | `devpal/tfa-poc` | Used to manage other tasks that do not fit into above. Often these branches should be converted into one of the above branches (or split into multiple branches of above types) and taken forward |

2. Ensure branch name represents what the branch is about (avoid using names like `fix/bug-fix`, etc)


## PullRequest conventions

While creating the PR we must use the PR’s - templates available in [common repository](https://github.com/flackonInc/.github/tree/main/PULL_REQUEST_TEMPLATE).
Add `?quick_pull=1&template=<TEMPLATE_NAME>` to end of PR url.

* For backend projects, use template [feature-backend.md](https://github.com/flackonInc/.github/blob/main/PULL_REQUEST_TEMPLATE/feature-frontend.md)
* For frontend projects, use the template [feature-frontend.md](https://github.com/flackonInc/.github/blob/main/PULL_REQUEST_TEMPLATE/feature-frontend.md) </br>

Example URL to create PR: https://github.com/flackonInc/docupilot-ui/compare/main...multipage?quick_pull=1&template=feature-frontend.md .</br>


Follow below points while creating the PR's.

* Ensure PR title hints the changes made in head branch appropriately
* Ensure PR desciption explains all the changes made in head branch in detail
* Use `Squash and Merge` option to land PRs once all checks are approved


## Commit message conventions

Follow this article on how to write your commit messages

https://cbea.ms/git-commit/
