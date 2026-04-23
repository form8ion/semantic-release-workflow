# semantic-release-workflow
A reusable workflow for running semantic-release with recommended simplicity

## Contributing

<!--contribution-badges start -->

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

[renovate-link]: https://renovatebot.com

[renovate-badge]: https://img.shields.io/badge/renovate-enabled-brightgreen.svg?logo=renovatebot