# 🔐 Auth & TodoList Project

Une application web complète développée avec **Node.js**, **Express** et **PostgreSQL**, combinant un système d'authentification sécurisé et une application de gestion de tâches (ToDo List).

Le projet est entièrement réalisé avec **HTML, CSS et JavaScript Vanilla** côté client, tandis que le serveur est développé avec **Express.js**.

---

## ✨ Fonctionnalités

### 👤 Authentification

- Création de compte
- Connexion utilisateur
- Déconnexion
- Gestion des sessions
- Hachage des mots de passe avec **bcrypt**
- Validation des informations

### ✅ Gestion des tâches

- Ajouter une tâche
- Modifier une tâche
- Supprimer une tâche
- Marquer une tâche comme terminée
- Consulter la liste des tâches

---

# 🛠 Technologies utilisées

### Backend

- Node.js
- Express.js
- PostgreSQL
- bcrypt
- express-session
- dotenv

### Frontend

- HTML5
- CSS3
- JavaScript (Vanilla)

---

# 📂 Architecture du projet

```text
login-project/
│
├── db/
│   └── database.sql
│
├── node_modules/
│
├── public/
│   ├── assets/
│   │   ├── css/
│   │   └── images/
│   │
│   ├── inc/
│   │   ├── script.js
│   │   └── todos.js
│   │
│   ├── home.html
│   └── index.html
│
├── .env.example
├── package.json
├── package-lock.json
├── server.js
├── .gitignore
└── README.md
```

---

# 🚀 Installation

## 1. Cloner le dépôt

```bash
git clone https://github.com/tojo_stack/auth_todolist_project.git
cd auth_todolist_project
```

---

## 2. Installer les dépendances

```bash
npm install
```

---

## 3. Configurer les variables d'environnement

Créer un fichier **.env** à la racine du projet.

Exemple :

```env
PORT=3000

DB_HOST=localhost
DB_PORT=5432
DB_NAME=auth_todolist
DB_USER=postgres
DB_PASSWORD=votre_mot_de_passe

SESSION_SECRET=your_secret_key
```

---

## 4. Initialiser la base de données

Créer une base PostgreSQL puis importer le fichier :

```bash
psql -U postgres -d auth_todolist -f db/database.sql
```

ou depuis le terminal PostgreSQL :

```sql
\i db/database.sql
```

---

## 5. Lancer le serveur

Mode production

```bash
npm start
```

Mode développement (si configuré)

```bash
npm run dev
```

L'application sera accessible à :

```
http://localhost:3000
```

---

# 📸 Aperçu

Ajouter ici quelques captures d'écran du projet :

- Page de connexion
- Page d'inscription
- Tableau de bord
- Gestion des tâches

---

# 🔒 Sécurité

- Mots de passe chiffrés avec **bcrypt**
- Variables sensibles stockées dans **.env**
- Sessions utilisateur sécurisées
- Validation des données côté serveur

---

# 🌐 Déploiement

L'application est compatible avec des plateformes comme :

- Render
- Koyeb
- Railway
- Northflank

Une base PostgreSQL distante (Neon, Supabase, etc.) peut être utilisée en production.

---

# 🚀 Évolutions prévues

- [ ] Recherche de tâches
- [ ] Catégories
- [ ] Priorités
- [ ] Dates d'échéance
- [ ] Notifications
- [ ] Responsive amélioré
- [ ] Mode sombre
- [ ] API REST
- [ ] Docker
- [ ] Tests unitaires

---

# 👨‍💻 Auteur

**n0ctua-42**

Étudiant en Télécommunications & Développeur Full Stack

GitHub : https://github.com/n0ctua-42

---

# 📄 Licence

Ce projet est distribué sous la licence MIT.