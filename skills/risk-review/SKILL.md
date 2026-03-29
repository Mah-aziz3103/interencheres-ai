\---

name: risk-review

description: Analyse les risques techniques et commerciaux des lots Interencheres à partir de docs/inbox/lots-to-analyze.md et écrit le rapport dans docs/reports/risk-review.md.

\---



\# But

Évaluer les risques des lots d'enchères présents dans `docs/inbox/lots-to-analyze.md`.



\# Entrée

Lire :

\- `AGENTS.md`

\- `docs/inbox/lots-to-analyze.md`



\# Travail à faire

Pour chaque lot :

\- identifier les risques techniques

\- identifier les risques de revente

\- identifier les informations manquantes

\- donner un niveau de risque

\- utiliser `INCERTAIN` si les données sont insuffisantes



\# Sortie obligatoire

Écrire uniquement dans :

\- `docs/reports/risk-review.md`



\# Format obligatoire

Pour chaque lot :

\- Risques techniques

\- Risques de revente

\- Informations manquantes

\- Niveau de risque

\- Conclusion courte



\# Contraintes

\- Ne modifier aucun autre fichier

\- Ne pas inventer d’informations

\- Garder un style court, lisible et orienté décision

