# Rôles et responsabilités

Les rôles Discord et GitHub sont deux systèmes différents. Avoir un rôle sur Discord ne donne pas automatiquement les mêmes permissions sur GitHub.

## Organigramme

```text
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

Cet organigramme représente des responsabilités, pas une hiérarchie de valeur entre les membres.

## Rôles

### Fondateur / Owner
- **Mission :** vision, administration de l'organisation GitHub, paramètres sensibles, désignation des responsables, continuité, arbitrage des décisions majeures.
- **Limites :** ne pas gérer seul toutes les activités ; ne pas bloquer les contributions légitimes ; documenter les décisions importantes.

### Administrateur communautaire
- **Mission :** coordination générale, suivi des responsables, réunions de coordination, respect des règles, incidents importants, feuille de route.
- **Permissions :** administration Discord selon le besoin ; pas de droit Owner GitHub automatique.

### Modérateur
- **Mission :** faire respecter les règles, accueillir et orienter, prévenir spam/harcèlement, traiter les signalements, escalader les incidents graves.
- **Permissions :** modération Discord ; aucun paramètre sensible GitHub.

### Mainteneur GitHub
- **Mission :** examiner Issues et Pull Requests, vérifier la qualité, maintenir l'organisation des dépôts, aider les contributeurs.
- **Permissions :** `Write` ou `Maintain` sur les dépôts concernés ; pas `Owner` par défaut.

### Responsable de domaine
Exemples : Python, web, cybersécurité, IA, DevOps.
- **Mission :** animer un domaine, identifier les ressources, proposer des ateliers, orienter les membres.
- **Permissions :** pas de droits globaux ; contribution aux dépôts concernés.

### Responsable d'activité
- **Mission :** transformer une proposition en activité réalisable, définir objectifs et programme, annoncer, gérer la séance, publier le compte rendu.
- **Permissions :** gestion du contenu de l'activité ; publication dans les salons autorisés.

### Mentor
- **Mission :** aider les membres à progresser, accompagner les débutants, proposer exercices et ressources.
- **Permissions :** accès aux espaces d'entraide ; pas de privilège technique automatique.

### Contributeur
- **Mission :** ajouter/corriger des ressources, contribuer au code et à la documentation, participer aux projets.
- **Permissions :** Issues, discussions, Pull Requests ; écriture uniquement si nécessaire.

### Membre
- **Mission :** participer, apprendre, partager, proposer des idées, signaler les problèmes.
- **Permissions :** lecture des ressources publiques, salons ouverts, Issues et contributions.

## Matrice de permissions

| Action | Owner | Admin Discord | Modérateur | Mainteneur | Resp. activité | Membre |
| --- | --- | --- | --- | --- | --- | --- |
| Paramètres de l'organisation GitHub | Oui | Non | Non | Non | Non | Non |
| Gérer les dépôts GitHub | Selon besoin | Non | Non | Dépôts attribués | Non | Non |
| Examiner les Pull Requests | Oui | Non | Non | Oui | Selon dépôt | Proposer |
| Gérer les salons Discord | Selon besoin | Oui | Selon besoin | Non | Salons attribués | Non |
| Modérer les messages | Selon besoin | Oui | Oui | Non | Non | Non |
| Proposer une activité | Oui | Oui | Oui | Oui | Oui | Oui |
| Organiser une activité | Oui | Oui | Oui | Oui | Oui | Oui, avec coordination |
| Proposer une ressource | Oui | Oui | Oui | Oui | Oui | Oui |
| Participer à un projet | Oui | Oui | Oui | Oui | Oui | Oui |

**Important :** ne pas donner de permission globale « administrateur » à chaque responsable. Uniquement les droits nécessaires à sa mission.

## Équipes GitHub

| Équipe | Membres | Accès |
| --- | --- | --- |
| `founders` | Fondateurs | Admin (Owners de l'organisation) |
| `maintainers` | Mainteneurs GitHub | `Maintain` sur les 4 dépôts |
| `resources-maintainers` | Mainteneurs de la bibliothèque | `Write` sur `resources` |
| `activity-leads` | Responsables d'activités | `Write` sur `activities` |
| `project-leads` | Responsables de projets | `Write` sur `community-projects` |

## Titulaires actuels

| Rôle | Titulaire | Remplaçant |
| --- | --- | --- |
| Fondateur / Owner | @TheSanctuaryDev | [À DÉFINIR] |
| Administrateur communautaire | [À DÉFINIR] | [À DÉFINIR] |
| Modération | [À DÉFINIR] | [À DÉFINIR] |
| Mainteneur `community-handbook` | [À DÉFINIR] | [À DÉFINIR] |
| Mainteneur `resources` | [À DÉFINIR] | [À DÉFINIR] |
| Mainteneur `community-projects` | [À DÉFINIR] | [À DÉFINIR] |
| Mainteneur `activities` | [À DÉFINIR] | [À DÉFINIR] |

## Nomination et renouvellement

- Toute responsabilité a une description et un titulaire.
- Les responsabilités peuvent être volontaires et cumulées.
- Les responsables documentent leur travail.
- Un remplaçant est prévu pour les tâches critiques.
- Les rôles sont réexaminés tous les trois mois.
