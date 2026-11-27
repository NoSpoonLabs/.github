# .github

Shared files of the organisation's repositories: the issue and pull request templates and a reusable workflow.

## Secret scan

Reusable workflow `.github/workflows/secret-scan.yml`: gitleaks and a check for absolute local paths on the new commits
of a pull request or a push. A run without a base commit (manual run, new branch, rewritten history) scans the whole
history. The calling repository chooses the triggers (`pull_request`, `push`, `workflow_dispatch`).
