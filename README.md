Todo List App - Synthèse du Projet

Ce projet est une application de gestion de tâches (Todo List) développée avec React (Frontend) et NestJS (Backend), utilisant une base de données MySQL et l’ORM Prisma pour la gestion des migrations.

📌 Objectif du Projet

L’application permet aux utilisateurs de :

Créer, modifier et supprimer des tâches,

Consulter la liste des tâches enregistrées,

Gérer les états des tâches en temps réel.

🛠️ Technologies Utilisées

Frontend : React (interfaces dynamiques, gestion d’état avec useState).

Backend : NestJS (architecture modulaire, API REST, gestion des routes et services).

Base de données : MySQL (gestion fiable des données avec Prisma).

Gestion des dépendances : Utilisation de Yarn pour une installation rapide et efficace.

🚀 Déploiement et Configuration

1️⃣ Installation des Dépendances

# Cloner le projet
git clone <URL-REPO>

# Installer les dépendances
cd backend && yarn install
cd ../frontend && yarn install

2️⃣ Configuration de la Base de Données

Configuration de MySQL en local ou via Docker :

docker run --name mysql-container -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql:5.7

Ajout des credentials dans le fichier .env du backend.

Migration Prisma :

cd backend
yarn prisma migrate dev

3️⃣ Lancement de l’Application

# Lancer le backend
yarn start

# Lancer le frontend
cd ../frontend
yarn start

✅ Fonctionnalités Implémentées

Backend (NestJS) :

Connexion MySQL via Prisma

Création et modification des tâches

Suppression des tâches (déjà implémentée dans l’API)

Frontend (React) :

Affichage des tâches récupérées depuis le backend

Ajout et modification des tâches via formulaire

Suppression des tâches en utilisant l’API existante

🔍 Défis Rencontrés et Solutions

Problème

Solution

Conflit de port 3000

Changer le port du frontend à 3001

Conflit de versions avec ESLint

Aligner les versions des dépendances

Erreurs de typage TypeScript

Définir précisément les types et ajuster le code

🎯 Perspectives d’Amélioration

Améliorer l’UI avec un design plus moderne.

Ajouter une gestion des utilisateurs pour un suivi personnalisé des tâches.

Mise en place d’un stockage distant avec un service cloud pour la persistance des données.

📩 Conclusion

Ce projet m’a permis de renforcer mes compétences en développement full-stack, en particulier dans l’intégration de React et NestJS, ainsi que dans la gestion des bases de données avec Prisma et MySQL. Les défis rencontrés ont été autant d’opportunités d’apprentissage, me permettant d’améliorer ma capacité à résoudre des problèmes complexes et à prendre des décisions techniques éclairées.
