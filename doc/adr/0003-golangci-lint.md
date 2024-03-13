# 3. golangci-lint

Date: 2024-03-13

## Status

Accepted

## References

- [golangci-lint](https://golangci-lint.run/)
- [A guide to using act with GitHub Actions](https://dev.to/logrocket/a-guide-to-using-act-with-github-actions-2n3m)


## Usage

How to use this pipeline in your project.

```yaml
name: Go Linting
on:
  workflow_dispatch:
  push:
  release:
    types: [created]
jobs:

  go-lint:
    uses: estenrye/.github/.github/workflows/golangci-lint.yaml@v0.1.15
    secrets:
      token: ${{ secrets.GITHUB_TOKEN }}
    # with:
    #   Override centrally managed .golangci.yaml configuration with a repository specific configuration.
    #   golangci_lint_config_path: .golangci.yaml
```

How to launch this pipeline locally in your project.

```bash
brew bundle
gh auth login
act push --container-architecture=linux/amd64 -s GITHUB_TOKEN="$(gh auth token)"
```
