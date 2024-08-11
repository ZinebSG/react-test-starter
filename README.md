### Tester des Applications React

Ceci est le projet de démarrage pour le cours de test des applications React où vous apprendrez tout ce que vous devez savoir pour tester efficacement des applications React.

## À propos de ce Projet

Il s'agit d'une application React construite avec les technologies et bibliothèques suivantes :

- Auth0
- Tailwind
- RadixUI
- React Router
- React Query
- Redux Toolkit

Veuillez suivre attentivement ces instructions pour configurer ce projet sur votre machine.

## Configuration d'Auth0 pour l'Authentification

1. **Inscrivez-vous pour un compte Auth0 :**

   Si vous n'avez pas encore de compte Auth0, vous pouvez vous inscrire sur [https://auth0.com/](https://auth0.com/). Auth0 offre un plan gratuit que vous pouvez utiliser pour votre projet.

2. **Créer une Nouvelle Application :**

   - Connectez-vous à votre compte Auth0.
   - Allez sur le tableau de bord Auth0.
   - Cliquez sur "Applications" dans la barre latérale gauche.
   - Cliquez sur le bouton "Create Application".
   - Donnez un nom à votre application (par exemple, "Mon Application React").
   - Sélectionnez "Single Page Web Applications" comme type d'application.

3. **Configurer les Paramètres de l'Application :**

   - Sur la page des paramètres de l'application, configurez les paramètres suivants :
     - Allowed Callback URLs : `http://localhost:5173`
     - Allowed Logout URLs : `http://localhost:5173`
     - Allowed Web Origins : `http://localhost:5173`
   - Enregistrez les modifications.

4. **Obtenir le Domaine Auth0 et le Client ID :**

   - Sur la page des paramètres de l'application, vous trouverez votre domaine Auth0 et votre Client ID en haut de la page.
   - Copiez le domaine Auth0 (par exemple, `votre-domaine-auth0.auth0.com`) et le Client ID (par exemple, `votre-client-id`).

5. **Créer un fichier `.env.local` :**

   - Dans le répertoire racine du projet, vous trouverez un fichier `.env` exemple. Faites-en une copie et enregistrez-la sous le nom `.env.local`.
   - Remplacez le domaine Auth0 et le Client ID par les valeurs réelles que vous avez obtenues de Auth0.

## Exécuter l'Application

Maintenant que vous avez configuré Auth0 et configuré vos variables d'environnement, vous pouvez exécuter l'application React en utilisant les commandes suivantes :

```bash
# Installer les dépendances
npm install

# Démarrer le serveur de développement
npm start
```

Cela lancera le processus backend à `http://localhost:3000`. Si le port 3000 est déjà utilisé sur votre machine, mettez à jour le numéro de port dans les fichiers suivants et exécutez à nouveau `npm start` :

- json-server.json
- src/main.tsx