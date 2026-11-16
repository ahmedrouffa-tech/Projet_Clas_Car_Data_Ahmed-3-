# 🚗 Prédicteur de Gamme de Prix - Véhicules d'Occasion

Cette application utilise un modèle de Machine Learning (Gradient Boosting Classifier) entraîné sur des données de transactions automobiles pour classifier le prix de revente d'un véhicule d'occasion en deux catégories :
* 🟢 **Prix Standard** (inférieur à la médiane de 8.88 Lakhs)
* 💰 **Prix Élevé** (supérieur ou égal à la médiane de 8.88 Lakhs)

L'interface interactive a été conçue à l'aide de la bibliothèque **Streamlit**.

---

## 📦 Contenu du projet

- **`app.py`** : Le code source de l'application interactive Streamlit.
- **`list_items.joblib`** : Le fichier d'artefact contenant le modèle de Machine Learning entraîné, le scaler standard de normalisation, ainsi que les encodeurs pour les variables catégorielles.
- **`requirements.txt`** : Les dépendances Python indispensables à installer pour faire fonctionner l'application.
- **`runtime.txt`** : Fichier optionnel spécifiant la version cible de Python à utiliser sur Streamlit Cloud.
- **`.gitignore`** : Fichier spécifiant les dossiers locaux à ignorer par Git.
- **`README.md`** : Ce guide d'installation et de déploiement.

---

## 🛠️ Installation et Exécution en local

Pour faire fonctionner l'application sur votre machine locale, suivez ces étapes :

### 1. Cloner ou télécharger le dépôt
```bash
git clone https://github.com/<votre-nom-utilisateur>/<nom-du-depot>.git
cd <nom-du-depot>
```

### 2. Créer et activer un environnement virtuel
```bash
# Sur Mac/Linux
python3 -m venv venv
source venv/bin/activate

# Sur Windows
python -m venv venv
venv\Scripts\activate
```

### 3. Installer les dépendances nécessaires
```bash
pip install -r requirements.txt
```

### 4. Lancer l'application Streamlit
```bash
streamlit run app.py
```
Une fenêtre s'ouvrira automatiquement dans votre navigateur par défaut à l'adresse `http://localhost:8501`.

---

## 🚀 Déploiement en ligne sur Streamlit Cloud

1. Poussez votre code complet sur un dépôt public de votre compte **GitHub**.
2. Rendez-vous sur la plateforme [share.streamlit.io](https://share.streamlit.io/) et connectez-vous avec vos identifiants GitHub.
3. Cliquez sur **"Create App"**.
4. Sélectionnez votre dépôt, la branche `main` et configurez le chemin d'accès principal sur `app.py`.
5. Cliquez sur **"Deploy!"**.

Votre application sera en ligne et accessible via une URL unique en moins de deux minutes !
