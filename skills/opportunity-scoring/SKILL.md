---
name: opportunity-scoring
description: Évalue et classe les lots Interencheres selon leur potentiel, leurs risques et les priorités business définies dans docs/inbox/lots-priority.md.
---

# But
Attribuer un score global à chaque lot et classer les opportunités.

# Entrée
Lire :
- AGENTS.md
- docs/inbox/lots-priority.md
- docs/reports/lot-analysis.md
- docs/reports/risk-review.md
- docs/state/quality-gate.md si disponible

# Travail à faire
Pour chaque lot :
- évaluer l’adéquation avec les priorités business
- tenir compte du potentiel de revente
- tenir compte du niveau de risque
- tenir compte de la lisibilité du lot
- pénaliser fortement les informations manquantes
- pénaliser les lots incompatibles avec le budget ou le risque acceptable
- attribuer un score global sur 10
- classer les lots du meilleur au moins intéressant

# Sortie obligatoire
Écrire uniquement dans :
- docs/reports/scored-opportunities.md

# Format obligatoire
Pour chaque lot :
- Score global /10
- Points forts
- Points faibles
- Compatibilité avec les priorités business
- Niveau de confiance
- Verdict court

Puis ajouter :
- Classement final des lots
- Top opportunités
- Lots à surveiller
- Lots à éviter

# Contraintes
- Ne modifier aucun autre fichier
- Ne pas inventer d’informations
- Utiliser INCERTAIN si la qualité des données réduit fortement la confiance
- Le score doit être cohérent avec les analyses déjà produites