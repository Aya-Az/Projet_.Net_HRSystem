# 📊 HRSystem - Système de Gestion des Ressources Humaines (GRH)

## 📌 Présentation du projet

Ce projet consiste en la conception et la réalisation d'un Système de Gestion des Ressources Humaines (GRH) destiné à faciliter la gestion du personnel au sein d'une entreprise.

L'objectif principal est de fournir une solution moderne, sécurisée et performante, développée en **.NET**, permettant la centralisation, l'automatisation et le suivi des processus RH.

Ce projet a été réalisé dans un cadre académique, en respectant les bonnes pratiques de conception logicielle et les standards des systèmes d'information.

## 👥 Profils utilisateurs

Le système est basé sur trois profils d'utilisateurs :

- **Administrateur RH**
- **Manager**
- **Employé**

Chaque profil possède des droits d'accès spécifiques et des fonctionnalités adaptées à son rôle.

## 🔐 Authentification et sécurité

- Connexion via email professionnel et mot de passe
- Comptes créés par l'Administrateur RH
- Accès sécurisé selon le rôle utilisateur
- Séparation claire des responsabilités

## ⚙️ Fonctionnalités

### 🧑‍💼 Administrateur RH

L'Administrateur RH dispose des fonctionnalités suivantes :

**Gestion des employés**
- Création d'un employé avec les informations suivantes :
  - Nom, Prénom
  - Email professionnel
  - Téléphone
  - Date de naissance
  - Genre
  - Adresse
  - Département
  - Poste
  - Date d'embauche
  - Type de contrat
  - Statut
  - Salaire
  - Manager associé
- Modification des informations
- Suppression d'un employé
- Consultation des informations détaillées

**Gestion des départements**
- Création d'un département avec :
  - Code département
  - Nom du département
  - Budget annuel
  - Effectif maximum
  - Date de création
- Modification, suppression et consultation

**Gestion des congés**
- Consultation et suivi des congés des employés

**Tableau de bord RH & statistiques**
- Visualisation des indicateurs clés :
  - Nombre total d'employés
  - Répartition par département
  - Répartition par type de contrat
  - État des demandes de congés
- Aide à la prise de décision RH

### 👔 Manager

Le Manager peut :

- Se connecter avec les identifiants fournis par le RH
- Consulter la liste de son équipe
- Consulter les détails des employés
- Gérer les congés des employés :
  - Approuver une demande
  - Rejeter une demande

### 👨‍💻 Employé

L'Employé peut :

- Se connecter avec ses identifiants RH
- Consulter :
  - Son solde de congés restant
- Planifier une demande de congé :
  - Type de congé
  - Solde disponible
  - Date de début
  - Date de fin
  - Durée (en jours)
  - Jours ouvrés
- Consulter le statut de ses demandes

## 📧 Notifications par email

Le système intègre un mécanisme de notifications automatiques par email pour :
- La création de comptes utilisateurs

## 🧩 Conception du système

La conception repose sur plusieurs diagrammes UML, notamment :
- Diagramme de cas d'utilisation
- Diagramme de classes
- Diagramme de séquence
- Diagramme d'activités

**Outil de modélisation :** Draw.io

## 🛠️ Environnement technique

- **Framework / Langage :** .NET 8.0
- **Base de données :** MySQL avec Entity Framework Core
- **Architecture :** ASP.NET Core MVC
- **Frontend :** Bootstrap 5, jQuery
- **Modélisation UML :** Draw.io
- **Gestion de version :** Git & GitHub
- **IDE :** Visual Studio 2022

## 📁 Structure du projet

```
HRSystem/
├── Controllers/         # Contrôleurs MVC
├── Models/              # Modèles de données
├── Views/               # Vues Razor
├── Data/                # Contexte de base de données
├── Migrations/          # Migrations Entity Framework
├── Services/            # Services métier
├── wwwroot/             # Fichiers statiques (CSS, JS, images)
├── Program.cs           # Point d'entrée
└── appsettings.json     # Configuration
```

## 🚀 Installation et exécution

### Prérequis
- [.NET SDK 8.0+](https://dotnet.microsoft.com/download)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) ou [VS Code](https://code.visualstudio.com/)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/) ou [SQL Server](https://www.microsoft.com/sql-server)

### Étapes d'installation

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/Aya-Az/Projet_.Net_HRSystem.git
   cd Projet_.Net_HRSystem
   ```

2. **Configurer la base de données**
   - Modifier la chaîne de connexion dans `appsettings.json`
   - Appliquer les migrations :
   ```bash
   dotnet ef database update
   ```

3. **Restaurer les packages**
   ```bash
   dotnet restore
   ```

4. **Lancer l'application**
   ```bash
   dotnet run
   ```

5. **Accéder à l'application**
   - Ouvrir : `https://localhost:5001` ou `http://localhost:5000`

## 👥 Collaborateurs

- Aya Azari - https://github.com/Aya-Az 
- Inas Mzabi - https://github.com/inas-web 

## 📝 Licence

Ce projet est développé dans un cadre académique.

## 🔗 Liens utiles

- [Documentation .NET](https://docs.microsoft.com/dotnet/)
- [Documentation ASP.NET Core](https://docs.microsoft.com/aspnet/core)
- [Entity Framework Core](https://docs.microsoft.com/ef/core)

---

## ✅ Résultats obtenus

- ✅ Centralisation des données RH
- ✅ Automatisation de la gestion du personnel
- ✅ Suivi efficace des congés
- ✅ Tableau de bord RH avec statistiques
- ✅ Gestion des performances et évaluations
- ✅ Notifications automatiques par email
- ✅ Application sécurisée et modulaire
