# Optimisation des Dockerfiles avec multi-stage builds

## Objectif : 
- Apprendre à optimiser la taille des images Docker avec des multi-stage builds.
- Étapes à suivre Avec une application Python.

## Etape 1: Créer un Dockerfile standard pour builder cette application, puis s'assurer qu’elle fonctionne.
  - Créer un dossier my-python-app
  - Dans ce dossier, 
    - Créer un fichier app.py
    - Créer un fichier requirements.txt
    - Créer un fichier Dockerfile

## Etape 2: Optimiser le Dockerfile avec un multi-stage build
- Ecrire le nouveau Dockerfile

- Ensuite, optimiser ce Dockerfile avec un multi-stage build :
  - Première étape : Utilise une image lourde pour builder les dépendances.
  - Deuxième étape : Utilise une image légère (comme alpine) pour l’exécution finale de l’application.
- Comparer la taille des images Docker avant et après l'optimisation (docker image ls).