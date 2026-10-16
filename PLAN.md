# PLAN — bbl-hostrules
<!-- Project plan (French). -->

## Etape 0. Cadrage
- [x] BRIEF rev. 1 — 2026-10-16
- [x] Validation par Alexandre (H2, H3) — 2026-10-16
- [x] Depot local, identite noreply, commit 1, depot `blackberrylabs/hostrules` public — 2026-10-16

## Etape 1. Extraction (rules, env, read, secrets, resolve ; tests ; clippy)
- [x] Crate ecrite, 22 tests verts, clippy propre — 2026-10-16
## Etape 2. Migration MCProster 0.2.1 (sorties identiques, 33 tests) — release sur accord
- [x] MCProster migre dans le cloud : `--json list/findings/files` identiques octet pour octet au faux home ; `hosts --json` : `remove_hint`/`list_hint` → `hints` (seul changement) — 2026-10-16
- [x] MCProster 0.2.1 sur `tag = "v0.1.0"`, passage reel identique — 2026-10-16 ; release 0.2.1 : plus tard
## Etape 3. Tag v0.1.0 — sur accord ; Permitt demarre dessus
- [x] Tag v0.1.0 pousse — 2026-10-16

## Etape 4. Version 0.2.0 — extension par hote
- [x] `HostRule<X, H = NoExt>` + `HostExtension` ; MCProster verifie inchange (compile contre 0.2.0) — 2026-10-16
- [x] 23 tests, clippy propre — 2026-10-16
- [x] Commit 2, push, tag v0.2.0 — 2026-10-16

## Etape 5. crates.io — a decider (condition remplie : deux outils, API tenue)

## Etape 6. Renommage `bbl-hostrules` (decision H4, 2026-10-16)
- [x] Dossier local renomme `Bbl_hostrules` — 2026-10-16
- [ ] Depot GitHub renomme, remote mis a jour, commit 0.3.0, tag v0.3.0
- [ ] Permitt et MCProster sur `bbl-hostrules` v0.3.0, sorties identiques
