Docker Compose pour une application multi-service

Objectif : Utiliser Docker Compose pour orchestrer plusieurs services Docker ensemble.

Étapes :
1. Créer un projet qui contient une application web (pour une application Django) et une base de données PostgreSQL.
2. Écrire un fichier docker-compose.yml pour orchestrer les deux conteneurs (un pour Django et un pour PostgreSQL).
3. Configurer les réseaux Docker pour que les services puissent communiquer entre eux.
4. Lancer les services avec docker-compose up et vérifie que l’application fonctionne correctement.

Etape 1: 
1. Créer le projet
mkdir multi-service-app
cd multi-service-app


2. Créer l'application Django
mkdir django-app
cd django-app
django-admin startproject core .


3. Créer un Dockerfile pour Django
- Dans le répertoire django-app, crée un fichier Dockerfile.
- S'assurer d'avoir un fichier requirements.txt avec Django.

Etape 2: Écrire un fichier docker-compose.yml
A la racine du projet (multi-service-app), créer un fichier docker-compose.yml

Etape 3: Configurer les réseaux Docker
Docker Compose configure automatiquement un réseau pour les services définis dans le même fichier docker-compose.yml, donc pas besoin de configuration supplémentaire pour les réseaux.

Etape 4: Lancer les services
- Pour lancer les services, celà se fait avec la commande suivante :
docker-compose up

- Vérifier que l’application fonctionne. Pour celà il faut se rendre dans le navigateur et accéder à http://localhost:8000. A la page d’accueil devrait apparaitre le projet Django.




























