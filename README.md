# Documentation de l'API ArgentBank

Ce document fournit des informations sur nos points de terminaison API tels que définis dans notre fichier Swagger.

[À propos de Swagger](https://swagger.io/)

## Authentification

La plupart de nos points de terminaison API nécessitent une authentification. Cela se fait en utilisant un token Bearer.

## Points de terminaison

### Module Utilisateur

#### POST /user/login

Utilisez ce point de terminaison pour vous connecter au système. Le corps de la requête doit inclure `username` et `password`.

#### POST /user/profile

Utilisez ce point de terminaison pour mettre à jour le profil de l'utilisateur. Le corps de la requête doit inclure les attributs de profil à mettre à jour.

### Module Compte

#### GET /user/accounts/{accountId}

Utilisez ce point de terminaison pour récupérer des informations sur un compte spécifique. Remplacez `{accountId}` par l'ID du compte que vous souhaitez récupérer.

#### DELETE /user/accounts/{accountId}

Utilisez ce point de terminaison pour supprimer un compte spécifique. Remplacez `{accountId}` par l'ID du compte que vous souhaitez supprimer.

#### GET /user/accounts/{accountId}/{transactionId}

Utilisez ce point de terminaison pour récupérer une transaction spécifique d'un compte donné. Remplacez `{accountId}` par l'ID du compte et `{transactionId}` par l'ID de la transaction que vous souhaitez récupérer.

#### PATCH /user/accounts/{accountId}/{transactionId}

Utilisez ce point de terminaison pour modifier ou supprimer des information pour une transaction spécifique d'un compte donné. Remplacez `{accountId}` par l'ID du compte et `{transactionId}` par l'ID de la transaction que vous souhaitez supprimer.

## Codes d'erreur

Notre API utilise des codes de statut HTTP standard pour indiquer le succès ou l'échec d'une requête API.

- 200: OK
- 400: Mauvaise requête
- 401: Non autorisé
- 404: Non trouvé
- 500: Erreur interne du serveur

Pour plus d'informations détaillées sur nos points de terminaison API, veuillez vous référer à notre fichier Swagger.

## Auteur

- [Raphael Sanchez](https://www.linkedin.com/in/raphael-sanchez-design/)
