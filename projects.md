---
---

# Projects

As a passionate contributor to the open-source ecosystem, I dedicate my spare time to developing tools, extensions, and mobile applications that solve real-world problems.

- [TypeScript (JavaScript)](#typescript-javascript)
- [Dev Container](#dev-container)
- [GitHub Actions](#github-actions)
- [Gnome](#gnome)
- [Firefox](#firefox)
- [Sailfish OS (Jolla)](#sailfish-os-jolla)
- [Android](#android)
- [SaaS Services](#saas-services)
- [Design](#design)
- [Miscellaneous](#miscellaneous)

## TypeScript (JavaScript)

### Helpers4
*TypeScript-first, enterprise-grade utility library — zero dependencies, 100% test coverage*

[helpers4](https://helpers4.dev/) is a JavaScript/TypeScript utility library designed to eliminate the need to rewrite the same helpers across every project. Built around a per-category package architecture for optimal tree-shaking, it covers the practical, real-world helpers that every professional JS/TS project ends up needing. v2 shipped in May 2026 after two years of development and 22 pre-releases.

**12 packages available:**
- `@helpers4/array` - chunk, compact, difference, intersection, union, deepEquals…
- `@helpers4/string` - capitalize, slugify, camelCase, kebabCase, truncate…
- `@helpers4/object` - deepMerge, pick, omit, compact, deepEquals
- `@helpers4/promise` - delay, retry, debounce, throttle
- `@helpers4/date` - daysDifference, isSameDay, toISO8601, Temporal support
- `@helpers4/number` - clamp, isEven, isOdd, sum, inRange
- `@helpers4/function` - debounce, throttle, memoize
- `@helpers4/type` - isString, isNumber, isNull, isNullish, isArray
- `@helpers4/url` - cleanPath, extractPureURI, onlyPath
- `@helpers4/version` - Full SemVer 2.0.0 parsing and comparison
- `@helpers4/observable` - RxJS Observable helpers and operators
- `@helpers4/id` - UUID v7 generation

[Source code](https://github.com/helpers4/typescript) | [Documentation](https://helpers4.dev/typescript) | [v2 release post](https://helpers4.dev/blog/2026-05-23-helpers4-typescript-v2/)

## Dev Container

[helpers4/devcontainer](https://helpers4.dev/devcontainer/) is a collection of plug-and-play DevContainer features for consistent, reproducible development environments. Features are published to `ghcr.io/helpers4/devcontainer` and follow the DevContainer Features specification.

**9 features available:**
- `essential-dev` - Git visualization, editor enhancements, Markdown
- `typescript-dev` - TypeScript/JS dev with import management
- `angular-dev` - Angular dev, port 4200 forwarding
- `vite-plus` - Vite development setup
- `package-auto-install` - Auto-detect and install packages
- `git-absorb` - Automatic absorption of staged changes into logical commits
- `shell-history-per-project` - Persistent shell history isolation per project
- `dotfiles-sync` - Sync local Git/SSH/GPG/npm config
- `peon-ping` - AI agent sound notifications

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

[Source code](https://github.com/helpers4/action) | [Documentation](https://helpers4.dev/action/) | [GitHub Marketplace](https://github.com/marketplace?type=actions&query=helpers4)

## Gnome

### Firefox Profiles
*Quick profile switching for Firefox power users*

[Firefox Profiles](https://extensions.gnome.org/extension/7236/firefox-profiles/) ([source code](https://github.com/baxyz/firefox-profiles)) is a Gnome extension that simplifies the management of multiple Firefox profiles. Instead of navigating through Firefox's profile manager or using command-line arguments, users can quickly launch Firefox with their desired profile directly from the system indicator menu. This extension is particularly useful for developers, testers, or anyone who maintains separate Firefox profiles for different purposes (work, personal, testing, etc.).

## Firefox

### Close Bookmarked Tabs
*Keep your browser organized by closing saved tabs*

[Close Bookmarked Tabs](https://addons.mozilla.org/en/firefox/addon/close-bookmarked-tabs/) ([source code](https://github.com/baxyz/close-bookmarked-tabs)) is a lightweight Firefox extension designed to help users maintain a cleaner browsing experience. The extension identifies all currently open tabs that have been bookmarked and provides a simple way to close them with a single click. This is especially useful for users who tend to accumulate many tabs but want to keep important pages bookmarked for future reference without cluttering their current session.

## Sailfish OS (Jolla)

### Mobile Applications
*Please contact me for details about my Sailfish OS app development work*

### Translations
I actively contribute to the French localization of 10+ Sailfish OS applications since 2021. [See complete list](/extra/translations)

## Android

### Translations
I contribute to French translations for Android applications, helping make open-source tools accessible to French-speaking users. [See complete list](/extra/translations)

## SaaS Services

### Feature Today
*Helping address user frustration - More to come*

A service focused on addressing and resolving user frustration points in digital products and services. The project is in development with more details to be announced.

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

### Open-Source Contributions
I regularly contribute to various open-source applications and development tools, focusing on user experience improvements, bug fixes, and feature enhancements. Most of my early contributions from the 2000s are no longer publicly accessible, but I continue to actively participate in the open-source community.
