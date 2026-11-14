# Changelog

Public release notes for Ferry. Download binaries from [Releases](../../releases).

## 0.24.2 (2026-11-14)

### Bug Fixes

* fix Neutralino window maximize, titlebar drag, and bottom dock resize

## 0.24.1 (2026-11-14)

### Bug Fixes

* correct migration process helper template literals
* prevent false-negative Electron migration release failures
* recognize Windows 8.3 process paths in migration release gate

### Tests

* stop migrated processes before uninstall verification

### Continuous Integration

* run real Electron-to-Neutralino migration E2E for migration PRs

## 0.23.1 (2026-11-14)

### Bug Fixes

* ensure Neutralino installers are built and recover failed releases

## 0.22.0 (2026-11-13)

### Features

* introduce consistent responsive motion for dock and files
* polished motion for dock, folders, and tabs

### Bug Fixes

* avoid terminal layout squeeze during dock transitions
* preserve smooth site-tab exit layout

### Documentation

* document motion invariants and align template formatting

## 0.21.0 (2026-11-13)

### Features

* Enhancements of monitoring and logs tailing

### Bug Fixes

* align monitor history getter with compact CPU samples
* keep terminal search compatible with optional log highlight keywords

### Performance Improvements

* smooth live monitoring and log tail interactions

## 0.20.0 (2026-11-12)

### Features

* redesign settings dialog with sidebar tabs

## 0.19.2 (2026-11-12)

### Bug Fixes

* show window on load failure and init updater before manual use
* single instance, no blank-window freeze, safer update install

## 0.19.1 (2026-11-11)

### Documentation

* explain Release Please bot PR checks and token setup

## 0.19.0 (2026-11-11)

### Highlights

- **File browsing:** Compare local and remote folders, navigate back and forward, and toggle hidden files.
- **Transfers:** Pause and retry transfers with clearer progress and speed indicators.
- **Connections:** Import SSH configurations, back up saved sites, and use SSH keys or agents for quick connections.
- **Other improvements:** Expanded file permissions, log keyword highlighting, and better keyboard navigation.

## 0.18.4 (2026-11-11)

### Bug Fixes

* correctly detect missing public release tags

## 0.18.3 (2026-11-11)

### Bug Fixes

* exclude Node release tests from Vitest
* use GraphQL branchName when signing public releases

## v0.18.1 - 2026-11-11

- Moved future update delivery to the public `ferry-release` repository.
- Published a transition installer to both the existing and the new release feeds to preserve updates for current users.
- No user-facing SFTP workflow changes.

## v0.18.0 - 2026-11-11

- Added host key fingerprint confirmation when connecting to a new server.
- Improved file-transfer conflict handling and keyboard shortcuts.
- Improved file browser accessibility, feedback, and reliability.

Future releases are published here with Windows installers and update metadata.
