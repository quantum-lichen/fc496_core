# FC-496 / HSE — Hybrid Strand Engine (implémentation initiale)

Projet : FC-496 (Cellule Fractale 496 bits) + HSE (Hybrid Strand Engine)
Auteur : Bryan Ouellette (quantum-lichen) — prototype et documentation initiale

But
- Rendre consultable et exécutables les artefacts fondamentaux de l'architecture FC-496 / HSE.
- Fournir un prototype Rust minimal (fc496_rust) et la documentation technique (whitepaper, architecture).
- Donner une base pour monter la Phase 3 (performance, ECC avancée, portage Rust complet).

Contenu du dépôt (proposé)
- docs/whitepaper_BCP.md        — Whitepaper résumé + plan d'implémentation
- docs/architecture.md          — Diagrammes et spécifications techniques
- fc496_rust/                   — Prototype Rust minimal (lib skeleton)
  - Cargo.toml
  - src/lib.rs
  - src/ecc.rs
  - src/geo.rs
  - src/time.rs
  - src/utils.rs
- .github/workflows/ci.yml      — CI (build, test, bench)
- scripts/archive_project.py    — Archivage reproducible
- README.md                     — Ce fichier

Usage rapide
1. Valide ici les fichiers / demande modifications.
2. Dis "push to quantum-lichen/UICT-CEML-H-Scale branch bcp/initial-implementation" (ou autre branche) et je pousse.
3. Après push : je lance CI et un benchmark de smoke-test.

Remarques
- Les fichiers Rust fournis sont des squelettes fonctionnels : compilation possible et tests unitaires de base inclus.
- Whitepaper : résumé organisé en Markdown. On peut y intégrer la totalité du contenu long brut si tu veux (je peux importer ton fichier Implementation.txt complet dans docs/raw/).
