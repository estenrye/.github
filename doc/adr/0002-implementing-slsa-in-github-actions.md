# 2. Implementing SLSA in GitHub Actions

Date: 2023-08-15

## Status

Accepted

## Context

This repository provides reusable pipelines for my opensource project work.
I want to use best practices when building my artifacts so that users have
confidence in the binaries I produce with my build pipelines.

### References

- [Achieving SLSA 3 Compliance with GitHub Actions and Sigstore for Go modules](https://github.blog/2022-04-07-slsa-3-compliance-with-github-actions/), Jose Palafox, 2022-04-07
- [GitHub Actions: reusable workflows is generally available](https://github.blog/2021-11-29-github-actions-reusable-workflows-is-generally-available/), Jennifer Schelkopf, 2021-11-29
- [Using starter workflows](https://docs.github.com/en/actions/using-workflows/using-starter-workflows#using-starter-workflows)
- [General Availability of SLSA 3 Go native builder for GitHub Actions](https://slsa.dev/blog/2022/06/slsa-github-workflows), Laurent Simon, Asra Ali, Ian Lewis, Mark Lodato, Jose Palafox, Joshua Lock, 2022-06-20
- [Generation of SLSA3+ provenance for Go projects](https://pkg.go.dev/github.com/slsa-framework/slsa-github-generator/internal/builders/go#section-readme)

## Decision

The change that we're proposing or have agreed to implement.

## Consequences

What becomes easier or more difficult to do and any risks introduced by the change that will need to be mitigated.
