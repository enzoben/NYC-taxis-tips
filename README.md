# NYC taxis tips

## Description

description rapide de l'étude

## Installation

Les données train et test doivent se trouver dans le dossier data. Le notebook NYTT_data_analysis présente l'analyse des données et l'ensemble des transformation nécéssaires avant d'appliquer les modèles. A la fin de l'exécution du notebook NYTT_data_analysis, deux nouveaux fichiers au format csv seront enregistrés dans le dossier data : train_nettoye et test_nettoye. 
Ensuite, les notebook NYTT_linear_regression, NYTT_SVR et NYTT_XGBoost permettent d'appliquer les trois modèles retenus pour ce problème de régression, et enregistrent chacun, dans le dossier output, une prédiction réalisée à partir des données de test test_nettoye.

## Description des fichiers et dossiers

| file/folder | description |
|-----------|-----------|
| data  | dossier contenant les données train et test |

