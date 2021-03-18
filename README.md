# valeo-challenge 2020 by ENS -> 13th

The goal of the challenge is to predict defect on starter motor production lines (real data!)
Classification task over imbalanced data (0.1% / 99,9%).

HOW TO USE THIS ?
- download thh dataset
- launch the EDA and modeles files in a JUPYTER environnement
- explanations on this challenge can be read here : https://challengedata.ens.fr/participants/challenges/36/

EDA
- localisation of NaNs
- features distribution comparison regarding to their status (OK or KO)
- features correlation observation

MODELES
- data cleaning of meaningless data
- imputation techniques attempts
- over sampling techniques (SMOTE, ADASYN, UNDER et OVERSAMPLING)
- ROC AUC SCORE performance evaluation
- bench with numerous modeles (logistic regression, naive bayes, trees, forests, adaboost, SVM, KNN, XGBoost)
- learning curves
- pipelines (kbest features, polynomial expansion, PCA,...)
- girdsearch hyperparameters optimisation

NB: IsolationForest not tried yet

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

SAME IN FRENCH 

Premier fichier: EDA pour guider la tactique à venir et le choix des modèles:
- localisation des valeurs manquantes
- observation des distributions des variables selon la classe
- observation de la corrélation des variables

Le deuxième fichier est une procédure, évaluée à chaque étape par un indicateur chiffré, pour proposer le modèle le plus adapté et avec des hyperparamètres optimisés.
- nettoyage des colonnes peu renseignées
- essais d' imputation sur les valeurs manquantes (médiane, moyenne, zéro, etc...)
- over sampling (SMOTE, ADASYN, UNDER et OVERSAMPLING) pour palier le déséquilibre de classes
- implémentation d'une fonction d'évaluation de la performance (à base de score AUC)
- comparaison de nombreux modèles (régression logistique, naïve bayes, arbres, forêts, adaboost, SVM, proches voisins, xgboost)
- courbes d'apprentissage
- pipelines aves kbest features, PCA, expansion polynomiale pour adresser l'overfitting ou l'underfitting selon le modèle
- optimisation du meilleur modèle par un gridsearch implémenté à la main

NB : pas eu l'occasion d'essayer un IsolationForest (appris trop tard)
