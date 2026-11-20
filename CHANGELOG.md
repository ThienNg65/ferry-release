# Changelog

Public release notes for Ferry. Download binaries from [Releases](../../releases).

## 1.2.2 (2026-11-20)

### Continuous Integration

* validate Ferry MSIX packages before Store upload

## 1.2.1 (2026-11-19)

### Bug Fixes

* **ui:** fix footer wrapping, connect preload race, middle-click, and glass menu blur
* **ui:** fix footer wrapping, connect preload race, middle-click, and glass menu blur

## 1.2.0 (2026-11-19)

### Features

* **branding:** refresh the Ferry app icon

### Code Refactoring

* **branding:** slim the Ferry mast crossbar

## 1.1.0 (2026-11-19)

### Features

* add Arc UI motion system, responsive container polish, and glass skeleton shimmer

### Bug Fixes

* address security, reliability, and UI edge cases from repo audit
* protect file workflow targets and recover waiting states
* protect file workflow targets and recover waiting states
* revalidate resume stamps and preserve strict file permissions
* review symlink deletions in mirror sync
* show confirmed paths after interrupted sync
* **ui:** preserve horizontal trackpad scrolling in tab strips

## 1.0.1 (2026-11-19)

### Bug Fixes

* isolate Quick Connect visibility filters by SSH port
* preserve fractional bandwidth scheduling credit
* reclaim cancelled bandwidth reservations
* reclaim cancelled bandwidth reservations with FIFO scheduling
* reject premature updater stream closure and test write failures
* reject prematurely closed updater streams and enable write fault injection
* **ui:** persist Glass UI prefs across restarts and refine Glass tab bar
* **ui:** persist Glass UI prefs across restarts and refine Glass tab bar
* **ui:** protect newer UI edits from in-flight settings hydration

### Tests

* cover bandwidth cancellation and cap changes
* cover updater ENOSPC EACCES backpressure and premature close
* guard sustained bandwidth throughput and bounded catch-up

## 1.0.0 (2026-11-18)

### Features

* add Microsoft Store MSIX packaging and CI workflow

### Bug Fixes

* enforce non-zero MSIX major version for Store

### Miscellaneous Chores

* **ci:** remove obsolete Electron-to-Neutralino migration workflow

## 0.32.0 (2026-11-18)

### Features

* **ui:** redesign Ferry icon with minimalist Glassmorphism and dynamic favicon sync
* **ui:** redesign Ferry icon with minimalist Glassmorphism and dynamic favicon sync

### Bug Fixes

* harden SFTP close timeout, drop abort sync, and duplicate drop paths
* stream external drops, pipeline SFTP transfers, and honor local start path

## 0.31.0 (2026-11-18)

### Features

* Fix/log window readiness & new ui
* **ui:** implement Modern Glass UI redesign and enhance dock/pane bars

### Bug Fixes

* **tail:** harden log window readiness, lifecycle, and dock UI

### Documentation

* add session handoff for Phase 2 glassmorphism UI implementation planning
* **design:** add component patterns, feature switch, and discovery toast spec
* **design:** add glassmorphism CSS tokens and Light/Dark recipes
* **design:** add modern typography system spec with Plus Jakarta Sans and JetBrains Mono
* **design:** add root DESIGN.md agent entrypoint and design system index
* **design:** add visual direction and Gałęziowski glassmorphism study
* **design:** resolve final review findings across styling, typography, and component patterns

## 0.30.1 (2026-11-18)

### Bug Fixes

* **release:** harden NSIS process cleanup, packaging, and update manifest verification
* **update-ui:** guard update restarts, surface errors, and harden store state
* **update:** harden auto-update lifecycle, UI, and release verification
* **update:** harden sidecar updater lifecycle, security, and shutdown handoff

## 0.30.0 (2026-11-18)

### Features

* add file visibility filter popover, counts, and pattern helper UI
* add glob visibility filter engine and filename pattern helper
* add per-connection file visibility filter store and persistence
* Feat/file visibility filters
* Feat/terminal predictive echo
* **sites:** click selects a saved site, double-click or Enter connects
* **sites:** harden connection lifecycle, dialogs, and WCAG 2.2 AA UX
* **sites:** redesign site details panel and fix connecting indicators
* **terminal:** add buffer reconciliation and password safety gates to TerminalEchoPredictor
* **terminal:** add core TerminalEchoPredictor state machine
* **terminal:** add predictive local echo setting and toggle
* **terminal:** integrate Mosh-style predictive local echo into terminal stream

### Bug Fixes

* **files:** replace RegExp glob matcher with bounded-cost iterative matcher
* scope bulk delete and range selection to visible filtered entries
* scope Command Palette and pane keyboard actions to visible selected entries
* **terminal:** await prediction flush before fit and re-arm early underline timer
* **terminal:** clear awaitingNewlineConfirm after deferred-wrap command newline
* **terminal:** defer predictions mid-escape, restore erased line suffixes, and preserve SGR attributes
* **terminal:** guard predictive echo callbacks across disable and shell restart
* **terminal:** handle combined backspace chunks, chunked enter, and wrap edge cases in TerminalEchoPredictor
* **terminal:** handle saturated scrollback and retyped erased prefixes in predictive echo
* **terminal:** preserve multibyte UTF-8 stream decoding across predictive echo byte chunks

### Documentation

* document file visibility filters and common glob patterns
* note sites list select-vs-connect convention in PROJECT_MAP
* **terminal:** add predictive local echo design spec and implementation plan

## 0.29.1 (2026-11-17)

### Performance Improvements

* **terminal:** reduce keystroke echo latency 3.47x and double bulk throughput

## 0.29.0 (2026-11-17)

### Features

* refine UI with minimalist HIG design tokens, dock, explorer, and monitor polish

## 0.28.1 (2026-11-16)

### Bug Fixes

* polish right-dock tabs, symlink truncation, breadcrumb a11y, and reconnect banner

## 0.28.0 (2026-11-16)

### Features

* add Ctrl+backtick terminal toggle, dock tooltips, and right-split dock layout
* add session tab context menu with disconnect, reconnect, duplicate, and close others
* display inline symlink targets and broken badge in file rows
* Feat/p3 power user enhancements

### Bug Fixes

* catch tab context menu reconnect rejections and polish review findings
* focus F2 rename input reliably and add Quick Connect reconnect banner

## 0.27.1 (2026-11-16)

### Bug Fixes

* default to full location paths with shorten toggle and clean accent picker layout

## 0.27.0 (2026-11-16)

### Features

* save active Quick Connect session as site and add recent connections dropdown

### Bug Fixes

* add inline port validation and aria-invalid across port fields
* collapse middle breadcrumb segments and wrap long fingerprint errors
* disable preview actions on error, loading, and broken symlinks
* Fix/p2 ux polish and a11y
* improve color picker accessibility, modal close labels, and checkbox shape
* offset toaster above bottom dock and suppress benign ResizeObserver loop errors
* polish hex error state, dropdown close focus, and breadcrumb edge cases

## 0.26.1 (2026-11-15)

### Bug Fixes

* accept scope on bookmarks:create and enable remote bookmarks for quick connect
* auto-refresh destination pane after transfers without losing selection or scroll
* raise muted and dimmed text contrast to WCAG AA in light and dark themes
* render privacy policy and terms markdown as semantic HTML with safe external links
* surface error toast and alert banner on failed mkdir and touch

## 0.26.0 (2026-11-14)

### Features

* Activity dock tab — live progress for every long-running operation
* add log tail overview rail and dock tab controls
* add terminal font and color scheme selection
* add terminal font and color scheme selection
* add zebra striping and directory bolding to file browser rows
* add zebra striping to process monitor rows
* built-in editor improvements, pane resizing, and ui polishing
* calm file list with short dates, row density, and joined title/tab bars
* complete Neutralino cutover and automatic Electron migration
* complete Neutralino cutover and automatic Electron migration
* confirm host key fingerprint on first connect
* connection progress dialog & Happy Eyeballs speed enhancement
* download to active workspace and prevent silent overwrites
* Enhancements of monitoring and logs tailing
* files-first layout with collapsed dock and active pane highlight
* **files:** confirm before deleting folders (and file trash-button/context-menu deletes)
* hide jump host and proxy fields behind progressive disclosure in Add Site dialog
* include P2/P3 UX refinements in release notes
* introduce consistent responsive motion for dock and files
* **logs:** enhance tail log viewer with virtual scrolling, color tracking, and in-log search
* migrate desktop host to Neutralinojs with Node sidecar
* migrate desktop host to Neutralinojs with Node sidecar
* Monitor dock tab — remote CPU/memory/load resource monitor
* **monitor:** storage usage, top-processes table, resizable dock
* native OS window frame, Win11 caption sync, and unclipped toolbars
* native OS window frame, Win11 caption sync, and unclipped toolbars
* polished motion for dock, folders, and tabs
* redesign settings dialog with sidebar tabs
* redesign settings dialog with sidebar tabs
* richer transfer conflict dialog and F5 copy
* **security:** harden main-process against Electron checklist gaps
* **sites:** add bulk select and delete for saved sites
* **tail:** enhance UI/UX, formatting, contrast, and controls for live log tail
* **ui:** enhance UI/UX across session manager, shell chrome, file browser, and bottom dock
* **update:** enhance auto-update with manual checks, progress tracking, and settings
* **ux:** multi-agent UX polish, site export, port validation, and deletion safety
* v0.9.0 — compress-to-zip, bandwidth limit, tab persistence, theme, command palette
* WinSCP-parity gap review — 13 features (v0.13.0)

### Bug Fixes

* abort in-flight connection when the user cancels or closes the tab
* accessibility baseline (labels, contrast, reduced motion)
* add transactional NSIS rollback, custom-dir discovery, and PE icon check
* address code review findings for fast remote browsing
* address final review findings on ui-polish branch
* address PR #45 review findings for updater, release workflow, drop cleanup, and SSH/SFTP smoke parity
* address review findings (host-key bypass, prompt timeout, safe edit saves, conflict rename)
* align monitor history getter with compact CPU samples
* avoid terminal layout squeeze during dock transitions
* **build:** point auto-update feed at real GitHub repo
* close proxy socket and early-cancel leaks, validate terminal send payloads
* confirm single-file delete, cancel rename and path edit on blur
* correct migration process helper template literals
* correctly detect missing public release tags
* detect remote changes and save edits atomically
* **dnd:** resolve dropped-file paths via webUtils for Electron 43
* ensure Neutralino installers are built and recover failed releases
* ensure Neutralino installers are built and recover failed releases
* exclude Node release tests from Vitest
* file list readable at any pane width
* fix Neutralino window maximize, titlebar drag, and bottom dock resize
* fix Neutralino window maximize, titlebar drag, and bottom dock resize
* fix URL pathname matching and cleanup in E2E migration script
* harden crash-safe NSIS rollback, HKLM discovery, and real Electron E2E suite
* harden window bounds, updater timeouts, async dialogs, and store search perf
* harden window bounds, updater timeouts, async dialogs, and store/search perf
* keep migration update server responsive during UI automation
* keep terminal search compatible with optional log highlight keywords
* keyboard focus and selection visibility in file panes
* Live tail log navigation and immediate output (Ticket #2)
* measure maximized dock height from parent bounds
* migrate Ferry auto-update feed to public release repository
* Milestone 2 pilot-hardening — bug fixes, test coverage, Open Edits UI
* plain-language connection errors and persistent error toasts
* preserve rollback backups and gate real Electron migration on isolated Windows runner
* preserve smooth site-tab exit layout
* prevent app crash on unhandled ssh client error events
* prevent false-negative Electron migration release failures
* prevent remote command injection in compress/extract via crafted filenames
* publish latest.yml so auto-update actually works, prep dormant SignPath signing
* recognize Windows 8.3 process paths in migration release gate
* **release:** auto-publish releases with generated changelog notes
* **release:** push git tag before electron-builder publish
* resolve critical and high-priority code review findings
* resolve PR #45 blockers for Neutralino sidecar build, security, updater, drop, and CI smoke
* **security:** allow clipboard-write through the permission handler
* show window on load failure and init updater before manual use
* single instance, no blank-window freeze, safer update install
* single instance, no blank-window freeze, safer update install
* **sites:** batch import into one refetch and avoid duplicate re-creates
* **sites:** stop WinSCP import self-recursion producing duplicated names
* synchronize and verify public Ferry releases
* **tail:** fail fast on permanent errors instead of retrying
* terminal keyboard interaction — focus, copy/paste, right-click
* type check
* **update:** resolve electron-updater CJS interop for autoUpdater export
* use GraphQL branchName when signing public releases

### Performance Improvements

* add in-memory SWR directory caching and optimistic navigation
* add remote exec directory listing parser and command generator
* add watermark flow control so shell floods no longer queue in IPC
* implement exec-first directory listing with SFTP fallback
* **main:** lazy-load ssh2 and archiver off the startup path
* optimize app startup time
* render terminal with WebGL and coalesce output into one IPC message per frame
* **renderer:** virtualize FileList with @tanstack/vue-virtual
* send terminal input and resize fire-and-forget, debounce resize, add ssh keepalive
* smooth live monitoring and log tail interactions
* wire hover prefetching and force refresh for remote directory navigation

### Documentation

* add 0.8.0 changelog entry for the file-op perf pass and injection fix
* add changelog entries for UI polish work
* add changelog entry for 0.11.0 security & performance hardening
* add CI/CD release engineering guide and architecture diagram
* add fast ssh remote browsing implementation plan
* add LICENSE, README, and package release metadata
* add real app screenshots to README
* add UX audit and record new conventions in PROJECT_MAP
* **changelog:** release v0.14.5
* correct PROJECT_MAP gotchas on the WinSCP import self-recursion bug
* correct PROJECT_MAP's permission-handler description, add clipboard gotcha
* document abortable connect and batched terminal output in PROJECT_MAP
* document motion invariants and align template formatting
* explain Release Please bot PR checks and token setup
* finalize v0.14.5 changelog
* finalize v0.14.6 changelog
* finalize v0.14.6 changelog
* finalize v0.14.7 changelog
* finalize v0.14.8 changelog
* finalize v0.14.9 changelog
* update changelog for perf improvements
* update changelog for ssh client error fix
* update PROJECT_MAP for round-6 (Activity/Monitor dock, terminal fix, UI pass)
* write handoff.md for the security & performance hardening session

### Styles

* visual hierarchy pass — separate chrome from content, sharpen selection

### Miscellaneous Chores

* bump version to 0.14.6
* **deps:** upgrade Electron v30 -&gt; v43 and modernize build toolchain
* **main:** release ferry 0.15.0
* **main:** release ferry 0.15.0
* **main:** release ferry 0.15.1
* **main:** release ferry 0.15.1
* **main:** release ferry 0.16.0
* **main:** release ferry 0.16.0
* **main:** release ferry 0.16.1
* **main:** release ferry 0.16.1
* **main:** release ferry 0.17.0
* **main:** release ferry 0.17.0
* **main:** release ferry 0.18.0
* **main:** release ferry 0.18.0
* **main:** release ferry 0.18.1
* **main:** release ferry 0.18.1
* **main:** release ferry 0.18.2
* **main:** release ferry 0.18.2
* **main:** release ferry 0.18.3
* **main:** release ferry 0.18.3
* **main:** release ferry 0.18.4
* **main:** release ferry 0.18.4
* **main:** release ferry 0.19.0
* **main:** release ferry 0.19.1
* **main:** release ferry 0.19.1
* **main:** release ferry 0.19.2
* **main:** release ferry 0.19.2
* **main:** release ferry 0.20.0
* **main:** release ferry 0.20.0
* **main:** release ferry 0.21.0
* **main:** release ferry 0.21.0
* **main:** release ferry 0.22.0
* **main:** release ferry 0.22.0
* **main:** release ferry 0.23.0
* **main:** release ferry 0.23.0
* **main:** release ferry 0.23.1
* **main:** release ferry 0.23.1
* **main:** release ferry 0.24.0
* **main:** release ferry 0.24.0
* **main:** release ferry 0.24.1
* **main:** release ferry 0.24.1
* **main:** release ferry 0.24.2
* **main:** release ferry 0.24.2
* **main:** release ferry 0.25.0
* **main:** release ferry 0.25.0
* **release:** bump to 0.14.11 and guard CD pipeline against existing tags
* **release:** bump version to 0.14.2 [skip ci]
* **release:** bump version to 0.14.3 [skip ci]
* **release:** bump version to 0.14.4 [skip ci]
* **release:** bump version to 0.14.5 [skip ci]
* **release:** bump version to 0.14.6 [skip ci]
* start next development cycle
* start next development cycle
* start next development cycle
* start next development cycle
* start next development cycle
* start next development cycle
* start next development cycle

### Tests

* preserve installer rollback snapshot on restore failure
* stop migrated processes before uninstall verification
* validate Electron migration E2E script in PR CI

### Build System

* stop bundling renderer-only deps into packaged app

### Continuous Integration

* add typecheck/test CI and tag-triggered release workflow
* adopt release-please workflow and sync version to 0.14.15
* auto-tag on main and grant release job write perms
* enhance github actions workflow for atomic releases
* explicitly push lightweight tag
* fix github release 422 error by deferring api calls until after git push
* fix npm exit-handler crash on windows runners
* handle protected branch on main with PR fallback and tag resilience
* harden electron-builder packaging with cache, retry, and prebuilt ico
* run real Electron-to-Neutralino migration E2E for migration PRs

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
