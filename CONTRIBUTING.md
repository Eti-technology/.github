# Contributing

Default contributing guide for every Eti-technology repository that doesn't ship its own.
Repo-specific rules (in a repo's own `CONTRIBUTING.md`, `CLAUDE.md` or `README.md`) take precedence.

## Commit Conventions

* Follow [Conventional Commits](https://www.conventionalcommits.org/): `type(scope): subject` with an optional body.
* **Types (only these 5):** `feat`, `fix`, `refactor`, `chore`, `revert`.
* **Scope is the Jira ticket ID, lowercase:** `fix(et-123): subject`.
  * One ticket per scope. Extra tickets go in the subject as full keys — `fix(et-1441): rotate key ET-1446` — so `jira-transition` moves them too (it matches keys case-insensitively).
  * No ticket (Dependabot's `chore(deps)`, a one-off CI tweak): omit the scope or use a lowercase noun.
* **Subject:** lowercase start, no trailing period, max 100 characters.
* **NEVER** add `Co-Authored-By` (or any similar attribution trailer). This applies to all commits, including those made by AI assistants.

## Pull Requests

* Branch from `main` and open a PR — never push directly to `main`.
* PR title follows the same format as a commit. In squash-merged repos it becomes the commit on `main`.
* Name branches after the ticket: `fix/et-123-short-description`.
