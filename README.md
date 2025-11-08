# Projet Formulaire d'Authentification Django

Ce projet est une application web simple développée avec le framework Python Django. Il met en œuvre un système d'authentification utilisateur de base avec des fonctionnalités d'inscription et de connexion.

## Fonctionnalités

-   **Page d'inscription** : Permet aux nouveaux utilisateurs de créer un compte.
-   **Page de connexion** : Permet aux utilisateurs existants de se connecter.
-   **Page d'accueil** : Une page de bienvenue simple accessible après la connexion.

## Technologies Utilisées

-   **Backend** : Python, Django
-   **Frontend** : HTML
-   **Base de données** : SQLite (par défaut avec Django)

## Installation et Lancement

Suivez ces étapes pour lancer le projet sur votre machine locale.

1.  **Clonez le dépôt**
    ```bash
    git clone <URL_DE_VOTRE_DEPOT>
    cd Formulaire
    ```

2.  **Créez et activez un environnement virtuel**
    ```bash
    # Pour Linux/macOS
    python3 -m venv env
    source env/bin/activate

    # Pour Windows
    python -m venv env
    .\env\Scripts\activate
    ```

3.  **Installez les dépendances**
    Il est recommandé de créer un fichier `requirements.txt`. Pour ce projet, la dépendance principale est Django.
    ```bash
    pip install Django
    ```

4.  **Appliquez les migrations de la base de données**
    Cela créera les tables nécessaires dans votre base de données `db.sqlite3`.
    ```bash
    python manage.py migrate
    ```

5.  **Lancez le serveur de développement**
    ```bash
    python manage.py runserver
    ```
    L'application sera accessible à l'adresse [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Structure du Projet

```
Formulaire/
├── authentification/      # Application Django pour la gestion des utilisateurs
│   ├── migrations/
│   ├── templates/         # Fichiers HTML (inscription, connexion, etc.)
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py           # Formulaires Django
│   ├── models.py          # Modèles de données
│   ├── tests.py
│   └── views.py           # Logique des vues
├── formulaire/            # Fichiers de configuration du projet Django
│   ├── settings.py
│   └── urls.py
├── db.sqlite3             # Base de données
└── manage.py              # Utilitaire de ligne de commande Django
```
