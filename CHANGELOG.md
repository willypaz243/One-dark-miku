# Change Log

## v1.1.2

- **Accessibility**: Improved contrast for selection backgrounds, status bar items, scrollbar hover, line highlight, and find match highlights. Upgraded editor whitespace and indent guide visibility (`#3b4048` → `#4a5060`). Fixed tab active border and debugging border legibility.
- **Terminal ANSI palette**: Corrected 6 colors — blue brightened to `#3a97ff`, magenta fixed from gray `#A3A3A3` to `#d975e0`, bright green changed from cyan `#48FFF4` to `#a0e07a`, bright blue adjusted to `#6bb3ff`, yellow boosted to `#e6b450`. All 16 ANSI colors are now visibly distinct.
- **Selection states**: Active/inactive selection backgrounds use `#334a63` / `#2d3340` with tints closer to the Miku palette, improving visual hierarchy between focused and unfocused list items.

## v1.1.1

- **Semantic Highlighting**: Refined `semanticTokenColors` — removed 12 entries (`class.name`, `function.call`, `function.definition`, `function.macro`, `variable.readonly`, `parameter.declaration`, `parameter.labelParameter`, `type.defaultLibrary`, `interface.name`, `keyword.control`, `keyword.operator`, `variable.static`, `function.async`). Added `enumMember` (`#58c1cf`) and `variable.constant` (`#e6a971`). Updated `variable.defaultLibrary` from `#39C5BB` to `#e9bd6c`.

## v1.1.0

- **Refactor**: Migrated to `pnpm@10` and installed `@vscode/vsce` locally as a dev dependency for faster, consistent builds.
- **Theme**: Integrated custom Miku color palette (`#39C5BB`, `#48FFF4`) across 115+ UI tokens.
- **Configuration**: Removed legacy `.vscodeignore` in favor of explicit `"files"` array to optimize package size.
- **Metadata**: Renamed extension from "One dark sweet" to "One dark Miku".

## v1.0.0

- Initial release!
