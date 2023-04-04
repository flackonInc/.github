# Guidelines for contributing to this repository

Whenever working on a new change, always branch out and keep publishing your changes from time to time to avoid data loss.
We try to follow linear commit history, so always use rebase instead of merge.

## Branch naming conventions

Naming a branch depednds on the changes you are working on and the type of changes.

1. Following branch naming patterns are recommended:

| Type | Pattern | Example |
|------|---------|---------|
| New features | `<author-name>/feature/<feature-name>_issue<issue-id>` | `devpal/feature/intorduce-storage_issue122` |
| Bug Fix | `<author-name>/bug/<bug-name>_issue<issue-id>` | `devpal/bug/auth-error_issue123` |
| Hotfix (urgent bug fixes) | `<author-name>/hotfix/<bug-name>_issue<issue-id>` | `devpal/hotfix/docusign-regression_issue124` |
| Maintenance | `<author-name>/maintenance/<maintenance-name>_issue<issue-id>` | `devpal/maintenance/run-integration-tests-in-workflows_issue125` |

2. Ensure branch name represents what the branch is about (avoid using names like `fix/bug-fix`, etc)


## PullRequest conventions

* Ensure PR title hints the changes made in head branch appropriately
* Ensure PR desciption explains all the changes made in head branch in detail
* Ensure all commits are linear (no merge commits)
* Use `Rebase and Merge` option to land PRs once all checks are approved


## Commit message conventions

Follow this article on how to write your commit messages

https://cbea.ms/git-commit/
