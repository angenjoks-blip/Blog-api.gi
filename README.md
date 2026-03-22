# Blog-api.gi - Projet INF222

## Présentation
Ce projet consiste en le développement d'une API REST pour la gestion d'un blog simple. Il permet de gérer des articles avec toutes les opérations CRUD (Create, Read, Update, Delete) et une fonction de recherche.

## Architecture Technique
- Environnement : Node.js
- Framework :Express.js
- Base de données : SQLite
- Documentation :Swagger 

## Fonctionnalités et Endpoints
L'API expose les routes suivantes :
- `POST /api/articles': Création d'un article (Titre, contenu, auteur, date, catégorie, tags).
- `GET /api/articles` : Récupération de la liste des articles (filtrable par catégorie ou auteur).
- `GET /api/articles/:id` : Lecture d'un article spécifique via son identifiant.
- `PUT /api/articles/:id` : Mise à jour d'un article existant.
- `DELETE /api/articles/:id` : Suppression définitive d'un article.
- `GET /api/articles/search?query=texte` : Recherche textuelle dans le titre ou le contenu.

## Installation
1. `npm install` (pour installer les dépendances Express et SQLite3).
2. `node server.js` (pour lancer le serveur sur le port 3000).

## Codes de statut HTTP
L'API utilise les codes standards pour la gestion des erreurs : 200 (OK), 201 (Création), 400 (Requête invalide), 404 (Non trouvé) et 500 (Erreur serveur).
