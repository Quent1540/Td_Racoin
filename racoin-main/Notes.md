## Langages utilisés

CSS, PHP, SCSS, Javascript

## Frameworks utilisés

Twig, Slim

## But général de l'appli

publier/consulter des annonces

## Problèmes identifiés

- CSS pas dans le gitignore
- README pas écrit
- Beaucoup de code en commentaire
- Pas de config.ini
- Dockerfile dans un dossier php
- Pas de mysql en localhost
- Routes non sécurisées(N'importe qui peut accéder à config.ini)

## Estimation de ce qu'il faut pour faire marcher l'application

- Creer le config.ini
- rajouter un service mysql dans le docker compose

## Faire marcher l'application

- Installer/Mettre à jour les dépendances -> composer install
- Créer le fichier config.ini dans le dossier config et renseigner: driver, host, port, database, username, password, charset
- Lancer l'application: docker compouse up -d --build

## Trouver les dépendances non maintenues

- slim 2(fin de vie)
- illuminate/database 4.2
- twig 1.4
- symfony 4

## Améliorations à réaliser

- sécuriser les routes(mettre le fichier index et les images etc dans un dossier public), actuellement tout le projet est accessible en modifiant l'url T**emps: 2/10 **Impact**: 10/10**
- Changer la version de twig, passer directement à la version 3.x  **Temps: 4/10 **Impact**: 4/10**
- Changer la version de symfony(passer à la version 8.05)  **Temps: 5/10 **Impact**: 10/10**
- Changer la version de slim pour passer à la 4.15 en itérant **Temps: 4/10 Impact: 10/10**
- Ajouter le css dans le gitignore(sinon il est push sur git inutilement) **Temps: 1/10 Impact: 2/10**
