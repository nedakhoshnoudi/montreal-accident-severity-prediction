Ce projet porte sur l’analyse et la modélisation de la gravité des accidents de la route à partir de données historiques réelles.

## Jeu de données
Les données proviennent de Données Québec et couvrent les accidents routiers à Montréal entre 2011 et 2022.  
En raison de la taille du jeu de données, les fichiers bruts ne sont pas inclus dans ce dépôt.  
Les données peuvent être téléchargées depuis la source officielle :  
https://www.donneesquebec.ca/recherche/dataset/vmtl-collisions-routieres

## Objectif
L’objectif de ce projet est de prédire les différents niveaux de gravité des accidents de la route à Montréal, avec une attention particulière portée aux accidents graves, moins fréquents mais d’une importance critique.

## Méthodologie
Les données ont été nettoyées et préparées (notamment le traitement des valeurs manquantes), puis séparées en ensembles d’entraînement et de test.  
Plusieurs modèles de classification supervisée (Decision Tree, Random Forest, XGBoost) ont été comparés en tenant compte du fort déséquilibre des classes.  
Des techniques de pondération ainsi que l’ajustement du seuil de décision ont été appliqués afin d’améliorer la détection des accidents graves.  
Un compromis précision–rappel a été analysé pour cette classe afin d’optimiser la performance du modèle.

## Structure du projet
- `*.ipynb` : notebook(s) contenant l’analyse, les expériences et les visualisations
- `requirements.txt` : dépendances Python nécessaires à l’exécution du projet

## Prérequis
- Python 3.9 ou plus récent
- Bibliothèques listées dans `requirements.txt`

## Installation
```bash
pip install -r requirements.txt
