# JOURNAL — hostrules
<!-- Project journal (French), newest first. -->

---

## 2026-10-16, extraction

- Faite dans la soiree : `rules` (generique `HostRule<X>`, extension flattenee, `NoExt` pour
  les tests), `env`, `read`, `secrets` copies tels quels, `resolve` sorti d'`inventory.rs`
  avec `project_roots`. 22 tests, dont deux sur les promesses (aucune ecriture, aucun
  reseau) qui lisent le code source de la crate — le premier a d'abord attrape les
  fixtures des tests unitaires, exclues depuis.
- MCProster migre dans le cloud en une passe : `hosts.rs` reduit a `McpLocation` + regles
  embarquees, trois modules supprimes, re-exports `env`/`read`/`secrets` pour garder les
  chemins. Sorties `--json` identiques sauf `hosts` (`hints`). Clippy propre.

## 2026-10-16, naissance

- Troisieme outil Blackberrylabs (Permitt) → regle de la convention du 16/10 : la fondation
  commune s'extrait au troisieme outil, pas avant. Option C choisie par Alexandre : le coeur
  maintenant, l'UI apres Permitt.
- Perimetre : regles d'hotes sourcees, env, lecteurs, masquage, resolution d'emplacements.
  Les regles elles-memes restent a chaque outil. Nom verifie libre sur crates.io.
