# Serveur HTTP Simple en TypeScript

## Description
Ce projet est un serveur HTTP simple écrit en TypeScript. Il est conçu pour répondre uniquement aux requêtes GET à l'URL `/ping`. Lorsqu'une telle requête est reçue, le serveur renvoie les en-têtes de la requête sous forme de JSON. Pour toutes les autres URL ou méthodes, le serveur renvoie une erreur 404 (Not Found).

## Installation
Pour utiliser ce serveur, vous devez avoir Node.js installé sur votre machine. Si vous n'avez pas encore installé Node.js, vous pouvez le télécharger et l'installer à partir de [nodejs.org](https://nodejs.org/).

Une fois Node.js installé, clonez ce dépôt sur votre machine locale en utilisant la commande suivante :

`git clone https://github.com/Senchurion/tp-wik-dps-tp01-typescript`

## Utilisation
Pour démarrer le serveur, naviguez dans le répertoire du projet cloné et exécutez la commande suivante :

`npx tsc`

Puis ensuite lancer cette commande:

`node build/index.js`

Le serveur écoute par défaut sur le port 8080, mais vous pouvez définir un port différent en utilisant la variable d'environnement PING_LISTEN_PORT:

`export PING_LISTEN_PORT=x`

Une fois le serveur en cours d'exécution, vous pouvez tester la réponse /ping en utilisant un navigateur ou un outil de requête HTTP comme curl. Par exemple : 

`curl http://localhost:8080/ping -v`
