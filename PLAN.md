# PLAN — hostrules
<!-- Project plan (French). -->

## Etape 0. Cadrage
- [x] BRIEF rev. 1 — 2026-10-16
- [x] Validation par Alexandre (H2, H3) — 2026-10-16
- [ ] Depot local, identite noreply, `.gitignore`, LICENSE MIT, README — fichiers ecrits le 2026-10-16, commit 1 a lancer

## Etape 1. Extraction (rules, env, read, secrets, resolve ; tests ; clippy)
- [x] Crate ecrite, 22 tests verts, clippy propre — 2026-10-16
## Etape 2. Migration MCProster 0.2.1 (sorties identiques, 33 tests) — release sur accord
- [x] MCProster migre dans le cloud : `--json list/findings/files` identiques octet pour octet au faux home ; `hosts --json` : `remove_hint`/`list_hint` → `hints` (seul changement) — 2026-10-16
- [ ] Dependance git sur le tag v0.1.0 (apres push de hostrules), commit, passage reel, release 0.2.1
## Etape 3. Tag v0.1.0 — sur accord ; Permitt demarre dessus
