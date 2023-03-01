# Nettoyage Preparation Modelisation


## Description du Projet

Ce projet a été réalisé lors de la formation Tech IA chez Simplon HDF. L'objectif est d'analayser, nettoyer un Data Frame contenant les ventes de maison de 2014-2015 dans la conté de King à Washington US, afin de comprendre les variables pour préparer et entraienr un modéle capable prédire les prix de maison à partir de ces même variables.
Le projet est directement lié [à ce projet **](https://github.com/ForskyOnly/djang_app_prediction) et fais partie des 3 premières étapes : le nettoyage, l'analyse et la modélisation.

** Cliquez pour en savoir plus sur l'étape suivante : L'implantation du modéle dans une application web avec Django.


### Contexte du projet


Nous devons effectuer tout d'abord une phase d’exploration de nos données (EDA = Exploratory Data Analysis). Cette phase nous permettra de mieux comprendre nos données.
Après l’EDA, nous avons passer à la phase suivante, la préparation de nos données pour le machine learning. (feature scaling, data transformation, etc.)
Quand nos données étaient prêtes nous avons entraîner notre modèle et atteint un score de 86% de précision pour prédir les prix de maisons.


## Organisation du dossier

Le dossier comporte plusieurs fichiers:

 Trois notebook :
 - "data_clean_analys" : Où nous avons éffectué la prémière phase, l'analyse du DataFrame et de nettoyage de donées 
 - "data_preparation" : Où nous avons préparer nos données et crée des grapfiques avec seaborn et matplotlib afin de mieux comprendre nos données
 - "data_modelisation" : Où nous avons entrainé et tester plusieurs modéles tels que KNeighborsRegressor ( Le modéle ayant obtenu le plus gros score et qui sera utilisé comme model pour notre application Django), LinearRegression, Lasso, Ridge afin de choisir le modéle le plus adéquat pour prédir le prix.


 Trois DataFrame : 
 - "kc_house_data.csv" : le DataFrame inital avec les données brut.
 - "data_hous.csv" : le DataFrame nettoyé.
 - "test_data_hous.csv" : le DataFrale nettoyé, utilisé pour les test et l'entrainement du modéle

### Pré-requis et installation:

- Pour observer les données et les methodes utilisées il suffit de cloner le projet en [Cliquant Ici](https://github.com/ForskyOnly/ml_data_analyse_modelisation) ;
- Avoir installé Python
- Installer et importer les modules suivantes de cette maniére : 
    - from sklearn.linear_model import LinearRegression, Ridge, Lasso
    - from sklearn.model_selection import GridSearchCV, train_test_split, cross_val_score, validation_curve, learning_curve
    - from sklearn.neighbors import KNeighborsRegressor
    - import numpy as np
    - from sklearn.pipeline import Pipeline
    - from sklearn.preprocessing import MinMaxScaler,StandardScaler,OneHotEncoder, RobustScaler
    - from sklearn.compose import ColumnTransformer
    - from sklearn.impute import SimpleImputer
    - import pickle
    - import pandas as pd
    - import matplotlib.pyplot as plt
    - import seaborn as sns