# Change Log

## v1.1.1

- **Semantic Highlighting**: Refined `semanticTokenColors` — removed 12 entries (`class.name`, `function.call`, `function.definition`, `function.macro`, `variable.readonly`, `parameter.declaration`, `parameter.labelParameter`, `type.defaultLibrary`, `interface.name`, `keyword.control`, `keyword.operator`, `variable.static`, `function.async`). Added `enumMember` (`#58c1cf`) and `variable.constant` (`#e6a971`). Updated `variable.defaultLibrary` from `#39C5BB` to `#e9bd6c`.

## v1.1.0

- **Refactor**: Migrated to `pnpm@10` and installed `@vscode/vsce` locally as a dev dependency for faster, consistent builds.
- **Theme**: Integrated custom Miku color palette (`#39C5BB`, `#48FFF4`) across 115+ UI tokens.
- **Configuration**: Removed legacy `.vscodeignore` in favor of explicit `"files"` array to optimize package size.
- **Metadata**: Renamed extension from "One dark sweet" to "One dark Miku".

## v1.0.0

- Initial release!
