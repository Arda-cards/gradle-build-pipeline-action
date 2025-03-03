# gradle build

... Grab the badge for the CI build here, see
[Adding a workflow status badge](https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/monitoring-workflows/adding-a-workflow-status-badge) ...
[CHANGELOG.md](CHANGELOG.md)

This action handle the complete build pipeline for a gradle project. It uses the project's `CHANGELOG.md`, the GitHub event and the branch to decide
whether to publish artifacts or not.

## Arguments

See [action.yaml](action.yaml).

## Usage

```yaml
jobs:
  build:
    runs-on: ubuntu-latest
    permissions:
      contents: write
      packages: write
    steps:
      - id: build
        uses: Arda-cards/gradle-build-pipeline-action@v1
        with:
          gpr_user: # user with read access to GitHub Package Repository
          gpr_key: # PT with read access to GitHub Package Repository
          docker_registry: # where to publish docker images; workflow's token need write access to it
          helm_registry: # where to publish helm charts; workflow's token need write access to it
          token: ${{ secrets.GITHUB_TOKEN }}
```

## Permission Required

```yaml
  permissions:
    # to tag
    contents: write
    # to publish artifacts
    packages: write
```
