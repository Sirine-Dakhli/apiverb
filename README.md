# apiverb
Application de Conjugaison de Verbes Français
Objectif
Cette application a été développée dans le cadre d'un projet de cours pour permettre aux utilisateurs d'interagir avec une API de verbes français, notamment pour récupérer des informations sur des verbes spécifiques et effectuer d'autres opérations sur les verbes (favoris, conjugaison, etc.). L'application utilise Angular pour le front-end et l'API pour gérer les données des verbes.

Fonctionnalités
Inscription et Connexion : Les utilisateurs peuvent s'inscrire et se connecter pour accéder à l'application.
Rechercher un verbe spécifique : Récupérez les informations détaillées sur un verbe spécifique via un point de terminaison de l'API.
Ajouter des verbes en favoris : Permet d'ajouter des verbes en favoris pour les retrouver facilement.
Obtenir des verbes aléatoires : Les utilisateurs peuvent également consulter des verbes aléatoires via un autre point de terminaison de l'API.
Technologies utilisées
Frontend : Angular, HTML, CSS
Backend API : L'API des Verbes Français (Node.js avec Express)
Autres technologies : JWT pour l'authentification, Bcrypt pour la sécurité des mots de passe
Installation
Clonez le dépôt :
bash
Copier le code
git clone <lien-du-repo>
Installez les dépendances :
bash
Copier le code
npm install
Lancer l'application :
bash
Copier le code
ng serve
Points de terminaison utilisés
Inscription et Connexion :

URL : https://french-verbs-fall-2023-app-ramym.ondigitalocean.app/v0/users/login
Méthode : POST
Headers : x-access-token
Body :
json
Copier le code
{
  "email": "votre-email",
  "password": "votre-mot-de-passe"
}
Récupération d'un verbe spécifique :

URL : https://french-verbs-fall-2023-app-ramym.ondigitalocean.app/v0/verbs/
Méthode : POST
Body :
json
Copier le code
{
  "verb": "habiter"
}
Verbes aléatoires :

URL : https://french-verbs-fall-2023-app-ramym.ondigitalocean.app/v0/verbs/random
Méthode : GET
Headers : x-access-token
Personnalisation
L'interface utilisateur a été adaptée pour offrir une expérience fluide et interactive aux utilisateurs. Vous pouvez modifier les fichiers src/app pour adapter les couleurs, les images, et les styles à vos besoins.
