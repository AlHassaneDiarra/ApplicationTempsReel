# ⚡ Application Temps Réel avec Socket.IO

## 📌 Description

Ce projet est une application **temps réel** construite avec **Node.js**, **Socket.IO** et un client frontend.  
Il illustre comment mettre en place une communication **bidirectionnelle en temps réel** entre un serveur et plusieurs clients.

L’architecture est séparée en deux parties :
- **Backend (serveur Node.js + Socket.IO)** : gère les événements temps réel, la logique métier et la communication.  
- **Frontend (client)** : interface utilisateur qui se connecte au serveur via WebSocket.  

---

## 📂 Structure du projet

Socket.io_UA1/
│
├── client/ # Code du client (frontend)
│ ├── package.json
│ ├── package-lock.json
│ ├── src/ # Composants et logique client
│ ├── public/ # Fichiers statiques
│ └── node_modules/ # Dépendances (auto-générées)
│
└── server/ (si présent) # Backend Node.js
├── app.js / index.js # Point d’entrée du serveur
├── package.json
├── routes/ # Routes API classiques
├── models/ # Schémas (MongoDB ou autres BDD)
└── socket/ # Gestion des événements Socket.IO

---

## ⚙️ Technologies utilisées

- **Node.js** (backend)  
- **Express.js** (framework serveur HTTP)  
- **Socket.IO** (communication temps réel)  
- **React.js** ou client léger avec Webpack (frontend)  
- **MongoDB** (si utilisé pour stocker les données, ex. utilisateurs / scores)  

---

## 🚀 Installation et exécution

### 1️⃣ Cloner le projet
```bash
git clone https://github.com/AlHassaneDiarra/ApplicationTempsReel
cd Socket.io_UA1
2️⃣ Installer les dépendances
Backend
cd server
npm install

Frontend
cd client
npm install

3️⃣ Lancer le serveur
cd server
npm start
➡️ Le backend tourne sur http://localhost:4000 (ou autre port configuré)

4️⃣ Lancer le client
cd client
npm start
➡️ Le frontend tourne sur http://localhost:3000

🔧 Fonctionnalités principales
Connexion en temps réel via Socket.IO

Événements bidirectionnels entre serveur et client

Gestion de plusieurs clients connectés simultanément

Mise à jour instantanée de l’interface utilisateur

📡 Exemple d’utilisation
Ouvrez deux navigateurs différents sur http://localhost:3000

Connectez-vous en tant qu’utilisateurs distincts

Les événements envoyés par un client (ex. message, action de jeu) apparaissent instantanément chez les autres clients connectés

📜 Licence
Projet sous licence MIT – libre d’utilisation et de modification.

👨‍💻 Auteur
Développé par Al Hassane Diarra
