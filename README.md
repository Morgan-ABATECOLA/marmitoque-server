# marmitoque-server
API Server for marmitoque project  
  
# How use the project
This project is currently deployed using Heroku : https://marmitoque-server.herokuapp.com/  
(no current welcome page but you can try routes listed below)

# Ressources

Cooks (users)  
Recipes

# Routes 

GET     /recipes/id            Retourne la recette possédant l'id en fin d'url  
GET     /recipes               Retourne toutes les recettes  
POST    /recipes               Créer une recette. Besoin d'un JSON object avec name, description et creator_id (étant un ID valide de cook (User))  
PUT     /recipes/id            Met à jour une recette. Besoin d'un JSON object avec name, description et creator_id. L'id de l'URL étant une recette déjà    existante  
DELETE  /recipes/id            Supprime une recette. L'id de l' est un recette déjà existante  
GET     /recipes/of/user       Affiche toutes les recettes créées par un utilisateur. L'id de l'User connecté est passé en paramètre dans l'appelle.  
  
GET     /cooks/id              Affiche un User selon l'id passé en URL  
POST    /cooks                 Affiche tous les Users  
  
POST    /auth/login            Permet de se connecter  
GET     /auth/me               Permet d'obtenir les informations de la personne connectée  

