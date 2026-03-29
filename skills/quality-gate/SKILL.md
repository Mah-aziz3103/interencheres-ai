\---

name: quality-gate

description: Vérifie que les rapports lot-analysis et risk-review existent, sont complets, et n’inventent pas d’informations avant la synthèse finale.

\---



\# But

Contrôler la qualité minimale du pipeline avant la décision finale.



\# Entrée

Lire :

\- `AGENTS.md`

\- `docs/reports/lot-analysis.md`

\- `docs/reports/risk-review.md`



\# Travail à faire

Vérifier :

\- que `docs/reports/lot-analysis.md` existe et contient une section pour chaque lot

\- que `docs/reports/risk-review.md` existe et contient une section pour chaque lot

\- que les sections attendues sont présentes

\- que les informations manquantes sont signalées par `INCERTAIN` au lieu d'être inventées



\# Sortie obligatoire

Écrire uniquement dans :

\- `docs/state/quality-gate.md`



\# Format obligatoire

\- Statut global : PASS ou FAIL

\- Vérifications réussies

\- Problèmes détectés

\- Correctifs recommandés



\# Contraintes

\- Ne modifier aucun autre fichier

\- Ne pas corriger les rapports automatiquement

\- Seulement constater et signalers

