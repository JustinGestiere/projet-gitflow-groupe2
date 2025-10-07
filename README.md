# TP-GitFlow
Quentin / Robin / Justin

Site de vente de booster de kayou

## Workflow Git Flow

![alt text](image.png)

| ------------------------------------------------ | ----------------------- | --------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Initialisation**                               | `master` + `develop`    | `git flow init`                                                             | Met en place les branches de base (master, develop) et les préfixes (feature/, release/, hotfix/) ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité"))           |
| **Développement d’une fonctionnalité (feature)** | `feature/…`             | `git flow feature start <nom>` puis `git flow feature finish <nom>`         | Travail isolé pour chaque nouvelle fonctionnalité, fusion vers `develop` après validation ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité"))                   |
| **Création d’une version (release)**             | `release/…`             | `git flow release start <version>` puis `git flow release finish <version>` | Préparation et tests avant mise en production ; fusion vers `master` + tag + retour vers `develop` ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité"))          |
| **Correction urgente en production (hotfix)**    | `hotfix/…`              | `git flow hotfix start <nom>` puis `git flow hotfix finish <nom>`           | Permet de corriger rapidement un bug bloquant directement depuis `master`, et fusionne aussi dans `develop` ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité")) |