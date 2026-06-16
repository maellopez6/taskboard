# TaskBoard Lite

Mini application fournie pour le TP DevOps.

## Fonctionnalités

- afficher la liste des tâches
- ajouter une tâche
- vérifier l'état de l'API via `/health`

## Stack technique

- Frontend : HTML / CSS / JavaScript
- Backend : Node.js / Express
- Base de données : PostgreSQL

## Objectif du TP

Vous devez créer l'infrastructure de conteneurisation de cette application.

### À produire

- `frontend/Dockerfile`
- `backend/Dockerfile`
- `docker-compose.yml`

### Contraintes

- backend exécuté en non-root
- PostgreSQL avec volume nommé
- isolation réseau correcte
- base non exposée inutilement