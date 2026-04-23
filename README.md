# semantic-release-workflow

A reusable workflow for running semantic-release with recommended simplicity

<!--status-badges start -->

[![CI Workflow Status][github-actions-ci-badge]][github-actions-ci-link]

<!--status-badges end -->

## Usage

```yaml
jobs:
  verify:
    ...
  release:
    needs:
      - verify
    permissions:
      contents: write
      id-token: write
      issues: write
      pull-requests: write
    uses: form8ion/semantic-release-workflow/.github/workflows/release.yml@v1.0.0
```

## Contributing

<!--contribution-badges start -->

[![PRs Welcome][PRs-badge]][PRs-link]
[![Conventional Commits][commit-convention-badge]][commit-convention-link]
[![semantic-release: angular][semantic-release-badge]][semantic-release-link]
[![Renovate][renovate-badge]][renovate-link]

<!--contribution-badges end -->

### Dependencies

1. Install [mise](https://mise.jdx.dev/getting-started.html)
2. Install project tools

   ```sh
   mise install
   ```

3. Install git hooks

   ```sh
   mise exec -- hk install --mise
   ```

### Verifying

```sh
mise run verify
```

[PRs-link]: http://makeapullrequest.com

[PRs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg

[commit-convention-link]: https://conventionalcommits.org

[commit-convention-badge]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg

[semantic-release-link]: https://github.com/semantic-release/semantic-release

[semantic-release-badge]: https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release

[github-actions-ci-link]: https://github.com/form8ion/semantic-release-workflow/actions/workflows/workflow-release.yml

[github-actions-ci-badge]: https://img.shields.io/github/actions/workflow/status/form8ion/semantic-release-workflow/workflow-release.yml.svg?branch=main&logo=github

[renovate-link]: https://renovatebot.com

[renovate-badge]: https://img.shields.io/badge/renovate-enabled-brightgreen.svg?logo=renovate