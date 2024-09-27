# Étape 1 : construire l'application React
FROM node:16 as build

# Créer et positionner dans le répertoire de travail
WORKDIR /app

# Copier les fichiers de package et installer les dépendances
COPY package.json package-lock.json ./
RUN npm install

# Copier tout le code source dans le conteneur
COPY . .

# Construire l'application React
RUN npm run build

# Étape 2 : Servir l'application avec Nginx
FROM nginx:1.21-alpine

# Copier les fichiers de build générés par React vers le répertoire Nginx
COPY --from=build /app/build /usr/share/nginx/html

# Copier la configuration Nginx (optionnel si besoin de personnalisation)
# COPY nginx.conf /etc/nginx/nginx.conf

# Exposer le port 80
EXPOSE 80

# Démarrer Nginx
CMD ["nginx", "-g", "daemon off;"]
