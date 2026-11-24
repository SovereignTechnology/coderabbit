# coderabbit

Account-wide [CodeRabbit](https://docs.coderabbit.ai/configuration/central-configuration) settings for the
SovereignTechnology repositories. CodeRabbit reads `.coderabbit.yaml` here for every repository that has no file of its
own; a repository's own `.coderabbit.yaml` wins.

- Assertive reviews, drafts included. It requests changes for blocking findings and approves once they are
  resolved, at minimal merge and security risk only (the policy rbitcoin-org/rbitcoin uses).
- Learnings are shared across all repositories; `CLAUDE.md`, `AGENTS.md` and `CONTRIBUTING.md` are read as guidelines.
- New issues are enriched with related code and a suggested approach.
- Fix comments, fix CI and merge-conflict help are on.
- Secret, supply-chain and workflow scanners are on (Semgrep, Gitleaks, TruffleHog, OSV-Scanner, Trivy, Checkov,
  zizmor, actionlint, ShellCheck, Hadolint).
- Dependabot and Renovate PRs are skipped (dependency bumps are checked separately).

Check which file a pull request used with `@coderabbitai configuration` (values from here read "Central YAML").
