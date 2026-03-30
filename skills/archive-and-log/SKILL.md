---
name: archive-and-log
description: Enregistre un résumé d'exécution du pipeline dans docs/state/run-log.md et ajoute la décision finale dans docs/state/decisions-history.md.
---

# But
Tracer l'exécution du pipeline après la synthèse finale.

# Entrée
Lire :
- AGENTS.md
- docs/reports/daily-summary.md
- docs/state/pipeline-status.json
- docs/state/quality-gate.md

# Travail à faire
- ajouter une entrée datée dans docs/state/run-log.md
- ajouter une entrée synthétique dans docs/state/decisions-history.md
- résumer :
  - le statut global
  - les meilleures opportunités
  - les lots à éviter
  - la recommandation finale
  - l’état du quality gate

# Sorties obligatoires
Écrire uniquement dans :
- docs/state/run-log.md
- docs/state/decisions-history.md

# Format obligatoire

## Pour run-log.md
- Date / heure
- Statut pipeline
- Quality gate
- Rapport final utilisé
- Résumé court

## Pour decisions-history.md
- Date / heure
- Lot recommandé
- Lots à éviter
- Décision
- Niveau de confiance
- Motif court

# Contraintes
- Ne modifier aucun autre fichier
- Ne rien inventer
- Si la décision finale est incomplète, le signaler