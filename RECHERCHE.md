## 1 – Recherche et compréhension
1. Présentation de Git Flow :

Gitflow est une extension / un modèle de workflow Git conçu pour apporter de la rigueur à la gestion de version dans les projets d’envergure.

GitFlow repose sur le workflow de création de branches repartie en plusieurs fonctionnalité. 

| État / étape                                     | Branche concernée       | Actions & commandes principales                                             | But / rôle                                                                                                                                                                                                                                                                               |
| ------------------------------------------------ | ----------------------- | --------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Initialisation**                               | `master` + `develop`    | `git flow init`                                                             | Met en place les branches de base (master, develop) et les préfixes (feature/, release/, hotfix/) ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité"))           |
| **Développement d’une fonctionnalité (feature)** | `feature/…`             | `git flow feature start <nom>` puis `git flow feature finish <nom>`         | Travail isolé pour chaque nouvelle fonctionnalité, fusion vers `develop` après validation ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité"))                   |
| **Création d’une version (release)**             | `release/…`             | `git flow release start <version>` puis `git flow release finish <version>` | Préparation et tests avant mise en production ; fusion vers `master` + tag + retour vers `develop` ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité"))          |
| **Correction urgente en production (hotfix)**    | `hotfix/…`              | `git flow hotfix start <nom>` puis `git flow hotfix finish <nom>`           | Permet de corriger rapidement un bug bloquant directement depuis `master`, et fusionne aussi dans `develop` ([Les e-novateurs](https://les-enovateurs.com/gitflow-workflow-git-incontournableprojets-de-qualite "Gitflow – Le workflow Git incontournable pour des projets de qualité")) |


![alt text](image.png)

- Avantages :
	- historique de projet
	- grosse structure claire 
	- Travail en parallèle facile
	- séparation nette entre le développement et la prod

- limites :
	- demande de la rigueur 



2. Explication du versionnement sémantique (SemVer) :
3. Le rôle du changelog et de la documentation de version :
4. Le lien entre issues, milestones, et releases sur GitHub :