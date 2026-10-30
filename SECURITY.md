# Politique de sécurité

## Signaler une vulnérabilité ou un secret exposé

**Ne pas ouvrir d'Issue publique.**

Utiliser l'une de ces voies :

1. L'onglet **Security → Report a vulnerability** du dépôt concerné (signalement privé GitHub), lorsqu'il est activé.
2. Un message privé à un fondateur ou administrateur.
3. Un email à [EMAIL_CONTACT].

Indiquer : le dépôt, le fichier ou le service concerné, la nature du problème et, si possible, comment le reproduire.

## Secret publié par erreur

1. Prévenir immédiatement un responsable en privé.
2. **Révoquer ou régénérer le secret** auprès du service concerné : supprimer le fichier ne suffit pas, l'historique Git le conserve.
3. Nettoyer l'historique si nécessaire.
4. Documenter l'incident sans republier le secret.

## Règles permanentes

Ne jamais publier : tokens Discord, clés API, mots de passe, clés privées, fichiers `.env` réels, informations d'accès à des services.

Utiliser : GitHub Actions Secrets pour les workflows, variables d'environnement pour les applications, un `.env.example` sans valeur réelle.
