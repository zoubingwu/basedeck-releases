# BaseDeck Releases

Public release artifacts for BaseDeck live in this repository.

## Required Configuration

- Repository secret: `BASEDECK_SOURCE_REPO_TOKEN`
- Optional repository variable: `BASEDECK_SOURCE_REPOSITORY` (defaults to `zoubingwu/basedeck`)

`BASEDECK_SOURCE_REPO_TOKEN` must be able to read the private source repository so `.github/workflows/release.yml` can check out the tagged commit and build release artifacts.
