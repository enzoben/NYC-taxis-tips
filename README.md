# NYC taxis tips

## Description

On s’intéresse ici à la prédiction du montant de pourboires (tips) payé pour des courses de taxi à New-
York. On dispose d’un jeu de données d’entraînement représentant 100 000 courses de taxis effectuées en
janvier 2024 pour lesquelles le montant des pourboires est connu et un jeu de données de test de courses de taxis effectués lors du même mois. Les données de test et d'entrainement se trouvent à l'adresse suivante :https://www.kaggle.com/competitions/nyc-taxis-tips/

Ce repo contient une analyse de données ainsi que trois modèles de prédiction. La démarche employée est expliquée dans le fichier Kaggle_supervise_MONDELICE_BENBALIT_DUGUERNE.pdf, et les étapes clés sont rappelées dans les notebooks.


## Installation

Les données train et test doivent se trouver dans le dossier data. Le notebook NYTT_data_analysis présente l'analyse des données et l'ensemble des transformation nécéssaires avant d'appliquer les modèles. A la fin de l'exécution du notebook NYTT_data_analysis, deux nouveaux fichiers, obtenus après feature engineering, au format csv seront enregistrés dans le dossier data : train_nettoye et test_nettoye. 
Ensuite, les noteboodks NYTT_linear_regression, NYTT_SVR et NYTT_XGBoost permettent d'appliquer les trois modèles retenus pour ce problème de régression, et enregistrent chacun, dans le dossier output, une prédiction réalisée à partir des données de test `test_nettoye.csv`.

 

Les packages suivants sont à installer
```{C}
pip install -U scikit-learn
pip install xgboost
pip install shap
```

## Description des fichiers et dossiers

| file/folder | description |
|-----------|-----------|
| /data  | Dossier contenant les données train et test, puis les données train_nettoye et test_nettoye après la première exécution de NYTT_data_analysis |
| /output | Dossier qui va contenir les predictions pour chacun des trois modèles retenus|
| `NYTT_data_analysis.ipynb` | Notebook jupyter présentant l'analyse des données et les transformations à appliquer. Ce notebook doit être exécuté avant les trois notebook contenant les modèles |
| `NYTT_linear_regression.ipynb` | Notebook jupyter contenant le modèle de régression linéaire |
| `NYTT_SVR.ipynb` | Notebook jupyter contenant le modèle de Support Vector Regression |
| `NYTT_xgboost.ipynb` | Notebook jupyter contenant le modèle de Gradient Boosting |


