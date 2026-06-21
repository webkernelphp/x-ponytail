# x-ponytail

Lazy senior dev mode for AI agents. Inspired by [ponytail](https://github.com/DietrichGebert/ponytail).

**One file to edit:** [`rules/ponytail.md`](rules/ponytail.md). Everything else is generated.

## Install

```bash
composer install-agent   # from this package
# or
./bin/x-ponytail install
```

Symlinks `dist/` into `~/.grok` and `~/.cursor`. No `AGENTS.md` in your app repos.

## Commands

| Command   | What                             |
| --------- | -------------------------------- |
| `install` | Build `dist/` + symlink globally |
| `build`   | Build `dist/` only               |

After editing `rules/ponytail.md`, re-run `install`.

## Layout

```
rules/ponytail.md              ← edit this
templates/skill-header.md      ← YAML frontmatter only
templates/cursor-header.mdc    ← YAML frontmatter only
dist/                          ← generated, gitignored
src/Installer.php
bin/x-ponytail
```

## Usage

- Default: rules load every session
- `/ponytail lite|full|ultra` — intensity
- `stop ponytail` — off

## License

MIT
