<!--
Copyright (c) 2026 The Jaeger Authors.
SPDX-License-Identifier: Apache-2.0
-->

# OpenSSF Best Practices Badge Readiness

This document tracks repository-local evidence for the OpenSSF Best Practices badge application for `github.com/jaegertracing/jaeger-ui`.

GitHub code scanning alert `#10` comes from the Scorecard `CIIBestPracticesID` check. That alert stays open until the repository has an OpenSSF Best Practices badge entry on [bestpractices.dev](https://www.bestpractices.dev/).

## Repository Evidence

- License: [LICENSE](../LICENSE)
- Contributing guide: [CONTRIBUTING.md](../CONTRIBUTING.md)
- Project code of conduct: [CODE_OF_CONDUCT.md](../CODE_OF_CONDUCT.md)
- Security policy: [SECURITY.md](../SECURITY.md)
- Release process: [RELEASE.md](../RELEASE.md)
- Architectural decision records: [docs/adr](./adr)
- Unit tests workflow: [`.github/workflows/unit-tests.yml`](../.github/workflows/unit-tests.yml)
- Lint and build workflow: [`.github/workflows/lint-build.yml`](../.github/workflows/lint-build.yml)
- CodeQL analysis: [`.github/workflows/codeql.yml`](../.github/workflows/codeql.yml)
- Dependency update automation: [`.github/dependabot.yml`](../.github/dependabot.yml)
- Scorecard analysis workflow: [`.github/workflows/scorecard.yml`](../.github/workflows/scorecard.yml)

## Remaining Manual Step

The badge state itself is managed outside this repository. A Jaeger UI maintainer must:

1. Create or claim the project entry for `github.com/jaegertracing/jaeger-ui` on [bestpractices.dev](https://www.bestpractices.dev/).
2. Mark the project as `in progress` or complete the badge criteria there.
3. Update [README.md](../README.md) with the badge URL once the project entry exists.

Completing step 1 changes the Scorecard signal from `0` to a non-zero badge score, which is the condition needed to resolve alert `#10`.
