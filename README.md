# VeloDeck Releases

Public release artifacts for VeloDeck live in this repository.

## Required Configuration

- Repository secret: `VELODECK_SOURCE_REPO_TOKEN`
- Optional repository variable: `VELODECK_SOURCE_REPOSITORY` (defaults to `zoubingwu/velodeck`)

`VELODECK_SOURCE_REPO_TOKEN` must be able to read the private source repository so `.github/workflows/release.yml` can check out the tagged commit and build release artifacts.
