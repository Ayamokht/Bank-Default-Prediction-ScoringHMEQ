# ScoringHMEQ

## Instructions d'installation

1. **Créer un environnement virtuel :**

   Dans le dossier parent du projet, exécutez la commande suivante :
   ```
   python -m virtualenv .venv --python=python3.11
   ```
    Puis il faut l'activer avec : 
    ```
    cd .\.venv\Scripts\activate.ps1
    ```
    Installer poetry :
    ```
    pip install poetry
    ```
    Rentrer dans le projet:
    ```
    cd .\ScoringHMEQ\
    ```
    Installer les dépendances
    ```
    poetry install
    ```
    Lancer ce code pour définir la variable d'environnement directement dans PowerShell 
    ```
    env:PYTHONPATH = "$env:PYTHONPATH;$PWD"
    ```
    Lancer le modèle logit 
    ```
    python src/cli/cli.py --model logit
    ```

2. **Objectif du projet :**
Ce projet consiste à proposer un modèle expliquant la variable « BAD » à partir des autres variables disponibles dans le jeu de données hmeq. 

3. **Livrables** :
Rapport synthétique (.doc) ormatiques utilisés pour réaliser les analyses et le modèle. Le projet peut être réalisé avec Python, R, et/ou SAS. code Python 

4. **Structure du dépôt** :
- /src : Ce dossier contient tous les scripts Python nécessaires à la réalisation des analyses et à la construction du modèle. 
- /sandbox : Des notebooks Jupyter utilisés pour tester des idées ou explorer des pistes avant leur implémentation finale dans les scripts.
- /output : 
Les graphiques générés lors des analyses, les fichiers de modèles enregistrés, les rapports intermédiaires et résultats chiffrés.
- rapport.docx : Le document principal contenant le rapport synthétique détaillé des analyses.

5. **Instructions pour exécuter le projet** : 
Pré-requis : 
```
poetry install
python src/.py
python src/report_generator.py
``` 
Le projet explore plusieurs algorithmes de classification afin d'expliquer la variable cible « BAD » :
Régression logistique
Arbre de décision
Forêts aléatoires

Les modèles seront évalués selon les métriques suivantes :
Précision
Recall
F1-score
Courbe ROC et AUC


