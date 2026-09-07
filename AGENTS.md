# AGENTS.md — baxyz `baxyz.github.io`

This repository inherits the [canonical workspace rules](https://github.com/baxyz/.dev/blob/main/AGENTS.md). Only project-specific details are documented here.

## Scope

GitHub Pages site (Jekyll) at <https://berenger.arnaud.work/> — personal portfolio and
publication list for Bérenger Arnaud. Content only, no build tooling of its own beyond Jekyll.

## License

AGPL-3.0-only, the workspace default.

## Commit Scopes

Defined in `scopes.json`: `content`, `portfolio`, `publication`, `assets`, `deps`, `ci`.

## Structure

```text
baxyz.github.io/
  index.md
  about.md
  portfolio/       ← project write-ups
  publication/     ← publication list
  extra/           ← tools.md, translations.md
  assets/
  _config.yml       ← Jekyll config
  CNAME
```

## Rules

- No runtime code or build pipeline beyond what GitHub Pages' Jekyll build provides.
- Keep `CNAME` and `_config.yml` untouched unless the custom domain or site metadata actually
  changes.
