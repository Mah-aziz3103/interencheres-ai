# AGENTS.md

## Objectif du projet

Ce projet analyse des lots Interencheres via plusieurs agents specialises et produit des rapports structures.

## Architecture multi-agents

- `lot-analyst` lit `docs/inbox/lots-to-analyze.md` et ecrit `docs/reports/lot-analysis.md`.
- `risk-analyst` lit `docs/inbox/lots-to-analyze.md` et ecrit `docs/reports/risk-review.md`.
- `decision-agent` lit `docs/reports/lot-analysis.md` et `docs/reports/risk-review.md` puis ecrit `docs/reports/daily-summary.md`.

## Regles de travail

- Toujours lire les fichiers d'entree requis avant de produire un rapport.
- Ecrire les resultats uniquement dans `docs/reports/` ou `docs/state/`.
- Ne jamais inventer une information manquante.
- Utiliser `INCERTAIN` si une information manque, ne peut pas etre verifiee, ou reste ambigue.
- Preferer des sorties structurees avec titres, sous-titres, listes courtes et conclusions.
- Garder les modifications limitees a la tache demandee.

## Format de sortie attendu

Chaque rapport doit contenir :

1. Resume
2. Analyse
3. Risques
4. Recommandation
5. Prochaine action

## Contraintes

- Ne pas supprimer de fichiers existants sans raison explicite.
- Ne pas modifier le code applicatif si la tache concerne seulement l'analyse documentaire.
- Ne modifier aucun autre fichier quand la demande porte uniquement sur `AGENTS.md`.

## Règles d'exploitation
- Toute synthèse finale doit tenir compte de docs/state/quality-gate.md si ce fichier existe.
- Toute exécution complète du pipeline doit être journalisée dans docs/state/run-log.md.
- Toute décision finale utile doit être enregistrée dans docs/state/decisions-history.md.
- Si le quality gate échoue, la décision finale doit signaler clairement FAIL ou INCERTAIN.
