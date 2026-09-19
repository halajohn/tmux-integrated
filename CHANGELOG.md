# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.6.0] - 2026-09-19

### Changed

- Window sizing
- Strip OSC 10/11 color query responses from pane output (reapply)
- Revert "fix: strip OSC 10/11 color query responses from pane output"
- Strip OSC 10/11 color query responses from pane output
- Keep tmux windows alive unless the user closed the tab
- Document tab-name model and showAutomaticRename in README and architecture
- Unit, integration, and real-tmux e2e coverage for tab rename sync
- Opt-in showAutomaticRename tab titles and robust bidirectional rename sync (#40)
- Document node-pty loading strategy and multi-root start-directory pick in ARCHITECTURE
- Reuse already-materialized node-pty shim when the copy fails
- Materialize node-pty shim in global storage and prefer zero-copy loading
- Load node-pty from node_modules.asar on VS Code 1.129+
- Respect selected workspace for new terminals
- Support VS Code 1.129 node-pty packaging
- Sync lockfile with eslint and typescript-eslint devDependencies
- Update release workflow and changelog generation
- Dispose stray default-shell tab spawned by the workbench before activation
- Wait for VS Code restore to settle before adopting tmux windows
- Activate eagerly so the terminal profile provider beats Cursor's panel restore
- Add AGENTS.md with build, release and commit conventions guide
- Update dependencies
- Fix cursor position report issue seen e.g. with gh auth
- Focus new windows and ensure naming of initial window in a session
- Performance improvement - avoid iterating over chunks to do \n -> \r\n replacement use regex
- Document automated release and changelog flow
- Minor doc updates
- Eliminate reconnect races on high-latency links
- Add architecture overview
- Preserve raw escape sequences in tmux %output and forward CSI input atomically (#26)
- Correct git tag sort key in changelog script (refnum → refname)
- Preserve utf-8 boundaries in tmux control mode
- Handle non-ASCII text input literally
- Generate changelog entries from git log instead of placeholder
- Make marketplace publish steps independent with continue-on-error
- Bidirectional tab rename sync + Open VSX publishing
- Use tmux window names as vscode terminal tab names
- Add option to control cwd, independently from terminal.integrated.cwd, default to terminal.integrated.cwd
- Fix automated CHANGELOG.md
- Update to Node 22 for release workflow
- - use xterm-256color to clean up alternate screen - exit vscode tab when last tmux window exits
- - vscode terminal tab closes when tmux window exits - exiting vscode terminal tab kills tmux window - tmux-integrated.autoConnect option. Connect to windows when opening workspace (default: true) - Update node version from 18 to 20 to enable auto publish workflow
- 1.5
- 1.5 fix for '$;' and '\ek' bugs
- 1.4
- Clean resizing
- Fix scrolling
- Phase 1 - extract TmuxGateway, add command flags, batching, and write queuing
- Initial plan for Phase 1 - Architecture & Protocol Hardening
- Initial plan
- Add some plans and arch diagram
- Remove comparison from README.md
- Remove tmux 3.x feature dependencies, update to Version 0.1.4
- Fix changelog format for v0.1.3 and update auto-update script
- Initial plan
- Disable -e env injection for new-window and respawn-pane
- Fix terminal width bug: revert resize-pane approach back to refresh-client -C
- Merge main into branch; resolve conflicts adapting changes to node-pty architecture
- Auto update CHANGELOG.md
- Update changelog for 0.1.2
- Add integrated github/vscode marketplace workflow
- Version 0.1.1
- Fix persistence issue at the cost of stale terminal tabs on exit
- Remove tmux_pty_bridge.py dependency
- Address code review feedback: remove unused field, add named constants
- Architecture review: fix compatibility issues, simplify code, improve correctness
- Initial plan
- Update publisher
- Name windows as tmux:<window number>
- ITerm2-like tab-window model: 1:1 mapping, close kills window, session persists on exit
- Replace TUI jargon and simplify Contributing section in README
- Initial plan
- Rewrite README to be user-focused and platform-agnostic
- Initial plan
- Auto-reattach default profile; fix icon; rename profile to tmux-integrated
- Add icon to extension
- Add remote/SSH support: extensionKind, activationEvents, Linux binary paths
- Close VS Code terminal tab when tmux window/session exits
- Initial plan
- PTY bridge transport, post-input screen reconciliation, UTF-8 fix
- Add tmux control-mode development host and connection fixes
- Correct license from MIT to GPL-3.0-only; document reasoning in README
- Initial plan
- Rename: vscode-tmux → tmux-integrated
- Initial plan
- Implement vscode-tmux VS Code extension with tmux control-mode integration
- Initial plan
- Initial commit

## [0.4.0] - 2026-09-18

### Changed

- Revert "fix: strip OSC 10/11 color query responses from pane output"
- Strip OSC 10/11 color query responses from pane output
- Keep tmux windows alive unless the user closed the tab
- Document tab-name model and showAutomaticRename in README and architecture
- Unit, integration, and real-tmux e2e coverage for tab rename sync
- Opt-in showAutomaticRename tab titles and robust bidirectional rename sync (#40)
- Document node-pty loading strategy and multi-root start-directory pick in ARCHITECTURE
- Reuse already-materialized node-pty shim when the copy fails
- Materialize node-pty shim in global storage and prefer zero-copy loading
- Load node-pty from node_modules.asar on VS Code 1.129+
- Respect selected workspace for new terminals
- Support VS Code 1.129 node-pty packaging

## [0.2.0] - 2026-05-29

### Changed

- Sync lockfile with eslint and typescript-eslint devDependencies
- Update release workflow and changelog generation

## [0.1.16] - 2026-05-29

### Changed

- Dispose stray default-shell tab spawned by the workbench before activation
- Wait for VS Code restore to settle before adopting tmux windows
- Activate eagerly so the terminal profile provider beats Cursor's panel restore

## [0.1.15] - 2026-05-25

### Changed

- Add AGENTS.md with build, release and commit conventions guide
- Update dependencies
- Fix cursor position report issue seen e.g. with gh auth
- Focus new windows and ensure naming of initial window in a session
- Performance improvement - avoid iterating over chunks to do \n -> \r\n replacement use regex

## [0.1.14] - 2026-05-20

### Changed

- Document automated release and changelog flow
- Minor doc updates
- Eliminate reconnect races on high-latency links
- Add architecture overview

## [0.1.13] - 2026-04-25

### Changed

- Preserve raw escape sequences in tmux %output and forward CSI input atomically (#26)

## [0.1.12] - 2026-04-13

### Changed

- Correct git tag sort key in changelog script (refnum → refname)
- Preserve utf-8 boundaries in tmux control mode
- Handle non-ASCII text input literally
- Generate changelog entries from git log instead of placeholder

## [0.1.11] - 2026-03-30

### Changed

- Make marketplace publish steps independent with continue-on-error.

## [0.1.10] - 2026-03-30

### Changed

- Bidirectional tab rename sync + Open VSX publishing.

## [0.1.9] - 2026-03-29

### Added

- Add `tmux-integrated.cwd` setting to control start directory independently of `terminal.integrated.cwd`.

## [0.1.8] - 2026-03-21

### Changed

- Update Node.js to 22 for release workflow.

## [0.1.7] - 2026-03-21

### Added

- Phase 1 — extract TmuxGateway, add command flags, batching, and write queuing.

## [0.1.6] - 2026-03-21

### Added

- vscode terminal tab closes when tmux window exits
- exiting vscode terminal tab kills tmux window
- tmux-integrated.autoConnect option. Connect to windows when opening workspace (default: true)
- Update node version from 18 to 20 to enable auto publish workflow

## [0.1.5] - 2026-03-20

### Fixed

- bash '$;' bug modify send-keys
- zsh echo bug strip escapes

## [0.1.4] - 2026-03-20

### Fixed

- Removed dependency on tmux 3.x+ features allowing tmux 2.x to work
- Fixed scrolling
- Fixed resizing

## [0.1.3] - 2026-03-19

### Added

- GitHub Actions publish workflow for automated VS Code Marketplace and GitHub releases.

## [0.1.2] - 2025-03-18

### Added

- Github / VSCode Marketplace publish workflow

- Fixed persistence issue where tmux sessions were not properly maintained across reconnects.

## [0.1.1] - 2025-03-17

### Fixed

- Fixed persistence issue where tmux sessions were not properly maintained across reconnects.

### Removed

- Removed `tmux_pty_bridge.py` — PTY allocation now uses the native `script` command (macOS/Linux).

## [0.1.0] - 2025-03-16

### Added

- Initial release.
- Seamless tmux control-mode integration for VS Code terminals.
- Persistent terminal sessions that survive window reloads and reconnects.
- `code` command support from within tmux sessions.
- Copilot compatibility in tmux-backed terminals.
