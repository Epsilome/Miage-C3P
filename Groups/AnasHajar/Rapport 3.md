# Rapport week 3 Hajar

## Ce que j'ai fait
- **Exercice Chess (Échecs)** :
  - Choix de la pièce : prise en charge et correction du comportement du pion (`MyPawn`).
  - Correction du déplacement : gestion du blocage en cas d'obstacle devant le pion.
  - Implémentation de la capture diagonale des pièces adverses via `targetSquaresLegal:`.
  - Écriture des tests unitaires associés dans `MyPawnTest` pour valider les règles en TDD.
- **Vidéos & Cours** :
  - Visionnage des vidéos demandées pour cette semaine.

## Ce que je n'ai pas encore fait (et pourquoi)
- **Déclic / Assimilation complète du cours** :
  - Même si j'ai regardé les vidéos, je n'ai pas encore eu le déclic (*« aha moment »*).
  - Je dois revoir les vidéos et relire les slides pour bien intégrer la mécanique de lookup entre `self` et `super` dans des scénarios plus complexes.

## Difficultés rencontrées & Solutions
- **Déplacement en diagonale du pion** :
  - *Problème* : tentative d'appeler directement des messages inexistants sur la case (`upLeft`, etc.), ce qui levait des erreurs.
  - *Solution* : composition des déplacements verticaux et horizontaux (`square up left`) avec vérification des bords (`nil`).
- **Confusion de dépôt Git** :
  - *Problème* : tentative initiale de commiter le travail directement sur le dépôt source plutôt que sur mon fork personnel.
  - *Solution* : vérification de la configuration du remote dans Iceberg pour pointer vers mon propre dépôt avant d'effectuer les commits et pushs.
