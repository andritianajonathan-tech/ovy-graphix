OVY GRAPHIX — version corrigée (prototype local)

Fichiers :
- index.html : application
- manifest.json : configuration PWA
- sw.js : cache hors ligne de base
- icon-192.png / icon-512.png : icônes générées

Lancer le site :
1. Décompresse le ZIP dans un dossier.
2. Ouvre ce dossier dans VS Code.
3. Lance un serveur local avec Live Server, puis ouvre l'adresse localhost fournie.
   (Ne lance pas simplement index.html en file:// : Web Crypto et le service worker exigent un contexte sécurisé.)
4. Pour une mise en ligne, héberge tous les fichiers en HTTPS.

Limites importantes :
- Cette version est un prototype côté navigateur. Les données ne sont pas synchronisées entre utilisateurs ou appareils.
- L'adresse admin et les contrôles côté client ne constituent PAS une vraie sécurité. N'utilise pas ce prototype pour des comptes ou données sensibles.
- Pour un vrai concours partagé, il faut un backend, une base de données, une validation des fichiers côté serveur et des rôles contrôlés côté serveur.
- Le cache hors ligne est basique ; la première ouverture doit se faire avec une connexion.
