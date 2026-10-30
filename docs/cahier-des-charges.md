# CAHIER DES CHARGES MAÎTRE

# Création et déploiement d'une communauté informatique collaborative

> **Statut :** document de référence pour l'équipe chargée de construire
> la communauté.\
> **Version :** 1.0\
> **Langue :** français\
> **Nom de la communauté :** `Omada for eureka`\
> **Organisation GitHub :** `Omada-for-eureka`\
> **Serveur Discord :** `[NOM_SERVEUR_DISCORD]`\
> **Responsable du déploiement :** `[RESPONSABLE]`\
> **Date de lancement cible :** `[DATE]`

------------------------------------------------------------------------

# 0. Instructions d'utilisation du document

Ce document décrit ce qui doit être construit, comment le construire et
comment vérifier que le travail est terminé. Il est destiné à être
confié à une ou plusieurs personnes.

## 0.1 Règles pour l'équipe d'exécution

1.  Lire le document avant de commencer.
2.  Ne pas remplacer les noms entre crochets sans accord de l'équipe
    fondatrice.
3.  Créer les éléments dans l'ordre des phases, sauf dépendance
    explicitement indiquée.
4.  Ne jamais publier de mot de passe, jeton, clé API ou donnée
    personnelle dans GitHub ou Discord.
5.  Ne pas donner les droits Owner GitHub ou Administrator Discord à
    tous les membres.
6.  Faire valider les changements sensibles par un autre responsable.
7.  Documenter toute décision qui modifie l'architecture.
8.  Cocher une tâche uniquement lorsque son critère d'acceptation est
    vérifié.
9.  Utiliser des Issues GitHub pour répartir les tâches et garder une
    trace des décisions.
10. Ne pas ajouter des bots, outils ou fonctionnalités simplement parce
    qu'ils existent : chaque intégration doit répondre à un besoin réel.

## 0.2 Placeholders à remplacer

  Placeholder          Valeur à renseigner
  -------------------- --------------------------------------
  `Omada for eureka`   Nom officiel
  `Omada-for-eureka`       Identifiant de l'organisation GitHub
  `[DISCORD_INVITE]`   Lien d'invitation Discord
  `[EMAIL_CONTACT]`    Adresse de contact publique
  `[SITE_WEB]`         Site web, si disponible
  `[DATE]`             Date ou période cible
  `[RESPONSABLE]`      Responsable de la tâche ou du projet

## 0.3 Résultat final attendu

À la fin du déploiement, la communauté doit disposer de :

-   Une organisation GitHub sécurisée et documentée.
-   Des dépôts structurés pour la gouvernance, les ressources, les
    projets, les activités et les automatisations.
-   Un processus ouvert de contribution.
-   Des rôles et responsabilités compréhensibles.
-   Un serveur Discord organisé et modéré.
-   Une liaison fonctionnelle entre GitHub et Discord.
-   Un calendrier d'activités et un premier programme.
-   Une documentation permettant à de nouveaux responsables de reprendre
    le travail.
-   Un processus d'amélioration continue.

------------------------------------------------------------------------

# 1. Vision, mission et périmètre

## 1.1 Mission

`Omada for eureka` est une communauté collaborative d'étudiants et de
passionnés d'informatique. Elle a pour mission de favoriser
l'apprentissage collectif, le partage de connaissances, la réalisation
de projets et l'entraide technique.

La communauté doit permettre à chacun, quel que soit son niveau, de :

-   Découvrir des technologies et des domaines de l'informatique.
-   Partager des ressources fiables.
-   Apprendre auprès d'autres membres.
-   Proposer et organiser des activités.
-   Participer à des projets collaboratifs.
-   Présenter ses réalisations.
-   Développer ses compétences techniques et humaines.
-   Contribuer à un patrimoine de connaissances durable.

## 1.2 Principes de fonctionnement

1.  **Ouverture :** tout membre peut proposer une ressource, une
    activité ou un projet.
2.  **Contribution :** les membres peuvent contribuer sans être
    administrateurs.
3.  **Responsabilité :** chaque activité ou projet doit avoir un
    responsable identifié.
4.  **Transparence :** les règles, décisions et procédures sont
    documentées.
5.  **Respect :** les échanges doivent rester respectueux et
    constructifs.
6.  **Qualité :** les ressources et contributions sont vérifiées avant
    intégration.
7.  **Continuité :** les connaissances ne doivent pas dépendre d'une
    seule personne.
8.  **Sécurité :** les accès sont limités au besoin réel de chaque rôle.

## 1.3 Périmètre fonctionnel

  -----------------------------------------------------------------------
  Domaine                 Fonction attendue       Plateforme principale
  ----------------------- ----------------------- -----------------------
  Présentation et         Mission, règles, rôles, GitHub
  gouvernance             procédures              

  Bibliothèque            Cours, documentations,  GitHub
                          tutoriels, outils et    
                          liens                   

  Projets                 Code, tâches,           GitHub
                          documentation et        
                          contributions           

  Activités               Challenges, ateliers,   GitHub + Discord
                          événements et comptes   
                          rendus                  

  Discussions             Questions, entraide et  Discord
                          débats                  

  Annonces                Informations            Discord
                          officielles             

  Coordination            Organisation et suivi   GitHub Projects +
                          des tâches              Discord

  Automatisation          Notifications et bot    GitHub + Discord
                          communautaire éventuel  

  Portail futur           Recherche et            Évolution ultérieure
                          présentation            
                          centralisée             
  -----------------------------------------------------------------------

**Règle :** Discord ne doit pas devenir l'unique endroit où une
connaissance importante est conservée. Les décisions, tutoriels,
supports et comptes rendus durables doivent être archivés sur GitHub.

------------------------------------------------------------------------

# 2. Architecture générale

``` text
[NOM_COMMUNAUTE]
|
+-- GITHUB ORGANIZATION
|   |
|   +-- community-handbook
|   |   +-- Mission, règles, rôles, gouvernance
|   |   +-- Guides et procédures
|   |
|   +-- resources
|   |   +-- Programmation
|   |   +-- Informatique fondamentale
|   |   +-- Web, mobile, IA, cybersécurité
|   |   +-- Outils, plugins, formations
|   |
|   +-- community-projects
|   |   +-- Projets collaboratifs
|   |   +-- Issues et pull requests
|   |   +-- Documentation des projets
|   |
|   +-- activities
|   |   +-- Challenges
|   |   +-- Ateliers
|   |   +-- Tech talks
|   |   +-- Comptes rendus
|   |
|   +-- community-bot [phase ultérieure]
|   |   +-- Commandes Discord
|   |   +-- Intégrations
|   |   +-- Tests et documentation
|   |
|   +-- community-website [phase ultérieure]
|       +-- Portail web
|
+-- DISCORD SERVER
|   |
|   +-- Accueil et informations
|   +-- Communauté et entraide
|   +-- Ressources et outils
|   +-- Espaces d'apprentissage
|   +-- Activités et projets
|   +-- Salons vocaux
|
+-- INTÉGRATIONS
    +-- Notifications GitHub vers Discord
    +-- Bots de modération et événements si nécessaires
    +-- Bot communautaire développé par l'équipe, plus tard
```

## 2.1 Règles d'architecture

-   Utiliser une GitHub Organization et non le compte personnel d'un
    fondateur comme propriétaire unique des ressources.
-   Commencer avec cinq dépôts maximum : les quatre dépôts essentiels
    et, éventuellement, un dépôt de bot uniquement lorsqu'il est
    développé.
-   Ne pas créer un dépôt par langage ou par technologie pour la
    bibliothèque : utiliser des dossiers dans `resources`.
-   Les projets autonomes peuvent avoir leur propre dépôt lorsque leur
    taille, leur équipe ou leur cycle de livraison le justifie.
-   Garder les fichiers de gouvernance accessibles publiquement lorsque
    cela ne présente aucun risque.
-   Ne pas publier les informations privées des membres.

------------------------------------------------------------------------

# 3. Organisation GitHub

## 3.1 Création de l'organisation

**Action :** créer une organisation GitHub sous le nom `Omada-for-eureka`.

Procédure :

1.  Se connecter à son compte GitHub personnel.
2.  Ouvrir `https://github.com/account/organizations/new`.
3.  Choisir un plan adapté au budget et aux besoins. Le plan Free suffit
    généralement pour commencer.
4.  Choisir le nom de l'organisation.
5.  Renseigner l'adresse de contact.
6.  Finaliser la création.
7.  Ajouter un deuxième responsable de confiance lorsque cela est
    pertinent, sans multiplier les propriétaires.
8.  Vérifier que l'organisation apparaît dans le menu du compte.

## 3.2 Profil de l'organisation

Renseigner :

-   Nom : `Omada for eureka`
-   Description :
    `Communauté collaborative d'étudiants et passionnés d'informatique : apprentissage, partage de ressources, projets et innovation.`
-   Email : `[EMAIL_CONTACT]`
-   Site : `[SITE_WEB]`, si disponible
-   Localisation : facultative
-   Logo : visuel officiel de la communauté
-   Liens : Discord, site et autres canaux officiels

### Texte de présentation prêt à copier

``` text
[NOM_COMMUNAUTE] is a collaborative community for computer science students and technology enthusiasts.

Our mission is to learn together, share useful resources, build collaborative projects, organize technical activities and help every member grow.

Everyone can contribute, propose ideas, share knowledge and participate in community projects.
```

## 3.3 Sécurité de l'organisation

À configurer :

-   [ ] Exiger l'authentification à deux facteurs pour les membres
    lorsque l'option est disponible.
-   [ ] Limiter les propriétaires (`Owners`) aux fondateurs
    indispensables.
-   [ ] Examiner les permissions par défaut des membres.
-   [ ] Utiliser les équipes pour attribuer les accès aux dépôts.
-   [ ] Désactiver ou limiter la création de dépôts par tous les membres
    si cela est nécessaire à la gouvernance.
-   [ ] Examiner régulièrement les membres et les invitations en
    attente.
-   [ ] Retirer les accès qui ne sont plus nécessaires.
-   [ ] Ne jamais mettre de secrets dans les dépôts.
-   [ ] Activer les alertes de sécurité et outils disponibles selon le
    plan.
-   [ ] Prévoir au moins deux personnes capables d'assurer la continuité
    de l'administration, avec des droits adaptés.

**Critère de validation :** seuls les responsables autorisés peuvent
modifier les paramètres sensibles de l'organisation.

------------------------------------------------------------------------

# 4. Rôles, responsabilités et permissions

Les rôles Discord et GitHub sont deux systèmes différents. Une personne
peut avoir un rôle sur Discord sans recevoir automatiquement les mêmes
permissions sur GitHub.

## 4.1 Organigramme

``` text
                    FONDATEURS / OWNERS
                            |
             +--------------+--------------+
             |              |              |
        Administration   Coordination   Référents
             |              |              |
        Modération     Responsables     Mainteneurs
                       d'activités      GitHub
             |              |              |
             +--------------+--------------+
                            |
                      CONTRIBUTEURS
                            |
                         MEMBRES
```

Cet organigramme représente les responsabilités, pas une hiérarchie de
valeur entre les membres.

## 4.2 Rôles et missions

### A. Fondateur / Owner

Mission : - Définir la vision et les grandes orientations. - Administrer
l'organisation GitHub. - Gérer les paramètres sensibles. - Désigner les
responsables. - Assurer la continuité du projet. - Arbitrer les
décisions majeures.

Limites : - Ne pas gérer seul toutes les activités. - Ne pas utiliser
les droits d'administration pour empêcher les contributions légitimes. -
Documenter les décisions importantes.

### B. Administrateur communautaire

Mission : - Coordonner le fonctionnement général. - Suivre les
responsables. - Organiser les réunions de coordination. - Veiller au
respect des règles. - Gérer les incidents importants. - Suivre la
feuille de route.

Permissions : - Administration Discord selon le besoin. - Gestion des
tâches de coordination. - Pas de droit Owner GitHub automatique.

### C. Modérateur

Mission : - Faire respecter les règles. - Accueillir et orienter les
membres. - Prévenir le spam, le harcèlement et les abus. - Traiter les
signalements. - Faire remonter les incidents graves aux administrateurs.

Permissions : - Gérer les messages et incidents selon les permissions
Discord attribuées. - Pas de gestion des paramètres sensibles de
l'organisation GitHub.

### D. Mainteneur GitHub

Mission : - Examiner les Issues et Pull Requests. - Vérifier la qualité
des ressources. - Maintenir l'organisation des dépôts. - Corriger les
erreurs documentaires. - Aider les contributeurs. - Veiller à la
cohérence des fichiers.

Permissions : - Write ou Maintain sur les dépôts concernés selon la
tâche. - Pas de Owner par défaut.

### E. Responsable de domaine

Exemples : responsable Python, web, cybersécurité, IA, DevOps.

Mission : - Animer un domaine technique. - Identifier les ressources
pertinentes. - Proposer des ateliers. - Orienter les membres. -
Coordonner les contributions du domaine.

Permissions : - Pas de droits globaux automatiques. - Accès de
contribution aux dépôts concernés.

### F. Responsable d'activité

Mission : - Transformer une proposition en activité réalisable. -
Définir les objectifs et le programme. - Recruter des intervenants si
nécessaire. - Annoncer l'activité. - Gérer les inscriptions et la
séance. - Publier le compte rendu et les supports.

Permissions : - Gestion du contenu de l'activité. - Publication dans les
salons autorisés. - Pas de droits d'administration globaux.

### G. Mentor

Mission : - Aider les membres à progresser. - Répondre aux questions. -
Accompagner les débutants. - Proposer des exercices et ressources. -
Encourager l'autonomie.

Permissions : - Accès aux espaces d'entraide. - Pas de privilège
technique automatique.

### H. Contributeur

Mission : - Ajouter ou corriger des ressources. - Contribuer au code et
à la documentation. - Participer aux projets. - Proposer des
améliorations.

Permissions : - Issues, discussions et Pull Requests. - Accès en
écriture uniquement lorsque nécessaire.

### I. Membre

Mission : - Participer aux discussions. - Apprendre et partager. -
Proposer des idées. - Participer aux activités. - Signaler les
problèmes.

Permissions : - Lecture des ressources publiques. - Participation aux
salons ouverts. - Proposition d'Issues et contributions selon les
règles.

## 4.3 Matrice de permissions recommandée

  ---------------------------------------------------------------------------------------------
  Action                Owner      Admin   Modérateur   Mainteneur   Responsable         Membre
                                 Discord                                activité 
  ---------------- ---------- ---------- ------------ ------------ ------------- --------------
  Paramètres de           Oui        Non          Non          Non           Non            Non
  l'organisation                                                                 
  GitHub                                                                         

  Gérer les dépôts      Selon        Non          Non       Dépôts           Non            Non
  GitHub               besoin                            attribués               

  Examiner les            Oui        Non          Non          Oui   Selon dépôt       Proposer
  Pull Requests                                                                  

  Gérer les salons      Selon        Oui Selon besoin          Non        Salons            Non
  Discord              besoin                                          attribués 

  Modérer les           Selon        Oui          Oui          Non           Non            Non
  messages             besoin                                                    

  Proposer une            Oui        Oui          Oui          Oui           Oui            Oui
  activité                                                                       

  Organiser une           Oui        Oui          Oui          Oui           Oui      Oui, avec
  activité                                                                         coordination

  Proposer une            Oui        Oui          Oui          Oui           Oui            Oui
  ressource                                                                      

  Participer à un         Oui        Oui          Oui          Oui           Oui            Oui
  projet                                                                         
  ---------------------------------------------------------------------------------------------

**Important :** ne pas créer une permission globale « administrateur »
pour chaque responsable. Donner uniquement les droits nécessaires à sa
mission.

## 4.4 Nomination et renouvellement

-   Toute responsabilité doit avoir une description.
-   Toute responsabilité opérationnelle doit avoir un titulaire.
-   Les responsabilités peuvent être volontaires.
-   Les responsables doivent documenter leur travail.
-   Une personne peut cumuler plusieurs rôles.
-   Prévoir un remplaçant pour les tâches critiques.
-   Réexaminer les rôles périodiquement, par exemple tous les trois
    mois.

------------------------------------------------------------------------

# 5. Repositories GitHub : architecture détaillée

## 5.1 Repository `community-handbook`

**Rôle :** source officielle de la gouvernance et du fonctionnement de
la communauté.

### Arborescence

``` text
community-handbook/
|
+-- README.md
+-- CONTRIBUTING.md
+-- CODE_OF_CONDUCT.md
+-- GOVERNANCE.md
+-- ROLES_AND_RESPONSIBILITIES.md
+-- ROADMAP.md
+-- FAQ.md
+-- SECURITY.md
|
+-- docs/
|   +-- getting-started.md
|   +-- github-guide.md
|   +-- discord-guide.md
|   +-- contribution-workflow.md
|   +-- activity-workflow.md
|   +-- project-workflow.md
|   +-- moderation-process.md
|   +-- decision-making.md
|
+-- .github/
    +-- ISSUE_TEMPLATE/
    |   +-- bug_report.yml
    |   +-- documentation.yml
    |   +-- proposal.yml
    +-- PULL_REQUEST_TEMPLATE.md
```

### Description des fichiers

  Fichier                           Contenu obligatoire
  --------------------------------- ------------------------------------------------
  `README.md`                       Présentation, mission, liens et accès
  `CONTRIBUTING.md`                 Comment participer et proposer des changements
  `CODE_OF_CONDUCT.md`              Comportements attendus et interdits
  `GOVERNANCE.md`                   Fonctionnement et prise de décision
  `ROLES_AND_RESPONSIBILITIES.md`   Rôles et missions
  `ROADMAP.md`                      Phases et tâches du projet
  `FAQ.md`                          Réponses aux questions fréquentes
  `SECURITY.md`                     Signalement privé des vulnérabilités
  `getting-started.md`              Guide d'arrivée
  `github-guide.md`                 Issues, branches, commits et PR
  `discord-guide.md`                Salons et rôles Discord
  `contribution-workflow.md`        Parcours d'une contribution
  `activity-workflow.md`            Parcours d'une activité
  `project-workflow.md`             Parcours d'un projet
  `moderation-process.md`           Traitement des signalements
  `decision-making.md`              Décisions et consultation

### Contenu initial de `README.md`

``` markdown
# [NOM_COMMUNAUTE]

Communauté collaborative d'étudiants et passionnés d'informatique.

## Notre mission

Apprendre ensemble, partager des ressources, réaliser des projets et
organiser des activités techniques ouvertes à tous les membres.

## Participer

- Rejoindre Discord : [DISCORD_INVITE]
- Découvrir les ressources : [LIEN_RESOURCES]
- Découvrir les projets : [LIEN_PROJECTS]
- Consulter les activités : [LIEN_ACTIVITIES]

## Comment contribuer ?

1. Lire CONTRIBUTING.md.
2. Ouvrir une Issue pour proposer une idée ou signaler un problème.
3. Créer une Pull Request pour proposer une modification.
4. Échanger avec les mainteneurs si nécessaire.

## Nos valeurs

- Entraide
- Respect
- Curiosité
- Ouverture
- Collaboration
- Partage des connaissances

## Contact

[EMAIL_CONTACT]
```

## 5.2 Repository `resources`

**Rôle :** bibliothèque communautaire de ressources informatiques.

### Arborescence cible

``` text
resources/
|
+-- README.md
+-- CONTRIBUTING.md
+-- LICENSE
|
+-- computer-science/
|   +-- algorithms/
|   +-- data-structures/
|   +-- operating-systems/
|   +-- computer-networks/
|   +-- computer-architecture/
|
+-- programming/
|   +-- python/
|   +-- javascript/
|   +-- typescript/
|   +-- java/
|   +-- c/
|   +-- cpp/
|   +-- php/
|   +-- go/
|   +-- rust/
|
+-- web-development/
|   +-- frontend/
|   +-- backend/
|   +-- fullstack/
|   +-- api/
|
+-- mobile-development/
|   +-- android/
|   +-- ios/
|   +-- cross-platform/
|
+-- databases/
|   +-- relational/
|   +-- nosql/
|   +-- data-modeling/
|
+-- artificial-intelligence/
|   +-- machine-learning/
|   +-- deep-learning/
|   +-- generative-ai/
|   +-- data-science/
|
+-- cybersecurity/
|   +-- fundamentals/
|   +-- web-security/
|   +-- network-security/
|   +-- ethical-practice/
|
+-- devops-cloud/
|   +-- linux/
|   +-- docker/
|   +-- ci-cd/
|   +-- cloud/
|
+-- ui-ux-design/
|
+-- tools-and-plugins/
|   +-- vscode/
|   +-- browser-extensions/
|   +-- developer-tools/
|   +-- productivity/
|
+-- learning-paths/
+-- templates/
    +-- RESOURCE_TEMPLATE.md
```

**Règle d'évolution :** créer les dossiers au fur et à mesure des
contributions. Ne pas remplir le dépôt de dossiers vides.

### Contenu initial de `README.md`

``` markdown
# Community Resources

Bibliothèque de ressources partagées par la communauté.

## Catégories

- Informatique fondamentale
- Programmation
- Développement web
- Développement mobile
- Bases de données
- Intelligence artificielle et data
- Cybersécurité
- DevOps et cloud
- UI/UX
- Outils et plugins
- Parcours d'apprentissage

## Ajouter une ressource

1. Lire CONTRIBUTING.md.
2. Copier le modèle dans templates/RESOURCE_TEMPLATE.md.
3. Ajouter la fiche dans la catégorie correspondante.
4. Ouvrir une Pull Request.

## Règles

- Vérifier les liens.
- Décrire clairement la ressource.
- Indiquer le niveau et la langue.
- Privilégier les sources officielles.
- Respecter les licences et droits d'auteur.
- Ne jamais publier de secrets ou de données privées.
```

### Modèle `templates/RESOURCE_TEMPLATE.md`

``` markdown
# [Nom de la ressource]

- **Catégorie :** [Catégorie]
- **Type :** [Documentation / Cours / Tutoriel / Outil / Vidéo / Autre]
- **Niveau :** [Débutant / Intermédiaire / Avancé / Tous niveaux]
- **Langue :** [Français / Anglais / Autre]
- **Prix :** [Gratuit / Payant / Freemium / Non précisé]
- **Source :** [Officielle / Communautaire / Autre]
- **Lien :** [URL]
- **Contributeur :** [Pseudo GitHub]

## Description

[Expliquer ce que contient la ressource.]

## Pourquoi la recommander ?

[Expliquer ce qu'un membre peut apprendre ou réaliser avec cette ressource.]

## Prérequis

[Indiquer les connaissances nécessaires, si applicable.]

## Licence et conditions d'utilisation

[Indiquer les informations connues. Ne pas supposer qu'un contenu est libre de droits.]
```

### Règles de classement

-   Un fichier Markdown par ressource ou une liste thématique si les
    ressources sont très courtes.
-   Utiliser des noms de fichiers simples, en minuscules, sans espaces.
-   Éviter les copies de contenus protégés.
-   Préférer un lien vers la source officielle plutôt que l'hébergement
    d'un fichier.
-   Mentionner la date de vérification lorsqu'une ressource évolue
    rapidement.
-   Signaler les ressources obsolètes plutôt que les supprimer sans
    explication.

## 5.3 Repository `community-projects`

**Rôle :** index central des projets communautaires et de leurs règles.

### Arborescence

``` text
community-projects/
|
+-- README.md
+-- CONTRIBUTING.md
+-- PROJECT_GUIDELINES.md
|
+-- project-template/
|   +-- README.md
|   +-- REQUIREMENTS.md
|   +-- TEAM.md
|   +-- CONTRIBUTING.md
|   +-- ROADMAP.md
|
+-- proposals/
|   +-- README.md
|
+-- active/
|   +-- README.md
|
+-- completed/
|   +-- README.md
|
+-- archived/
    +-- README.md
```

### Contenu de `README.md`

``` markdown
# Community Projects

Espace de découverte et de coordination des projets de la communauté.

## Cycle de vie

1. Proposition
2. Discussion
3. Validation du périmètre
4. Constitution de l'équipe
5. Développement
6. Présentation
7. Maintenance ou archivage

## Participer

Consulter les propositions et les dépôts liés.
Chaque projet doit indiquer ses objectifs, son responsable et la manière de contribuer.

## Proposer un projet

Ouvrir une Issue avec le modèle de proposition de projet.
```

### Modèle `project-template/README.md`

``` markdown
# [NOM DU PROJET]

## Présentation

[Décrire le problème et la solution envisagée.]

## Objectifs

- [Objectif 1]
- [Objectif 2]

## Fonctionnalités prévues

- [Fonctionnalité 1]
- [Fonctionnalité 2]

## Technologies

- [Technologie 1]
- [Technologie 2]

## Équipe

- Responsable : [Pseudo]
- Membres : [Pseudos]

## État

[Proposé / En préparation / En développement / Terminé / Archivé]

## Contribuer

Lire CONTRIBUTING.md et consulter les Issues ouvertes.

## Installation

[Instructions à compléter.]

## Documentation

[Liens utiles.]
```

### Règle pour les projets de grande taille

Un projet autonome peut recevoir son propre dépôt dans l'organisation.
Dans ce cas :

-   Le dépôt doit avoir un README.
-   Le dépôt doit avoir une licence adaptée.
-   Le dépôt doit avoir un guide de contribution.
-   Le responsable doit être identifié.
-   Les secrets doivent être stockés dans les secrets GitHub ou un
    gestionnaire adapté.
-   Les membres doivent savoir comment installer et tester le projet.

## 5.4 Repository `activities`

**Rôle :** mémoire et documentation des activités de la communauté.

### Arborescence

``` text
activities/
|
+-- README.md
+-- CONTRIBUTING.md
|
+-- templates/
|   +-- ACTIVITY_TEMPLATE.md
|   +-- REPORT_TEMPLATE.md
|
+-- challenges/
|   +-- README.md
|
+-- workshops/
|   +-- README.md
|
+-- tech-talks/
|   +-- README.md
|
+-- study-sessions/
|   +-- README.md
|
+-- hackathons/
|   +-- README.md
|
+-- events/
    +-- README.md
```

### Modèle `ACTIVITY_TEMPLATE.md`

``` markdown
# [NOM DE L'ACTIVITÉ]

- **Type :** [Challenge / Atelier / Tech talk / Révision / Hackathon]
- **Organisateur :** [Pseudo]
- **Date :** [Date et heure avec fuseau horaire]
- **Durée :** [Durée]
- **Format :** [Discord vocal / Présentiel / Hybride]
- **Niveau :** [Débutant / Intermédiaire / Avancé / Tous niveaux]
- **Inscription :** [Lien ou procédure]

## Objectifs

[Ce que les participants doivent apprendre ou réaliser.]

## Programme

1. [Étape 1]
2. [Étape 2]
3. [Étape 3]

## Prérequis

[Connaissances et outils nécessaires.]

## Matériel

[Liens, logiciels, supports.]

## Résultat attendu

[Livrable ou résultat de l'activité.]

## Après l'activité

Le compte rendu et les ressources seront publiés dans ce dépôt.
```

### Modèle `REPORT_TEMPLATE.md`

``` markdown
# Compte rendu — [NOM DE L'ACTIVITÉ]

- Date :
- Organisateur :
- Participants (nombre, sans publier de données personnelles inutiles) :

## Résumé

[Résumé de l'activité.]

## Points abordés

- [Point 1]
- [Point 2]

## Ressources

- [Lien 1]
- [Lien 2]

## Résultats

[Ce qui a été réalisé ou appris.]

## Améliorations pour la prochaine fois

- [Amélioration 1]
```

## 5.5 Repository `community-bot` --- phase ultérieure

Ne pas créer ce dépôt comme une priorité du lancement. Le créer lorsque
l'équipe décide réellement de développer son propre bot.

Arborescence indicative :

``` text
community-bot/
|
+-- README.md
+-- CONTRIBUTING.md
+-- SECURITY.md
+-- .env.example
+-- .gitignore
+-- src/
|   +-- commands/
|   +-- events/
|   +-- services/
|   +-- integrations/
|   +-- config/
|
+-- tests/
+-- docs/
+-- .github/
    +-- workflows/
```

Fonctions envisagées :

  Commande        Fonction
  --------------- --------------------------------------------
  `/help`         Présenter les commandes
  `/resource`     Rechercher dans le catalogue de ressources
  `/activity`     Afficher les prochaines activités
  `/propose`      Proposer une activité
  `/project`      Afficher les projets
  `/contribute`   Expliquer comment contribuer

Ne pas développer ces commandes avant d'avoir défini les sources de
données, les permissions et les cas d'erreur.

## 5.6 Repository `community-website` --- phase future

À étudier uniquement après validation des besoins.

Fonctions possibles : - Présentation publique. - Catalogue de ressources
consultable. - Répertoire des projets. - Calendrier des activités. -
Liens vers Discord et GitHub. - Statistiques publiques non sensibles.

Ne pas créer un compte utilisateur ou une base de données de membres si
les besoins ne le justifient pas.

------------------------------------------------------------------------

# 6. Standards GitHub communs

## 6.1 Nommage des dépôts

-   Utiliser des noms en minuscules.
-   Séparer les mots par des tirets.
-   Éviter les abréviations difficiles à comprendre.
-   Utiliser un nom qui décrit la fonction du dépôt.

Exemples : `resources`, `community-handbook`, `community-projects`.

## 6.2 Branches

Convention recommandée :

-   `main` : version principale.
-   `docs/nom-du-sujet` : documentation.
-   `feat/nom-fonctionnalite` : fonctionnalité.
-   `fix/nom-correction` : correction.
-   `chore/nom-tache` : maintenance.

Les branches temporaires sont fusionnées puis supprimées après
validation.

## 6.3 Commits

Convention simple :

``` text
docs: add contribution guide
feat: add resource template
fix: correct broken resource link
chore: reorganize resource folders
```

Préfixes : - `feat` : nouvelle fonctionnalité ou contenu structurant. -
`fix` : correction. - `docs` : documentation. - `chore` : maintenance. -
`refactor` : réorganisation sans changement fonctionnel majeur. - `test`
: tests.

## 6.4 Pull Requests

Chaque Pull Request doit : - Avoir un titre compréhensible. - Expliquer
le changement. - Référencer l'Issue liée, si elle existe. - Indiquer les
tests ou vérifications réalisés. - Signaler les impacts sur les autres
dossiers. - Être relue par une personne autre que l'auteur lorsque cela
est possible.

### Modèle `.github/PULL_REQUEST_TEMPLATE.md`

``` markdown
## Description

[Décrire les changements.]

## Type de changement

- [ ] Nouvelle ressource
- [ ] Nouvelle documentation
- [ ] Correction
- [ ] Nouvelle fonctionnalité
- [ ] Réorganisation

## Issue liée

Closes #[NUMERO]

## Vérifications

- [ ] Les liens ont été testés.
- [ ] Les informations sont exactes autant que possible.
- [ ] Les règles de contribution sont respectées.
- [ ] Aucun secret ou renseignement privé n'a été ajouté.
- [ ] Les licences et droits d'auteur ont été pris en compte.

## Informations complémentaires

[Ajouter les précisions utiles.]
```

## 6.5 Labels communs

Créer progressivement ces labels dans les dépôts concernés :

  Label                   Couleur indicative   Utilisation
  ----------------------- -------------------- --------------------------------
  `good first issue`      Vert                 Tâche accessible aux débutants
  `help wanted`           Vert                 Besoin de contributeurs
  `documentation`         Bleu                 Documentation
  `bug`                   Rouge                Problème à corriger
  `enhancement`           Violet               Amélioration
  `question`              Jaune                Question
  `resource`              Bleu                 Proposition de ressource
  `activity`              Orange               Activité
  `project`               Violet               Projet
  `priority: high`        Rouge                Priorité élevée
  `priority: medium`      Orange               Priorité moyenne
  `priority: low`         Gris                 Priorité faible
  `status: triage`        Gris                 À examiner
  `status: in progress`   Bleu                 En cours
  `status: blocked`       Rouge                Bloqué

Les labels sont des outils de classement, pas une garantie de délai.

## 6.6 Issues à créer

Prévoir les types suivants :

1.  Proposition de ressource.
2.  Signalement d'un lien cassé.
3.  Proposition d'activité.
4.  Proposition de projet.
5.  Amélioration documentaire.
6.  Problème technique.
7.  Tâche de maintenance.

### Exemple de modèle d'Issue : proposition de ressource

``` markdown
---
name: Proposer une ressource
about: Ajouter une ressource utile à la communauté
title: "[RESOURCE] "
labels: resource, status: triage
---

## Nom de la ressource

## Lien

## Catégorie

## Type

## Niveau

## Langue

## Description

## Pourquoi cette ressource est-elle utile ?

## Licence ou conditions d'utilisation connues

## Vérification du lien

- [ ] Le lien fonctionne.
- [ ] La source est identifiée.
- [ ] La ressource est correctement décrite.
- [ ] Les droits d'utilisation ont été examinés.
```

------------------------------------------------------------------------

# 7. GitHub Projects : gestion du travail

Créer un GitHub Project d'organisation nommé :

`Community Operations`

## 7.1 Vues recommandées

-   **Board --- À faire / En cours / Terminé :** vue principale des
    tâches.
-   **Table --- Toutes les tâches :** responsable, priorité, dépôt,
    échéance.
-   **Roadmap --- Grandes phases :** suivi du déploiement et des
    évolutions.

## 7.2 Champs

  -----------------------------------------------------------------------
  Champ                   Type                    Valeurs
  ----------------------- ----------------------- -----------------------
  Status                  Single select           Backlog, Todo, In
                                                  progress, In review,
                                                  Done, Blocked

  Priority                Single select           High, Medium, Low

  Area                    Single select           GitHub, Discord,
                                                  Resources, Projects,
                                                  Activities, Governance

  Assignee                Person                  Responsable

  Due date                Date                    Échéance

  Phase                   Single select           Setup, Launch, Growth,
                                                  Future
  -----------------------------------------------------------------------

## 7.3 Règles d'utilisation

-   Une tâche importante doit avoir une Issue.
-   Une tâche en cours doit avoir un responsable.
-   Une tâche bloquée doit expliquer le blocage.
-   Une tâche terminée doit satisfaire ses critères d'acceptation.
-   Les responsables mettent à jour les tâches au moins lors des points
    de coordination.

------------------------------------------------------------------------

# 8. Discord : architecture complète

## 8.1 Principes

Discord est le lieu de discussion et d'animation. Les documents de
référence, les ressources et les livrables durables sont conservés sur
GitHub.

Ne pas créer trop de salons dès le début. Les salons peu actifs peuvent
être ajoutés plus tard.

## 8.2 Catégories et salons

### Catégorie 1 --- `00・ACCUEIL`

  -----------------------------------------------------------------------
  Salon                   Type                    Permission
  ----------------------- ----------------------- -----------------------
  `bienvenue`             Texte                   Lecture pour tous ;
                                                  messages limités ou
                                                  désactivés

  `reglement`             Texte                   Lecture pour tous ;
                                                  écriture limitée

  `annonces`              Texte                   Lecture pour tous ;
                                                  publication
                                                  responsables

  `presentations`         Texte                   Membres peuvent écrire

  `comment-participer`    Texte                   Lecture pour tous ;
                                                  publication limitée
  -----------------------------------------------------------------------

### Catégorie 2 --- `01・COMMUNAUTE`

  Salon                    Type    Utilisation
  ------------------------ ------- ---------------------------------
  `general`                Texte   Discussions générales
  `entraide`               Texte   Questions et aide
  `discussions-tech`       Texte   Débats et actualités techniques
  `idees-et-suggestions`   Texte   Propositions ouvertes
  `showcase`               Texte   Présentation des réalisations

### Catégorie 3 --- `02・RESSOURCES`

  Salon                     Type    Utilisation
  ------------------------- ------- ----------------------------------
  `partage-de-ressources`   Texte   Cours, tutoriels, documentations
  `outils-et-logiciels`     Texte   Logiciels et outils
  `plugins-et-extensions`   Texte   Extensions et plugins
  `sites-et-plateformes`    Texte   Sites et plateformes utiles
  `github-updates`          Texte   Notifications GitHub filtrées

### Catégorie 4 --- `03・APPRENTISSAGE`

  Salon                Type    Utilisation
  -------------------- ------- -----------------------------------
  `programmation`      Texte   Langages et algorithmique
  `web-dev`            Texte   Développement web
  `mobile-dev`         Texte   Développement mobile
  `cybersecurite`      Texte   Sécurité informatique responsable
  `ia-et-data`         Texte   IA, machine learning et données
  `devops-cloud`       Texte   Linux, cloud, conteneurs et CI/CD
  `bases-de-donnees`   Texte   SQL, NoSQL et modélisation

### Catégorie 5 --- `04・ACTIVITES`

  Salon                      Type                  Utilisation
  -------------------------- --------------------- -----------------------------
  `calendrier`               Texte ou événements   Programme des activités
  `challenges`               Texte                 Défis et exercices
  `ateliers`                 Texte                 Formations pratiques
  `hackathons`               Texte                 Organisation des hackathons
  `projets-communautaires`   Texte                 Coordination des projets
  `propositions-activites`   Texte                 Idées ouvertes

### Catégorie 6 --- `05・VOCAL`

  Salon                      Type    Utilisation
  -------------------------- ------- ----------------------------------
  `General`                  Vocal   Discussion libre
  `Salle-de-travail`         Vocal   Travail silencieux ou accompagné
  `Pair-programming`         Vocal   Programmation en binôme
  `Ateliers-et-formations`   Vocal   Sessions encadrées
  `Reunions-organisateurs`   Vocal   Coordination des responsables

### Catégorie 7 --- `06・EQUIPE` (accès restreint)

  Salon                      Type    Accès
  -------------------------- ------- --------------------------------------
  `coordination`             Texte   Fondateurs et responsables autorisés
  `moderation`               Texte   Modérateurs et administrateurs
  `organisation-activites`   Texte   Responsables d'activités
  `maintenance-github`       Texte   Mainteneurs
  `reunions-equipe`          Vocal   Membres de l'équipe autorisés

Les discussions privées de modération ne doivent pas servir à exposer
publiquement les données personnelles ou les signalements des membres.

## 8.3 Rôles Discord

Créer les rôles dans cet ordre indicatif :

1.  `Fondateur`
2.  `Administrateur`
3.  `Modérateur`
4.  `Responsable d'activité`
5.  `Mainteneur`
6.  `Responsable de domaine`
7.  `Mentor`
8.  `Contributeur`
9.  `Membre`
10. `Nouveau membre`, si nécessaire
11. Rôles de domaines facultatifs : `Python`, `Web`, `Cybersecurity`,
    `AI & Data`, `DevOps`, etc.

Les rôles de domaine servent à identifier les centres d'intérêt et ne
donnent pas de permissions d'administration.

## 8.4 Permissions Discord

-   `@everyone` : accès limité aux salons d'accueil.
-   `Nouveau membre` : accès aux présentations et salons de démarrage.
-   `Membre` : accès aux salons communautaires.
-   `Contributeur` : rôle de reconnaissance ; pas de privilège global
    automatique.
-   `Mentor` : rôle de reconnaissance ; pas de privilège global
    automatique.
-   `Responsable d'activité` : publication dans les salons d'activités
    selon le besoin.
-   `Mainteneur` : accès au salon de coordination GitHub.
-   `Modérateur` : permissions de modération nécessaires.
-   `Administrateur` : administration du serveur selon les
    responsabilités.
-   `Fondateur` : gestion complète réservée aux personnes
    indispensables.

### Sécurité Discord

-   Activer le niveau de vérification adapté au serveur.
-   Activer les protections anti-spam disponibles.
-   Limiter les invitations et intégrations aux responsables autorisés.
-   Vérifier les permissions des bots.
-   Ne pas accorder `Administrator` à un bot sans nécessité démontrée.
-   Prévoir une procédure de signalement.
-   Ne jamais demander de mot de passe ou de clé API dans un salon.
-   Utiliser les salons privés uniquement pour les besoins légitimes de
    coordination.

## 8.5 Messages prêts à publier

### Message `#bienvenue`

``` text
Bienvenue sur [NOM_COMMUNAUTE] !

Nous sommes une communauté d'étudiants et passionnés d'informatique.
Notre objectif est d'apprendre ensemble, partager des ressources,
réaliser des projets et organiser des activités techniques.

Pour commencer :
1. Lis le règlement.
2. Présente-toi dans #presentations.
3. Consulte #comment-participer.
4. Découvre notre organisation GitHub : [LIEN_GITHUB].
5. Participe aux discussions et propose tes idées.

Tu peux contribuer quel que soit ton niveau.
Bienvenue parmi nous !
```

### Message `#reglement`

``` text
RÈGLEMENT DE LA COMMUNAUTÉ

1. Respecter tous les membres.
2. Ne pas harceler, discriminer, menacer ou insulter.
3. Éviter le spam et la publicité non autorisée.
4. Publier dans les salons appropriés.
5. Respecter les droits d'auteur et les licences.
6. Ne jamais partager de données personnelles ou de secrets.
7. Ne pas diffuser de logiciels malveillants ou de contenus dangereux.
8. Accepter les désaccords techniques avec respect.
9. Respecter les décisions de modération et utiliser les voies de recours.
10. Contribuer à maintenir un environnement accueillant.

Les signalements peuvent être adressés à l'équipe de modération.
```

### Message `#comment-participer`

``` text
COMMENT PARTICIPER ?

Partager une ressource :
- Présente-la dans #partage-de-ressources.
- Propose son ajout sur GitHub : [LIEN_RESOURCES].

Proposer une activité :
- Décris ton idée dans #propositions-activites.
- Un responsable peut t'aider à la mettre en place.

Participer à un projet :
- Consulte [LIEN_PROJECTS].
- Rejoins une équipe ou propose ton aide.

Contribuer à la documentation :
- Consulte le guide CONTRIBUTING du dépôt concerné.
- Ouvre une Issue ou une Pull Request.

Tu n'as pas besoin d'être administrateur pour contribuer.
```

------------------------------------------------------------------------

# 9. Processus communautaires

## 9.1 Processus de proposition d'une ressource

``` text
Membre découvre une ressource
          |
          v
Partage le lien dans Discord ou ouvre une Issue
          |
          v
Un mainteneur vérifie le lien et les informations
          |
          v
Le contributeur ou le mainteneur prépare la fiche
          |
          v
Pull Request
          |
          v
Relecture et validation
          |
          v
Fusion dans resources
          |
          v
Annonce dans Discord si pertinent
```

Critères de validation : - Lien fonctionnel. - Source identifiable. -
Description utile. - Catégorie correcte. - Niveau et langue renseignés
lorsque pertinents. - Respect des droits d'auteur. - Absence de secret
ou donnée privée.

## 9.2 Processus de proposition d'activité

``` text
Membre propose une idée
          |
          v
Discussion et intérêt des participants
          |
          v
Un organisateur volontaire se manifeste
          |
          v
Objectifs, date, format et programme définis
          |
          v
Validation logistique par le responsable concerné
          |
          v
Annonce et inscriptions
          |
          v
Réalisation
          |
          v
Compte rendu et ressources sur GitHub
```

Un membre peut proposer et organiser une activité. L'équipe de
coordination intervient pour aider, éviter les conflits de calendrier et
vérifier les besoins logistiques.

## 9.3 Processus de proposition de projet

1.  Le membre ouvre une Issue de proposition.
2.  La communauté discute du besoin.
3.  Un responsable volontaire est identifié.
4.  Le périmètre minimum est défini.
5.  Les tâches sont créées.
6.  Les contributeurs rejoignent le projet.
7.  Le développement est suivi sur GitHub.
8.  Le résultat est présenté.
9.  La documentation est complétée.
10. Le projet est maintenu ou archivé.

## 9.4 Processus de modération

1.  Recevoir un signalement.
2.  Vérifier les faits sans tirer de conclusion hâtive.
3.  Prendre une mesure proportionnée si nécessaire.
4.  Conserver uniquement les informations nécessaires.
5.  Informer les personnes concernées dans la mesure appropriée.
6.  Escalader les incidents graves aux administrateurs.
7.  Prévoir un recours ou une demande de réexamen.
8.  Documenter la procédure sans exposer publiquement les personnes.

Mesures possibles selon la gravité : - Rappel des règles. - Demande de
correction. - Suppression d'un contenu problématique. - Avertissement. -
Restriction temporaire. - Exclusion en dernier recours ou en cas de
gravité particulière.

------------------------------------------------------------------------

# 10. Activités : programme initial

## 10.1 Formats

  Activité               Fréquence indicative        Livrable
  ---------------------- --------------------------- ----------------------------
  Coding Challenge       Hebdomadaire ou bimensuel   Énoncé et solutions
  Tech Workshop          Mensuel                     Support et exercices
  Tech Talk              Mensuel                     Présentation et ressources
  Study Session          Selon calendrier            Notes et exercices
  Projet communautaire   Continu                     Application ou prototype
  Hackathon              Occasionnel                 Démonstration et bilan

La fréquence doit être adaptée à la disponibilité réelle des étudiants.

## 10.2 Premier mois de lancement

### Semaine 1

-   Présentation de la communauté.
-   Accueil des premiers membres.
-   Présentation de GitHub et Discord.
-   Recueil des domaines d'intérêt.

### Semaine 2

-   Premier partage de ressources.
-   Premier challenge simple.
-   Atelier pratique Git et GitHub.

### Semaine 3

-   Premier Tech Talk.
-   Proposition de projets collectifs.
-   Constitution de petites équipes.

### Semaine 4

-   Présentation des résultats.
-   Bilan des activités.
-   Recueil des retours.
-   Publication de la prochaine feuille de route.

------------------------------------------------------------------------

# 11. Intégrations et automatisations

## 11.1 Intégration GitHub vers Discord

Objectif : informer les membres des changements importants sans
transformer Discord en flux de notifications.

À faire : - Installer l'intégration officielle GitHub-Discord ou
l'application appropriée. - Sélectionner uniquement les dépôts utiles. -
Choisir un salon `#github-updates`. - Tester les notifications. -
Filtrer les événements non pertinents. - Vérifier les permissions
accordées à l'application.

Événements potentiellement utiles : - Nouvelles Issues. - Pull Requests
ouvertes ou fusionnées. - Releases. - Discussions importantes, si
l'intégration le permet.

Éviter de notifier chaque commit dans un salon visible de tous.

## 11.2 Bots Discord

Évaluer les besoins avant d'installer un bot.

  Besoin       Solution à étudier
  ------------ -----------------------------------------
  Modération   Carl-bot, Dyno ou outils natifs Discord
  Événements   Sesh ou événements natifs Discord
  GitHub       Intégration officielle GitHub-Discord
  Rôles        Outils natifs ou bot de rôles vérifié

Avant installation : - Vérifier l'identité et la réputation du bot. -
Examiner les permissions demandées. - Limiter les accès aux salons
nécessaires. - Lire la politique de confidentialité. - Tester dans un
environnement limité. - Désinstaller les bots inutilisés.

## 11.3 Futur bot communautaire

Ne développer le bot qu'après avoir identifié des besoins réels et
répétitifs.

Technologies possibles : - Python et `discord.py`. -
JavaScript/TypeScript et `discord.js`.

Exigences : - Code versionné sur GitHub. - Fichier `.env.example` sans
valeur secrète. - Secrets conservés hors du dépôt. - Tests des
commandes. - Gestion des erreurs. - Permissions minimales. -
Documentation d'installation. - Procédure de redémarrage et de
maintenance. - Responsable technique identifié.

------------------------------------------------------------------------

# 12. Sécurité, confidentialité et licences

## 12.1 Secrets

Ne jamais publier : - Tokens Discord. - Clés API. - Mots de passe. -
Clés privées. - Fichiers `.env` réels. - Informations d'accès à des
services.

Utiliser : - GitHub Actions Secrets pour les workflows. - Variables
d'environnement pour les applications. - Un gestionnaire de secrets
adapté lorsque le projet grandit.

Ajouter `.env` au `.gitignore` et ne versionner qu'un `.env.example`
sans secret.

## 12.2 Données personnelles

-   Ne collecter que les données réellement nécessaires.
-   Ne pas publier les coordonnées personnelles des membres sans accord.
-   Ne pas publier de listes privées de participants.
-   Ne pas conserver indéfiniment les signalements de modération.
-   Limiter l'accès aux espaces privés.
-   Informer les membres de l'utilisation des informations collectées.

## 12.3 Ressources et droits d'auteur

-   Préférer les liens vers les sources officielles.
-   Respecter les licences des logiciels et contenus.
-   Ne pas héberger de copies piratées de livres, cours ou logiciels.
-   Ne pas présenter une ressource comme libre si sa licence n'est pas
    connue.
-   Ajouter les attributions requises.
-   Retirer ou corriger les contenus signalés comme illicites après
    vérification.

## 12.4 Licences des dépôts

Choisir une licence en fonction du contenu : - Code : licence logicielle
choisie explicitement par les responsables du projet. - Documentation :
licence adaptée à la documentation. - Ressources externes : conserver la
licence de leur auteur et pointer vers la source.

Ne pas ajouter automatiquement une licence unique à des contenus dont la
communauté ne possède pas les droits.

------------------------------------------------------------------------

# 13. Documentation et continuité

Chaque responsable doit documenter : - Ce qu'il gère. - Les opérations
régulières. - Les accès nécessaires, sans publier les secrets. - Les
incidents connus. - Les procédures de remplacement. - Les décisions
importantes.

Prévoir : - Une réunion de coordination périodique. - Un bilan mensuel
léger. - Une revue des rôles tous les trois mois. - Une passation
lorsqu'un responsable quitte son rôle. - Une sauvegarde ou export des
informations critiques lorsque cela est nécessaire et possible.

------------------------------------------------------------------------

# 14. Plan de déploiement et critères d'acceptation

## Phase 0 --- Préparation

-   [ ] Nom et mission validés.
-   [ ] Fondateurs identifiés.
-   [ ] Périmètre du lancement défini.
-   [ ] Adresse de contact choisie.
-   [ ] Responsable du déploiement nommé.

**Acceptation :** les fondateurs approuvent la mission, le nom et le
périmètre.

## Phase 1 --- Fondation GitHub

-   [ ] Organisation créée.
-   [ ] Profil renseigné.
-   [ ] Sécurité configurée.
-   [ ] Owners limités.
-   [ ] Équipes créées.
-   [ ] Permissions testées.

**Acceptation :** l'organisation est accessible aux responsables et les
permissions correspondent à la matrice.

## Phase 2 --- Dépôts et documentation

-   [ ] `community-handbook` créé.
-   [ ] `resources` créé.
-   [ ] `community-projects` créé.
-   [ ] `activities` créé.
-   [ ] README de chaque dépôt ajouté.
-   [ ] Modèles et guides ajoutés.
-   [ ] Licences examinées.
-   [ ] Arborescences validées.

**Acceptation :** chaque dépôt explique son utilité et la façon de
contribuer.

## Phase 3 --- Collaboration GitHub

-   [ ] Labels créés.
-   [ ] Modèles d'Issues créés.
-   [ ] Modèle de Pull Request créé.
-   [ ] Branches principales protégées lorsque possible.
-   [ ] Processus de revue testé.
-   [ ] GitHub Project créé.
-   [ ] Une contribution test a été fusionnée.

**Acceptation :** une personne sans droit d'administration peut proposer
une contribution et suivre son traitement.

## Phase 4 --- Discord

-   [ ] Serveur créé.
-   [ ] Catégories créées.
-   [ ] Salons créés.
-   [ ] Rôles créés.
-   [ ] Permissions configurées.
-   [ ] Messages d'accueil publiés.
-   [ ] Procédure de modération définie.
-   [ ] Test réalisé avec un compte membre standard.

**Acceptation :** un nouveau membre peut rejoindre le serveur,
comprendre son fonctionnement et participer aux salons autorisés.

## Phase 5 --- Intégration

-   [ ] Intégration GitHub-Discord installée.
-   [ ] Dépôts autorisés sélectionnés.
-   [ ] Notifications configurées.
-   [ ] Tests d'Issues et de Pull Requests réalisés.
-   [ ] Notifications excessives filtrées.

**Acceptation :** les événements importants sont visibles dans le bon
salon sans divulgation de données sensibles.

## Phase 6 --- Contenu et lancement

-   [ ] Ressources initiales ajoutées.
-   [ ] Première activité préparée.
-   [ ] Premier challenge ou atelier planifié.
-   [ ] Message de lancement préparé.
-   [ ] Liens officiels vérifiés.
-   [ ] Équipe de modération disponible.
-   [ ] Retours des premiers membres recueillis.

**Acceptation :** la communauté peut accueillir ses premiers membres et
organiser sa première activité.

## Phase 7 --- Amélioration

-   [ ] Bilan du premier mois réalisé.
-   [ ] Indicateurs examinés.
-   [ ] Salons inutiles identifiés.
-   [ ] Besoins d'automatisation évalués.
-   [ ] Prochaine feuille de route publiée.

**Acceptation :** les responsables disposent d'une liste priorisée
d'améliorations.

------------------------------------------------------------------------

# 15. Indicateurs de suivi

Suivre des indicateurs simples, sans transformer la participation en
compétition.

  Indicateur                   Ce qu'il mesure
  ---------------------------- ------------------------------------------
  Membres actifs               Participation réelle à la communauté
  Ressources vérifiées         Qualité et croissance de la bibliothèque
  Pull Requests fusionnées     Contributions acceptées
  Issues traitées              Capacité à répondre aux propositions
  Projets actifs               Collaboration technique
  Activités réalisées          Animation de la communauté
  Participants aux activités   Intérêt et accessibilité
  Retours des membres          Satisfaction et améliorations

Ne pas évaluer un membre uniquement au nombre de messages, commits ou
contributions.

------------------------------------------------------------------------

# 16. Décisions à faire valider par les fondateurs

Ces éléments ne doivent pas être inventés par l'équipe technique.

-   [ ] Nom définitif.
-   [ ] Logo et identité visuelle.
-   [ ] Public cible et périmètre géographique.
-   [ ] Adresse de contact.
-   [ ] Fondateurs et Owners.
-   [ ] Liste des administrateurs.
-   [ ] Personnes responsables des dépôts.
-   [ ] Règles d'adhésion.
-   [ ] Règles de modération et recours.
-   [ ] Licence des contenus originaux de la communauté.
-   [ ] Fréquence des activités.
-   [ ] Conditions d'ouverture des projets.
-   [ ] Budget éventuel et outils payants.
-   [ ] Politique de conservation des données.

------------------------------------------------------------------------

# 17. Liste de livraison à remettre aux fondateurs

L'équipe chargée de l'exécution doit remettre :

-   [ ] Lien de l'organisation GitHub.
-   [ ] Liste des propriétaires et responsables, communiquée de façon
    privée.
-   [ ] Liste des dépôts créés.
-   [ ] Liens vers les README et guides.
-   [ ] Arborescences finales des dépôts.
-   [ ] Liste des équipes et permissions.
-   [ ] Lien du GitHub Project.
-   [ ] Lien d'invitation Discord.
-   [ ] Liste des catégories et salons.
-   [ ] Liste des rôles Discord et permissions.
-   [ ] Liste des bots et intégrations installés.
-   [ ] Résultat des tests de contribution.
-   [ ] Résultat des tests d'intégration.
-   [ ] Liste des tâches restantes.
-   [ ] Documentation de passation.

Les mots de passe, tokens et secrets ne doivent jamais être remis dans
ce document ou dans une Issue. Les accès doivent être gérés par les
mécanismes sécurisés des plateformes.

------------------------------------------------------------------------

# 18. Ordre d'exécution obligatoire recommandé

Pour éviter de disperser l'équipe, suivre cet ordre :

1.  Valider la mission, le nom et les fondateurs.
2.  Créer et sécuriser l'organisation GitHub.
3.  Créer `community-handbook`.
4.  Créer `resources`.
5.  Créer `community-projects`.
6.  Créer `activities`.
7.  Ajouter les README, guides et modèles.
8.  Configurer les rôles et permissions GitHub.
9.  Configurer Issues, Pull Requests, labels et Projects.
10. Tester une contribution réelle.
11. Créer et configurer Discord.
12. Tester Discord avec un membre standard.
13. Relier GitHub et Discord.
14. Ajouter les premières ressources.
15. Préparer et réaliser la première activité.
16. Lancer officiellement la communauté.
17. Faire le bilan et prioriser les évolutions.

**Ne pas commencer par le bot ou le site web.** Le premier objectif est
d'obtenir une communauté qui fonctionne réellement avec GitHub et
Discord.

------------------------------------------------------------------------

# 19. Définition finale de réussite

Le déploiement initial est considéré comme réussi lorsque :

1.  L'organisation GitHub est créée et sécurisée.
2.  Les quatre dépôts essentiels sont disponibles et documentés.
3.  Les rôles et permissions sont compris par l'équipe.
4.  Un membre standard peut proposer une ressource sans droit
    d'administration.
5.  Un mainteneur peut examiner et accepter une contribution.
6.  Un membre peut proposer une activité.
7.  Un responsable volontaire peut organiser cette activité.
8.  Les informations durables sont archivées sur GitHub.
9.  Discord est organisé, accueillant et modéré.
10. Les notifications GitHub utiles arrivent dans Discord.
11. Une première activité a été réalisée et documentée.
12. Une autre personne peut reprendre les opérations grâce à la
    documentation.

------------------------------------------------------------------------

**Fin du cahier des charges maître.**

Ce document doit évoluer avec la communauté. Toute modification
importante de l'architecture, des rôles ou des règles doit être
discutée, validée et documentée dans le dépôt `community-handbook`.
