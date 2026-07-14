# AGENTS.md

## Repo in brief
VS Code color theme extension (One Dark Miku). The theme is defined in a single file: `themes/One dark miku-color-theme.json`.

## Commands
- `pnpm run package` — produce `one-dark-miku.vsix` via `@vscode/vsce`
- `pnpm run validate` — lint the extension manifest with `vsce ls`

## Dev workflow
- Run and debug from VS Code: press **F5** (uses `.vscode/launch.json` → `ExtensionHost` debugger).
- Edit `themes/One dark miku-color-theme.json`, then reload VS Code window to preview.
- `.npmrc` restricts native builds to `@vscode/vsce-sign` and `keytar`.

## Packaging / publishing (manual)
1. `pnpm install`
2. `pnpm run package` — produces `.vsix` in the repo root (gitignored).
3. Publish via `pnpm exec vsce publish` (requires `NPM_TOKEN` env var set by `@vscode/vsce`).

## Style / conventions
- Colors: Miku palette centered on `#39C5BB` / `#48FFF4`.
- `package.json` `"files"` array is the single source of truth for what lands in the `.vsix`; no `.vscodeignore`.
- Changelog lives in `CHANGELOG.md`, versioned alongside `package.json` version.

## Gotchas
- No tests, linters, CI, or lock-file enforcement beyond `pnpm-lock.yaml`.
- The `one-dark-miku-*.vsix` bundles committed in the repo are **not** tracked by git (see `.gitignore`). If you need them, rebuild with `pnpm run package`.
