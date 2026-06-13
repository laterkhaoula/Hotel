# 🏨 Système de Gestion de Base de Données pour un Hôtel

##  Description du Projet

Ce projet consiste à concevoir et implémenter une base de données relationnelle destinée à la gestion des activités d’un hôtel. L’objectif principal est de remplacer les registres papier et les fichiers Excel par une solution centralisée, fiable et sécurisée permettant d’améliorer l’organisation et la gestion des informations.

La base de données permet de gérer les clients, les chambres, les réservations et les paiements tout en garantissant une meilleure cohérence des données. Le projet couvre l’analyse des besoins, la modélisation des données selon la méthode MERISE ainsi que l’implémentation SQL sous MySQL.

---

# 🎯 Objectifs du Projet

* Centraliser les informations de l’hôtel dans une base de données unique.
* Faciliter la gestion des clients et des réservations.
* Assurer le suivi des chambres disponibles.
* Enregistrer les paiements des clients.
* Réduire les erreurs liées aux fichiers Excel et aux registres papier.
* Produire des statistiques utiles à la gestion de l’établissement.

---

# 📝 Analyse du Besoin

L’hôtel utilise actuellement plusieurs registres papier et fichiers Excel pour gérer ses activités quotidiennes. Cette organisation présente plusieurs limites :

* Informations clients dispersées.
* Réservations dupliquées ou incorrectes.
* Difficulté de suivi des chambres disponibles.
* Gestion manuelle des paiements.
* Production lente des statistiques.
* Recherche d’informations complexe et chronophage.

Afin d’améliorer son fonctionnement, une étude des besoins a été réalisée afin d’identifier les acteurs du système, les règles de gestion et les données à manipuler.

---

# 👥 Acteurs du Système

### Client

* Effectue une réservation.
* Consulte ses réservations.
* Effectue des paiements.

### Réceptionniste

* Enregistre les informations des clients.
* Gère les réservations.
* Consulte la disponibilité des chambres.

### Responsable de l’Hôtel

* Consulte les statistiques.
* Suit les paiements.
* Contrôle le taux d’occupation des chambres.

### Administrateur

* Gère la base de données.
* Assure la sécurité des données.
* Effectue les sauvegardes.
* Consulte l’historique des réservations et des paiements.

---

# 📋 User Stories

### Client

* Consulter ses réservations.
* Effectuer un paiement.

### Réceptionniste

* Enregistrer les informations des clients.
* Gérer les réservations.
* Consulter les chambres disponibles.

### Responsable

* Consulter les statistiques des réservations.
* Suivre les paiements.
* Analyser le taux d’occupation des chambres.

### Administrateur

* Gérer les utilisateurs.
* Effectuer les sauvegardes.
* Consulter l’historique des réservations et paiements.

---

# 🗄️ Conception de la Base de Données

La modélisation a été réalisée selon la méthode MERISE.

## Modèle Conceptuel de Données (MCD)

Le MCD permet d’identifier les entités, leurs attributs ainsi que les relations existantes entre elles.

### Entités Principales

* Client
* Type_Chambre
* Chambre
* Reservation
* Paiement

## Modèle Logique de Données (MLD)

Le MLD est obtenu à partir du MCD et représente les tables relationnelles prêtes à être implémentées dans MySQL.

---

# 🔗 Relations entre les Entités

* Un client peut effectuer plusieurs réservations.
* Une réservation concerne un seul client.
* Une réservation porte sur une seule chambre.
* Une chambre peut être réservée plusieurs fois à des dates différentes.
* Une chambre appartient à un type de chambre.
* Un paiement est associé à une réservation.

---

# ⚙️ Implémentation SQL

L’implémentation de la base de données a été réalisée en plusieurs étapes :

1. Création de la base de données (**CREATE DATABASE**).
2. Sélection de la base (**USE DATABASE**).
3. Création de la table **client**.
4. Création de la table **type_chambre**.
5. Création de la table **chambre**.
6. Création de la table **reservation**.
7. Création de la table **paiement**.
8. Insertion des données de test (**INSERT INTO**).
9. Consultation des données à l’aide des requêtes (**SELECT**).

---

# 🛠️ Technologies Utilisées

* MERISE
* MySQL
* SQL
* XAMPP
* phpMyAdmin

---

# 📂 Structure du Projet

```text
Projet-Hotel/
│
├── database.sql
├── README.md
├── MCD.png
└── MLD.png
```

---

# 📊 Fonctionnalités Réalisées

* Gestion des clients.
* Gestion des chambres.
* Gestion des réservations.
* Gestion des paiements.
* Consultation des données.
* Analyse et statistiques.

---

# ✅ Résultat

Cette solution permet de centraliser toutes les informations liées à l’activité de l’hôtel dans une base de données relationnelle fiable. Elle facilite la gestion quotidienne, améliore la cohérence des données et simplifie la consultation ainsi que l’analyse des informations.
