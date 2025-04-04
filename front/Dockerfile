# Utilisation d'une image Node.js
FROM node:18

# Définir le répertoire de travail
WORKDIR /usr/src/app

# Copier les fichiers nécessaires pour installer les dépendances
COPY package*.json ./

# Installer les dépendances dans le conteneur
RUN npm install --legacy-peer-deps

# Copier le reste des fichiers (sans node_modules)
COPY . .

# Exposer le port Angular
EXPOSE 4200

# Commande pour démarrer l’application
CMD ["npm", "start"]
