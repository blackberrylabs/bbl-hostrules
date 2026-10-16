# Changelog

## [0.3.0] — 2026-10-16

### Changed

- **Renamed `hostrules` → `bbl-hostrules`** (`use bbl_hostrules::…`), like `bbl-ui` and
  `bbl-report`: the shared foundations of the Blackberrylabs tools all carry the family
  prefix. Nothing else changes; the repository moved to
  `github.com/blackberrylabs/bbl-hostrules` (the old address redirects).

## [0.2.0] — 2026-10-16

### Added

- `HostExtension` and the second type parameter of `HostRule<X, H = NoExt>` / `Rules<X, H>`:
  a tool's fields about the host as a whole (Permitt: defaults, settings semantics,
  precedence), flattened next to the common fields and validated by the tool. Existing
  users (`HostRule<X>`) are unchanged.

## [0.1.0] — 2026-10-16

- Extracted from MCProster 0.2.0: `rules`, `env`, `read`, `secrets`, `resolve`.
