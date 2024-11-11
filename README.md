# NYC taxis tips

## Description

description rapide de l'étude

## Installation

Les données train et test doivent se trouver dans le dossier data. Le notebook NYTT_data_analysis présente l'analyse des données et l'ensemble des transformation nécéssaires avant d'appliquer les modèles. A la fin de l'exécution du notebook NYTT_data_analysis, deux nouveaux fichiers au format csv seront enregistrés dans le dossier data : train_nettoye et test_nettoye. 
Ensuite, les notebook NYTT_linear_regression, NYTT_SVR et NYTT_XGBoost permettent d'appliquer les trois modèles retenus pour ce problème de régression, et enregistrent chacun, dans le dossier output, une prédiction réalisée à partir des données de test test_nettoye.

## Description des fichiers et dossiers

| file/folder | description |
|-----------|-----------|
| data  | dossier contenant les données train et test, puis les données train_nettoye et test_nettoye après la première exécution de NYTT_data_analysis |
| output | dossier qui va contenir les predictions pour chacun des trois modèles retenus|
|-----------|-----------|
| NYTT_data_analysis | notebook jupyter présentant l'analyse des données et les transformations à appliquer. Ce notebook doit être exécuté avant les trois notebook contenant les modèles |
|-----------|-----------|
| NYTT_linear_regression | notebook jupyter contenant le modèle de régression linéaire |
|-----------|-----------|
| NYTT_SVR | notebook jupyter contenant le modèle de Support Vector Regression |
|-----------|-----------|
| NYTT_XGBoost | notebook jupyter contenant le modèle de Gradient Boosting |


