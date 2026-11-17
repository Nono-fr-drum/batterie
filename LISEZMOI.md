# Routine batterie : mise en ligne

## 1. Firebase (comptes + synchro du calendrier)
1. Va sur https://console.firebase.google.com, puis « Créer un projet » (Google Analytics inutile).
2. Dans le projet, ajoute une appli **Web** (icône `</>`) et copie l'objet `firebaseConfig`.
3. Colle ces valeurs dans `firebase-config.js` à la place de `A_REMPLIR`.
4. Va dans **Authentication**, puis « Commencer », active **Adresse e-mail/Mot de passe**.
5. Va dans **Firestore Database**, puis « Créer une base » (région europe-west), en mode production.
6. Dans l'onglet **Règles** de Firestore, colle le contenu de `firestore.rules` et publie.
7. Dans Authentication, va dans **Paramètres**, puis **Domaines autorisés**, et ajoute `TONPSEUDO.github.io`.

## 2. GitHub Pages (hébergement gratuit)
1. Crée un dépôt public, par exemple `batterie`, et mets-y tous les fichiers de ce dossier (il n y a aucun sous-dossier).
2. Va dans Settings, puis Pages, puis Source : « Deploy from a branch », branche `main`, dossier `/ (root)`.
3. L'appli est en ligne sur `https://TONPSEUDO.github.io/batterie/`.

## 3. Installer
- **PC (Edge ou Chrome)** : ouvre l'adresse, puis l'icône « Installer » dans la barre d'adresse. Tu obtiens un logiciel avec son icône (menu Démarrer, barre des tâches).
- **Android (Chrome)** : ouvre l'adresse, puis menu ⋮, puis « Installer l'application ».
- Après le premier lancement, l'appli marche hors connexion. Le calendrier se synchronise quand le réseau revient.
