# BaseDeck Releases

BaseDeck is a native database browser with a read-only MCP integration.

This repository is the public release repository for BaseDeck. It exists to host downloadable builds, release metadata.

## Download

If you are looking for the app, start here:

- https://github.com/zoubingwu/basedeck-releases/releases

Current public releases are macOS-first.

## What BaseDeck Is

BaseDeck is built for working with databases locally in a desktop app:

- Browse schemas, tables, and views
- Inspect fields, keys and bounded pages of data
- Export a preview page and copy cell values
- Share selected connections with external MCP clients

Version 0.34.0 replaces the desktop runtime with Go and MyGo native UI. It removes the built-in AI chat and SQL workbench. The website and licensing services remain unchanged.

## Upgrading existing installations

- Existing apps use the stable Electrobun feeds to download a full native replacement.
- macOS keeps `BaseDeck.app` and its bundle identity. Windows retains a small launcher for existing shortcuts.
- Existing connections, encrypted credentials, device IDs and license activations are preserved. The first configuration write creates a `config.json.pre-native-<timestamp>` backup in `~/.basedeck`.
- macOS may ask permission for the native app to access the original Keychain item once.
- Saved SQL and agent history remain on disk but are not part of the new workspace.
- Later updates use signed native archives and retain the existing paid-update eligibility rules.

For rollback, quit the app, reinstall the previous release and restore the configuration backup if needed. Do not run both runtimes against the same configuration concurrently.

Release builds are first uploaded as drafts. Publishing a verified draft is a separate action; do not point old clients at an incomplete release.

BaseDeck currently supports MySQL, TiDB, PostgreSQL, SQLite, BigQuery, and Cloudflare D1.

## About This Repository

- This is not the main source repository
- The application itself is developed in a private repository
- This public repository is only used for publishing release artifacts and download history
