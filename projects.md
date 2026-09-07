---
---

# Projects

As a passionate contributor to the open-source ecosystem, I dedicate my spare time to developing tools, extensions, and mobile applications that solve real-world problems.

- [TypeScript (JavaScript)](#typescript-javascript)
- [Dev Container](#dev-container)
- [GitHub Actions](#github-actions)
- [Linux](#linux)
- [Gnome](#gnome)
- [Firefox](#firefox)
- [Node.js](#nodejs)
- [Sailfish OS (Jolla)](#sailfish-os-jolla)
- [Android](#android)
- [SaaS Services](#saas-services)
- [Design](#design)
- [Miscellaneous](#miscellaneous)

## TypeScript (JavaScript)

### Helpers4
*TypeScript-first, enterprise-grade utility library — zero dependencies, 100% test coverage*

[helpers4](https://helpers4.dev/) is a JavaScript/TypeScript utility library designed to eliminate the need to rewrite the same helpers across every project. Built around a per-category package architecture for optimal tree-shaking, it covers the practical, real-world helpers that every professional JS/TS project ends up needing. v2 shipped in May 2026 after two years of development and 22 pre-releases, and has kept growing since — from 12 packages at launch to 19 today.

**20+ focused packages, plus 2 all-in-one bundles:**
- `helpers4` / `@helpers4/all` - the complete collection, as a real dependency or a documentation-only meta-package
- `@helpers4/array` - chunking, comparison, manipulation, async iteration
- `@helpers4/ci` - CI/CD workflow status formatting for PR comments and pipeline reports
- `@helpers4/color` - color conversion and validation
- `@helpers4/commit` - Conventional Commits parsing, validation, analysis
- `@helpers4/date` - comparison and validation utilities
- `@helpers4/function` - composition and utility wrappers
- `@helpers4/guard` - runtime type guards
- `@helpers4/id` - unique identifier generation (UUID v7, etc.)
- `@helpers4/license` - license validation and management
- `@helpers4/map` / `@helpers4/set` - native `Map`/`Set` manipulation
- `@helpers4/markdown` - Markdown formatting and escaping
- `@helpers4/node` - Node.js runtime utilities (Buffer, etc.)
- `@helpers4/number` - numeric operations and formatting
- `@helpers4/object` - deep merge, pick, omit, deep comparison
- `@helpers4/observable` - RxJS Observable helpers and operators
- `@helpers4/promise` - retry, delay, concurrency limiting, mutex/semaphore
- `@helpers4/string` - capitalize, slugify, camelCase, kebabCase, truncate…
- `@helpers4/type` - compile-time TypeScript utility types
- `@helpers4/url` - parsing, manipulation, normalization
- `@helpers4/version` - semantic version parsing, comparison, and validation

[Source code](https://github.com/helpers4/typescript) | [Documentation](https://helpers4.dev/typescript) | [v2 release post](https://helpers4.dev/blog/2026-05-23-helpers4-typescript-v2/)

## Dev Container

[helpers4/devcontainer](https://helpers4.dev/devcontainer/) is a collection of plug-and-play DevContainer features for consistent, reproducible development environments. Features are published to `ghcr.io/helpers4/devcontainer` and follow the DevContainer Features specification. What started as 9 features has grown to **20**:

**AI agent tooling**
- `claude-dev` - Claude Code extension + CLI, credentials persisted across rebuilds
- `cline-dev` - Cline AI coding agent extension + CLI
- `copilot-dev` - Copilot Chat, `gh copilot`, shared commit/PR/review instructions
- `mistral-dev` - Mistral Vibe IDE extension, credentials persisted across rebuilds
- `peon-ping` - game-character voice notifications when your AI agent needs you

**Core dev environments**
- `essential-dev` - Git visualization, editor enhancements, Markdown
- `typescript-dev` - TypeScript/JS dev with import management
- `angular-dev` - Angular dev, port 4200 forwarding
- `vite-plus` - full Vite+ toolchain (Vite, Vitest, Oxlint, Oxfmt, Rolldown, tsdown)
- `playwright-dev` - headless browsers + cached binaries + Playwright Test extension
- `github-dev` - GitHub CLI and VS Code platform extensions

**Infra & workflow**
- `package-auto-install` - auto-detect and install on container creation
- `pnpm-store` - shared pnpm content-addressable store across rebuilds
- `nub` - runs TS/JS files and local CLIs on the container's existing Node, no new runtime
- `git-absorb` - automatic absorption of staged changes into logical commits
- `shell-history-per-project` - persistent shell history isolation per project
- `dotfiles-sync` - sync local Git/SSH/GPG/npm config into the container
- `bitwarden-secrets-manager` - `bws` CLI, machine-account-token auth only
- `auto-header` - file headers from project/license/company/contributor info
- `helpers4-common` - shared bootstrap library and git-config self-heal used by the others

[Source code](https://github.com/helpers4/devcontainer) | [Documentation](https://helpers4.dev/devcontainer/)

## GitHub Actions

[helpers4/action](https://helpers4.dev/action/) is a collection of reusable GitHub Actions for consistent, automated workflows.

### Conventional Commits
*Validate commit messages against the Conventional Commits specification*

The [`conventional-commits`](https://helpers4.dev/action/actions/conventional-commits/) action enforces the [Conventional Commits](https://www.conventionalcommits.org/) format on every PR. Configurable commit types and optional scope requirement.

```yaml
- uses: helpers4/action/conventional-commits@v1
  with:
    types: 'feat|fix|docs|refactor|test|chore'
    require-scope: false
```

### Setup pnpm
*Node.js + pnpm in one step*

The [`setup-pnpm`](https://helpers4.dev/action/actions/setup-pnpm/) action sets up Node.js and pnpm via the official `pnpm/action-setup`, with optional dependency install.

### PR Status Comment
*One sticky PR comment, not one per push*

The [`pr-status-comment`](https://helpers4.dev/action/actions/pr-status-comment/) action posts or updates a single sticky PR comment summarizing job statuses as a table.

### Dispatch with Fallback
*Cross-repo triggers that survive a transient failure*

The [`dispatch-with-fallback`](https://helpers4.dev/action/actions/dispatch-with-fallback/) action sends a `repository_dispatch` event using a GitHub App token, with an optional second identity retried automatically if the first attempt fails.

[Source code](https://github.com/helpers4/action) | [Documentation](https://helpers4.dev/action/) | [GitHub Marketplace](https://github.com/marketplace?type=actions&query=helpers4)

## Linux

### Tuxery
*A unified Linux app store — one card per app, whatever the source*

[Tuxery](https://tuxery.store) (in active development) aggregates and merges packages from Flatpak (Flathub), Snap (Snapcraft), AppImage, and native (`.deb`, `.rpm`) sources into a single search-first store, so a duplicated app doesn't show up as four different listings. A matching/merge engine groups packages across sources into one unified card, enriched with category and compatibility metadata.

Split across two repos: [`tuxery/app`](https://github.com/tuxery/app) (the Qwik UI) and [`tuxery/catalog`](https://github.com/tuxery/catalog) (source connectors, matching pipeline, and the persisted dataset), so contributors can add a source connector without touching the UI.

[tuxery.store](https://tuxery.store) | [Source code](https://github.com/tuxery)

## Gnome

[gnome-extensions](https://github.com/baxyz/gnome-extensions) is a monorepo for my Gnome Shell extensions.

### Firefox Profiles
*Quick profile switching for Firefox power users*

[Firefox Profiles](https://extensions.gnome.org/extension/7236/firefox-profiles/) is a Gnome extension that simplifies the management of multiple Firefox profiles. Instead of navigating through Firefox's profile manager or using command-line arguments, users can quickly launch Firefox with their desired profile directly from the system indicator menu. This extension is particularly useful for developers, testers, or anyone who maintains separate Firefox profiles for different purposes (work, personal, testing, etc.).

### Browser Hub
*Firefox Profiles, generalized to (almost) any browser*

Browser Hub picks up where Firefox Profiles left off: launch a profile from the indicator menu for Firefox (native, Snap, Flatpak), Floorp, LibreWolf, Waterfox, Zen, IceCat, Palemoon, and more. In development, not yet published to extensions.gnome.org.

### Quick exit
*Quickly exit Gnome Shell and log out, restart, or shut down*

[Quick Exit](https://extensions.gnome.org/extension/10744/quick-exit/) is a Gnome Shell extension that allow to shorten the countdown timer when logging out, restarting, or shutting down the system. It provides a more efficient way to exit the Gnome Shell environment, especially for users who prefer a faster workflow.

## Firefox

### Close Bookmarked Tabs
*Keep your browser organized by closing saved tabs*

[Close Bookmarked Tabs](https://addons.mozilla.org/en/firefox/addon/close-bookmarked-tabs/) ([source code](https://github.com/baxyz/close-bookmarked-tabs)) is a lightweight Firefox extension designed to help users maintain a cleaner browsing experience. The extension identifies all currently open tabs that have been bookmarked and provides a simple way to close them with a single click. This is especially useful for users who tend to accumulate many tabs but want to keep important pages bookmarked for future reference without cluttering their current session.

## Node.js

### mozlz4
*Read and write Firefox's session/bookmark file format from Node, the browser, or GJS*

[mozlz4](https://www.npmjs.com/package/mozlz4) ([source code](https://github.com/baxyz/mozlz4)) encodes and decodes Mozilla's `mozLz40` format, the LZ4-compressed binary format Firefox, Zen Browser, and other Mozilla-based browsers use for files like `sessionstore.jsonlz4`, `zen-sessions.jsonlz4`, and `bookmarks.jsonlz4`. Zero dependencies, TypeScript-first, dual ESM+CJS, and runs in Node.js, browsers, Deno, Bun, and GNOME GJS.

### sqlite-reader
*A read-only SQLite3 binary parser*

[sqlite-reader](https://www.npmjs.com/package/sqlite-reader) ([source code](https://github.com/baxyz/sqlite-reader)) is a lightweight library for parsing SQLite3 binary files in Node.js, browsers, and other environments. It provides a simple API for reading and manipulating SQLite databases without the need for a full SQL engine.

## Sailfish OS (Jolla)

### Mobile Applications
*Please contact me for details about my Sailfish OS app development work*

### Whisperfish Icon Generator
*A small utility for the Whisperfish Signal client*

[whisperfish-icon-generator](https://github.com/baxyz/whisperfish-icon-generator) generates app icons for [Whisperfish](https://github.com/whisperfish/whisperfish), the Signal client for Sailfish OS.

### Translations
I actively contribute to the French localization of 10+ Sailfish OS applications since 2021. [See complete list](/extra/translations)

## Android

### Translations
I contribute to French translations for Android applications, helping make open-source tools accessible to French-speaking users. [See complete list](/extra/translations)

## SaaS Services

### Feature Today
*Helping address user frustration - More to come*

A service focused on addressing and resolving user frustration points in digital products and services. The project is in development with more details to be announced.

### brig·id
*Self-hosted identity, done properly — in development*

[brig·id](https://github.com/brig-id) is a self-hosted identity provider built around passkeys (WebAuthn), OIDC, and hybrid post-quantum cryptography, aimed at privacy-respecting, decentralized-compatible authentication (DID:web) that a team or individual can run themselves. Early-stage: specs and core crates are in progress, no public landing page or release yet.

[GitHub organization](https://github.com/brig-id)

### Other Projects
*Various SaaS initiatives - Contact me for more information*

I have been involved in several other SaaS projects and startup initiatives. Please contact me directly if you would like more details about these ventures.

### data·café (Data Terrae) - Discontinued
*Data processing platform for businesses - Project discontinued*

`data·café` was a SaaS platform developed as part of the Data Terrae startup, designed to help businesses process and analyze their data efficiently. The project was incubated through various startup accelerators but unfortunately did not reach commercial viability. While the startup has since closed, some of the open-source components remain available in the [Data Café GitLab repositories](https://gitlab.com/data-cafe), serving as a testament to the technical innovation that went into the platform.

## Design

### UI/UX Portfolio
*Visual design and user experience work*

As part of my Human-Computer Interaction expertise, I have extensive experience in UI/UX design, interaction design, and user experience optimization. You can explore my design work and case studies in my [portfolio](/portfolio).

## Miscellaneous

### Proton Repository Proxy - Archived
*APT/RPM proxy for Proton's official Linux apps*

A Cloudflare Workers-based APT/RPM repository proxy that redirects to Proton's official app releases (not affiliated with or endorsed by Proton AG). The original repo is archived; docs and maintenance continue under the [proton-makers](https://proton-makers.github.io/proton-repo-proxy/) community project.

### Open-Source Contributions
I regularly contribute to various open-source applications and development tools, focusing on user experience improvements, bug fixes, and feature enhancements. Most of my early contributions from the 2000s are no longer publicly accessible, but I continue to actively participate in the open-source community.
