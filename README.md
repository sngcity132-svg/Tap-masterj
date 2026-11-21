# TAP MASTER — MVP 1.0

## Contenu
- `index.html` : jeu complet (3 mini-défis)
- `manifest.webmanifest` : installation PWA
- `sw.js` : cache hors connexion
- `icons/icon.svg` : icône

## Tester depuis Android
1. Téléchargez et décompressez le ZIP.
2. Importez le contenu du dossier `tap-master` dans un dépôt GitHub.
3. Dans GitHub : Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.
4. Attendez la publication, puis ouvrez l'adresse GitHub Pages dans Chrome Android.
5. Menu Chrome → « Installer l'application » ou « Ajouter à l'écran d'accueil ».

Alternative : déployer le dossier sur Netlify en utilisant l'option de déploiement manuel.

## Monétisation — étape suivante
Les blocs « ESPACE PUBLICITAIRE » sont des emplacements visuels uniquement : aucune publicité ne s'affiche encore et aucun revenu n'est généré à ce stade.
Pour le web, étudier Google AdSense selon l'éligibilité du site. Pour une application Android publiée sur Google Play, intégrer Google AdMob via une enveloppe Android adaptée et respecter les règles de consentement et de publicité.
Ne jamais cliquer sur ses propres annonces. Utiliser des annonces de test pendant le développement.

## Limites connues du MVP
- Les scores et records sont stockés localement sur l'appareil.
- Le classement n'est pas encore mondial : il nécessitera un serveur et une base de données.
- Le jeu est une PWA, pas encore un APK natif.
- Le mode Memory Flash est une manche courte de mémorisation.
