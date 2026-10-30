# Parcours d'un projet

1. Le membre ouvre une Issue « Proposer un projet » dans [community-projects](https://github.com/Omada-for-eureka/community-projects).
2. La communauté discute du besoin.
3. Un responsable volontaire est identifié.
4. Le périmètre minimum est défini.
5. Les tâches sont créées (Issues).
6. Les contributeurs rejoignent le projet.
7. Le développement est suivi sur GitHub.
8. Le résultat est présenté (démo, `#showcase`).
9. La documentation est complétée.
10. Le projet est maintenu ou archivé.

## États d'un projet

| État | Dossier dans `community-projects` |
| --- | --- |
| Proposé | `proposals/` |
| En préparation / en développement | `active/` |
| Terminé | `completed/` |
| Archivé | `archived/` |

## Dépôt dédié

Un projet autonome peut recevoir son propre dépôt dans l'organisation lorsque sa taille, son équipe ou son cycle de livraison le justifie. Ce dépôt doit avoir :

- Un README (partir de `project-template/`).
- Une licence choisie explicitement.
- Un guide de contribution.
- Un responsable identifié.
- Des secrets stockés dans les secrets GitHub, jamais dans le code.
- Des instructions d'installation et de test.
