# coderabbit

Account-wide [CodeRabbit](https://docs.coderabbit.ai/configuration/central-configuration) settings for the
SovereignTechnology repositories. CodeRabbit reads `.coderabbit.yaml` here for every repository that has no file of its
own; a repository's own `.coderabbit.yaml` wins.

- Assertive reviews, drafts included. Automatic approvals are off (they never fired on the open-source plan).
- Fix comments, fix CI and merge-conflict help are on.
- Secret, supply-chain and workflow scanners are on (Semgrep, Gitleaks, TruffleHog, OSV-Scanner, Trivy, Checkov,
  zizmor, actionlint, ShellCheck, Hadolint).
- Dependabot and Renovate PRs are skipped (dependency bumps are checked separately).

Check which file a pull request used with `@coderabbitai configuration` (values from here read "Central YAML").
