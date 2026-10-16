# CLAUDE.md — bbl-hostrules
<!-- Working rules for Claude in this repository (French). Code and docs are in English. -->

`bbl-hostrules` (`use bbl_hostrules::…`) : crate Rust commune aux outils Blackberrylabs (MCProster, Permitt) — regles
d'hotes sourcees, environnement, lecteurs JSON/JSONC/TOML/YAML, masquage des secrets,
resolution d'emplacements. Lecture seule, aucun reseau, aucune interface.

## Regles de travail

- BRIEF valide avant le code ; PLAN et JOURNAL tenus ; `00_cadrage/` hors git.
- Aucune API d'ecriture de fichier, aucune dependance reseau, aucune regle embarquee.
- Un changement d'API se verifie sur les deux outils (MCProster : 33 tests et `--json`
  identique) avant d'etre commite.
- Commits locaux libres ; `git push`, suppression de fichiers, tags : accord explicite.
  Commandes completes, chemin absolu (`cd /home/nushoko/Bureau/Logiciels/Bbl_hostrules && …`).
- Anglais : code, commentaires, commits, README. Francais : pilotage.
- Seul nom cite : Alexandre Do.

## Identite git

Avant le **premier commit** : `git config user.name "Alexandre Do"` et
`git config user.email "277202463+Nimeria2026@users.noreply.github.com"` (config locale) ;
verifier `git log --format='%an <%ae>'` avant tout push.
