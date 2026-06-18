# build
FROM node:14

# définition du dossier de travail dans le container
WORKDIR /taskboard

# création d’un utilisateur non-root (sécurité)
RUN addgroup -S appgroup && adduser -S appuser -G appgroup

# copie des fichiers
COPY package*.json ./
RUN npm install

# copie uniquement des fichiers de dépendances
# permet de profiter du cache Docker si le code ne change pas
COPY . .

# attribution des droits
RUN chown -R appuser:appgroup /taskboard

# passage en non-root
USER appuser

# port de l'api exposé
EXPOSE 3000

CMD ["node", "src/app.js"]