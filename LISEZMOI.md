# Kaddach Fatoura : générer l'APK avec GitHub

1. Dans ton dépôt GitHub, supprime les anciens fichiers à la racine (index.html, sw.js, manifest.webmanifest, icon-192.png, icon-512.png).
2. Envoie le contenu de ce dossier à la racine du dépôt : `www/`, `.github/`, `package.json`, `capacitor.config.json`, `.gitignore`.
   (Sur le site GitHub : Add file > Upload files. Le dossier `.github` est caché sur certains systèmes : glisse tout le dossier décompressé.)
3. Onglet **Actions** > « Construire l'APK Android » > **Run workflow**.
4. Attends 5 à 8 minutes, ouvre l'exécution terminée, section **Artifacts** : télécharge `kaddach-fatoura-apk`.
5. Décompresse le zip : tu obtiens `app-debug.apk`. Envoie-le sur le téléphone et installe-le (autorise « sources inconnues »).

Pour modifier l'application plus tard : change `www/index.html`, relance l'étape 3.
