## Projet de scoring : Modélisation prédictive des défauts de paiement sur des prêts hypothécaires




1. **Instructions d'installation :** 

1. Cloner le projet

```bash
git clone https://github.com/Ayamokht/Bank-Default-Prediction-ScoringHMEQ.git
cd Bank-Default-Prediction-ScoringHMEQ
```
2. Création d'un environment virtuel


```bash
python -m venv venv
```
3. Activer l'environnement virtuel

* Windows:
```bash
.\venv\Scripts\activate
```
* Linux/Mac:
```bash
source venv/bin/activate
```
4. Installer les dépendances

```bash
pip install poetry 
```
Ensuite, 
```bash
poetry install
```


2. **Objectif du projet :**

Dans le contexte économique contemporain, la maîtrise du risque de crédit demeure une priorité pour les banques et les établissements financiers. Ce projet vise à développer un modèle prédictif permettant d'estimer la probabilité de défaut de paiement sur des prêts hypothécaires.

L'objectif principal est d'identifier les facteurs clés influençant le comportement de remboursement des emprunteurs et d'améliorer la gestion du risque de crédit.

3. **Modèles et métriques :**

Le projet explore plusieurs modèles de classification pour expliquer la variable cible "BAD", qui indique si un emprunteur est en défaut de paiement ou non. Les modèles testés incluent :

* Régression logistique : modèle statistique de base pour la classification binaire.
* Arbre de décision : permet de capturer des relations non linéaires.
* Forêts aléatoires : ensemble d'arbres de décision pour une meilleure généralisation.

Les performances des modèles seront évaluées à l'aide des métriques suivantes :

* Précision : pour mesurer le pourcentage de prédictions correctes.
* Recall : pour mesurer la proportion de cas positifs correctement identifiés.
* F1-score : pour équilibrer précision et recall.
* Courbe ROC et AUC : pour évaluer la capacité du modèle à distinguer les classes.


4. **Structure du projet** : 

```text
📁 Bank-Default-Prediction-ScoringHMEQ/
├── 📁 data/          
│   ├── 📁 hmeq.csv               
│
├── 📁 Sandbox/     
│   ├── 📁 Analyse_exploratoire_des_données.ipynb       
│   ├── 📁 Modèle_Regression_Logistique.ipynb    
│   ├── 📁 Modèle_XGBOOST.ipynb     
│
├── pyproject.toml
├── poetry.lock
```           



