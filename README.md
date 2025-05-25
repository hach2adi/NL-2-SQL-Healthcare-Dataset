# 🧠 Outil LN-2-SQL pour la Gestion des Données Médicales


## 🎯 Objectifs

Ce projet a pour but de développer une solution intelligente capable de :

- Convertir des requêtes en **langage naturel** (français) en requêtes **SQL** valides.
- Permettre au **personnel médical non technique** d'interroger une base de données médicale facilement.
- Proposer une **interface web intuitive** pour la saisie des requêtes et l'affichage des résultats.
- Offrir des fonctionnalités complémentaires comme l'**historique**, l'**exportation** de résultats et la **gestion des erreurs**.

---

## ⚙️ Fonctionnalités principales

| Fonctionnalité              | Description |
|----------------------------|-------------|
| 🔄 Requête LN → SQL        | Conversion d’une phrase en français en requête SQL |
| 📊 Affichage des résultats | Résultats présentés sous forme de tableau lisible |
| 🕒 Historique               | Sauvegarde des requêtes (LN & SQL) avec date/heure |
| ❌ Gestion d'erreurs        | Notifications en cas d'erreurs de syntaxe ou de conversion |
| 🔐 Authentification (optionnelle) | Accès restreint avec rôles : médecin, admin, assistant |
| 📤 Export                   | Export des résultats au format CSV ou PDF |

---

## 🧱 Architecture technique

| Couche       | Technologie                    | Rôle                                      |
|--------------|--------------------------------|-------------------------------------------|
| Frontend     | HTML / JavaScript *(Vanilla ou React)* | Interface utilisateur                   |
| Backend      | Python + FastAPI               | API REST + moteur de conversion LN → SQL |
| Base de données | PostgreSQL                  | Stockage structuré des données médicales  |
| NLP          | Règles ou modèle ML simple     | Compréhension du langage naturel         |
| Tests        | Pytest + tests manuels         | Vérification et validation du système    |

---


## 🚀 Lancement du projet

```bash
# Cloner le dépôt
git clone
cd ln-2-sql-medical

# Installer les dépendances
pip install -r requirements.txt

# Lancer le serveur FastAPI
uvicorn app.main:app --reload
