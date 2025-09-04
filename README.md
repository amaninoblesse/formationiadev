# 📚 Library API - Projet de formation IA

Ce repository contient le projet **Library API**, une application de gestion de bibliothèque, spécialement conçue pour la **formation sur l'intégration de l'IA dans le développement avec Django REST Framework**.

---

## 🚀 État du projet
Le projet est configuré et fonctionnel, mais des parties cruciales (**vues, tests, documentation**) sont à compléter pendant la formation en utilisant l'IA générative.

---

## 🎯 Objectifs de la formation
- Découvrir comment l’IA peut accélérer le développement.  
- Expérimenter la collaboration entre différents métiers (**Dev, QA, Analyste**) autour de l’IA.  
- Apprendre à générer du code, des tests et de la documentation avec des outils comme **GitHub Copilot, ChatGPT, Claude, Windsurf**.  
- Comprendre les bonnes pratiques et les limites de l’assistance par l’IA.  

---

## 👥 Rôles et tâches
- **Développeur / Intégrateur** : Implémentation des vues API (`views.py`).  
- **Ingénieur Qualité** : Écriture de la suite de tests (`tests.py`).  
- **Analyste Fonctionnel** : Rédaction de la documentation et validation des spécifications.  

---

## 🛠️ Prérequis
Avant de commencer, assurez-vous d’avoir installé :  
- [Python 3.8+](https://www.python.org/downloads/)  
- [Git](https://git-scm.com/downloads)  
- Un IDE recommandé : **VS Code** (avec extension Python + GitHub Copilot), **Windsurf** pour expérimenter l’IA, et **Postman** pour tester les APIs.  
- Comptes gratuits sur **ChatGPT**, **Claude.ai**, ou tout autre assistant IA.  

---

## ⚙️ Installation et configuration

### 1. Cloner le repository
```bash
git clone https://github.com/amaninoblesse/formationiadev.git
cd formationiadev
```
### 2. Créer un environnement virtuel
Il est fortement recommandé d'isoler les dépendances de votre projet dans un environnement virtuel.

### Sur Windows :

```bash
python -m venv venv
venv\Scripts\activate
```

### Sur macOS/Linux :

```bash
python -m venv venv
source venv/bin/activate
```
Votre invite de commande devrait maintenant afficher (venv) au début.

### 3. Installer les dépendances
Une fois l'environnement virtuel activé, installez tous les packages nécessaires :

```bash
pip install -r requirements.txt
```

### 4. Démarrer le serveur de développement
Lancez le serveur Django pour vérifier que l'installation est un succès.

```bash
python manage.py runserver
```
Ouvrez votre navigateur et allez à l'adresse : http://localhost:8000/admin

VOUS DEVRIEZ VOIR : Une interface d'administration qui demande de saisir le username et password. Félicitations, l'installation est réussie !

VOUS VOYEZ UNE ERREUR ? Vérifiez que vous avez bien exécuté toutes les étapes précédentes.

Structure du Projet
```text
formationiadev/
├── core/                # Configuration principale du projet Django
│   ├── settings.py      # Config : Apps, DB, DRF (Déjà configuré)
│   ├── urls.py          # URLs principaux (Déjà configuré)
│   └── ...
├── library/             # Application principale "Library"
│   ├── migrations/      # Fichiers de migration de la base de données
│   ├── models.py        # MODÈLES - COMPLET (Author, Book)
│   ├── serializers.py   # SÉRIALISEURS - COMPLET (AuthorSerializer, BookSerializer)
│   ├── urls.py          # URLs de l'app - PARTIEL (Search est configuré)
│   ├── views.py         # VUES - À COMPLÉTER PENDANT LA FORMATION
│   ├── tests.py         # TESTS - À COMPLÉTER PENDANT LA FORMATION
│   └── ...
├── requirements.txt    # Liste des dépendances Python
├── manage.py           # Script de management Django
└── README.md           # Ce fichier
```

Comment Tester Votre Installation
Avant la formation, assurez-vous que tout fonctionne en testant les points suivants :

L'API de test (Déjà fonctionnelle) :

Allez sur http://localhost:8000/library/api/test. Vous devriez obtenir une réponse JSON :

```json
{
    "message": "Test réussi"
}
```

## Démarrage de la formation
Une fois votre environnement vérifié, vous êtes prêt pour la formation.

Ouvrez le projet dans votre IDE (VS Code recommandé ou windsurf).

Ouvrez le fichier library/views.py : Vous verrez que les classes vues principales (BookListCreateAPIView, BookDetailAPIView, etc.) sont manquantes et devront être implémentées avec l'aide de l'IA.

Ayez sous le pied la bibliothèque de prompts qui vous sera fournie.

Ayez prêts vos assistants IA (Onglets ChatGPT, Claude, Copilot activé dans VS Code).

## Dépannage commun
ModuleNotFoundError: No module named ... : Votre environnement virtuel n'est probablement pas activé. Réactivez-le (venv\Scripts\activate sur Windows) et ré-exécutez pip install -r requirements.txt.

Error: That port is already in use. : Le port 8000 est utilisé. Tuez le processus ou lancez le serveur sur un autre port : python manage.py runserver 8001.

## Ressources utiles
- [Documentation Django](https://docs.djangoproject.com/fr/5.2/)
- [Documentation Django REST Framework](https://www.django-rest-framework.org/)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)

✍️ Conçu et préparé par Noé Amani