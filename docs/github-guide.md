# Guide GitHub

## Vocabulaire

- **Dépôt (repository) :** dossier versionné d'un projet.
- **Issue :** ticket pour proposer, signaler ou discuter.
- **Branche :** copie de travail isolée.
- **Commit :** enregistrement d'un changement.
- **Pull Request (PR) :** demande d'intégration d'une branche dans `main`.
- **Fork :** copie personnelle d'un dépôt, pour contribuer sans droits d'écriture.

## Nommage des dépôts

Minuscules, mots séparés par des tirets, nom qui décrit la fonction : `resources`, `community-handbook`, `community-projects`.

## Branches

| Branche | Usage |
| --- | --- |
| `main` | Version principale, protégée |
| `docs/nom-du-sujet` | Documentation |
| `feat/nom-fonctionnalite` | Fonctionnalité ou contenu structurant |
| `fix/nom-correction` | Correction |
| `chore/nom-tache` | Maintenance |

Les branches temporaires sont supprimées après fusion.

## Commits

```text
docs: add contribution guide
feat: add resource template
fix: correct broken resource link
chore: reorganize resource folders
```

Préfixes : `feat`, `fix`, `docs`, `chore`, `refactor`, `test`.

## Pull Requests

Chaque PR doit :

- Avoir un titre compréhensible.
- Expliquer le changement (le modèle est pré-rempli).
- Référencer l'Issue liée (`Closes #12`).
- Indiquer les vérifications réalisées.
- Signaler les impacts sur d'autres dossiers.
- Être relue par une autre personne que l'auteur lorsque c'est possible.

## Labels

| Label | Usage |
| --- | --- |
| `good first issue` | Tâche accessible aux débutants |
| `help wanted` | Besoin de contributeurs |
| `documentation` | Documentation |
| `bug` | Problème à corriger |
| `enhancement` | Amélioration |
| `question` | Question |
| `resource` | Proposition de ressource |
| `activity` | Activité |
| `project` | Projet |
| `priority: high/medium/low` | Priorité |
| `status: triage` | À examiner |
| `status: in progress` | En cours |
| `status: blocked` | Bloqué |

Les labels sont des outils de classement, pas une garantie de délai.

## Contribuer pas à pas (sans droits d'écriture)

```bash
# 1. Forker le dépôt depuis l'interface GitHub, puis :
git clone https://github.com/<ton-pseudo>/resources.git
cd resources
git checkout -b docs/ajout-ressource-python
# 2. Modifier les fichiers
git add .
git commit -m "docs: add python official tutorial"
git push origin docs/ajout-ressource-python
# 3. Ouvrir la Pull Request depuis GitHub
```

## Suivi du travail

Les tâches de l'organisation sont suivies dans le GitHub Project **Community Operations** (vues Board, Table, Roadmap).

- Une tâche importante a une Issue.
- Une tâche en cours a un responsable.
- Une tâche bloquée explique le blocage.
- Une tâche terminée satisfait ses critères d'acceptation.
