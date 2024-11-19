# COMMENCEMENT LE PROJET EST EN COURS DE CREATION🖤 **VibeFlicks** - Plateforme de recommandations de films basée sur l'humeur 🎬

## 🌟 **Description**  
VibeFlicks est une application web innovante qui recommande des films ou des séries en fonction de l'humeur de l'utilisateur. Grâce à une interface ludique et intuitive, l'utilisateur sélectionne son humeur et l'application lui propose des suggestions personnalisées. Une expérience unique pour chaque état d'esprit ! 🙌

## 🎯 **Fonctionnalités**  
- **Interface d'humeur** : Choisissez une humeur parmi des options visuelles, similaire à l’application "fruits".
- **Recommandations personnalisées** : Films et séries recommandés en fonction de l’humeur via l’API TMDb.
- **Filtres avancés** : Filtrez les films par genre, durée, auteur, ou date de parution.
- **Liste de favoris** : Ajoutez vos films préférés à une liste personnalisée.
- **Compte utilisateur** : Inscription et connexion obligatoire pour une expérience personnalisée.
- **Feedback pour améliorer les suggestions** : Un système de feedback pour affiner les recommandations (en fonction de l'utilisation).
- **Dons et soutien** : Possibilité de faire des dons via Paypal.

## 🛠️ **Technologies**  
- **Backend** : Symfony (API RESTful)
- **Frontend** : React JS + Vite + Bootstrap5
- **Base de données** : MySQL
- **Recommandations** : API TMDb (The Movie Database)
- **Dons** : API Paypal

## 🚀 **Installation**  

### Prérequis  
- **Docker** & **Docker Compose** (avec Docker Desktop)
- **Git** pour le clonage du projet

### Étapes d'installation

1. Clonez ce dépôt :
   
   git clone https://github.com/CorentinLartigue/VibeFlicks.git
   cd VibeFlicks/backend
   composer install
   cd ../
   
2. Lancez le projet avec Docker :

   docker-compose up --build


3. Accédez à l'application :

  Frontend React : http://localhost:3000
  Backend Symfony : http://localhost:8000

## 🧩 **Architecture & Design**

### **Pourquoi Symfony + React ?**
Ce projet combine **Symfony** pour le backend API et **React** pour le frontend afin de garantir une modularité maximale et une expérience utilisateur fluide.

- **Backend Symfony** : Gestion des données, de l’authentification, des requêtes API, et de la logique métier.
- **Frontend React** : Interface dynamique et réactive, avec une interaction fluide et rapide grâce à **Vite**.

### **Avantages de cette architecture**
- **Flexibilité** : Le backend et le frontend sont indépendants, ce qui permet une évolution sans perturber l’autre.
- **UX améliorée** : **React** permet de créer des interfaces riches et dynamiques pour une meilleure expérience.
- **Facilité de maintenance** : Chaque partie du projet peut être gérée séparément par des équipes spécialisées.

### **Défis**
- **Recommandations basées sur l’humeur** : La complexité réside dans la création de recommandations émotionnelles. **TMDb** ne fournit pas d’humeurs directes, ce qui nécessite de créer une logique d'association des films à des humeurs spécifiques.
- **Gestion des sessions et déconnexions** : La fonctionnalité de déconnexion automatique après une heure sans interaction peut poser un défi en termes d’ergonomie.

### 💡 **Réalisation**
- **Maquette** : Création d'une interface graphique sous **Figma**.
- **Développement backend** : Création d'une API **Symfony** pour gérer les films, les utilisateurs, et l'humeur.
- **Frontend** : Développement d’une interface moderne avec **React** pour permettre aux utilisateurs de choisir leur humeur et voir les suggestions de films.
