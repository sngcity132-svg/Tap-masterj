# TAP MASTER GLOBAL — Version 2.0

## Installation / mise à jour
Remplace les fichiers du dépôt GitHub par tous les fichiers de cette archive, en conservant la structure des dossiers. Le fichier `index.html` contient maintenant la connexion Supabase.

## Supabase
Le jeu utilise le Project URL et la clé publishable configurés dans `index.html`. Cette clé est publique et peut être présente dans le code client. Ne jamais y placer de clé `secret` ou `service_role`.

Le schéma SQL `profiles` et `scores` doit avoir été exécuté dans Supabase avant utilisation. Active le fournisseur Email dans Authentication → Sign In / Providers.

## Fonctionnalités ajoutées
- Inscription et connexion par email/mot de passe.
- Profil créé automatiquement par le trigger SQL.
- Enregistrement des scores des joueurs connectés.
- Classement par mode (20 résultats).

## Limites et sécurité
- Les scores sont soumis depuis le navigateur : ce MVP n'empêche pas la triche. Une validation serveur / Edge Function et des limites anti-abus sont nécessaires avant lancement public.
- Le classement est global mais affiche les meilleurs résultats soumis, pas un classement certifié.
- La confirmation email peut être requise selon les paramètres Auth du projet. Configure les URL autorisées dans Authentication → URL Configuration : ajoute l'URL GitHub Pages du jeu.
- Les publicités et paiements ne sont pas encore intégrés.
