# valeo-challenge 2020 by ENS -> 13th

The goal of the challenge is to predict defect on starter motor production lines (real data!)
Classification task over imbalanced data (0.1% / 99,9%).

#########################################################################################################

HOW TO USE THIS ?
- download the dataset
- launch the EDA and modeles files in a JUPYTER environnement
- explanations on this challenge can be read here : https://challengedata.ens.fr/participants/challenges/36/

#########################################################################################################

EDA file : 
- localisation of NaNs
- features distribution comparison regarding to their status (OK or KO)
- features correlation observation

MODELES file : 
- data cleaning 
- imputation techniques attempts
- over sampling techniques (SMOTE, ADASYN, UNDER et OVERSAMPLING)
- ROC AUC SCORE performance evaluation
- bench with numerous modeles (logistic regression, naive bayes, trees, forests, adaboost, SVM, KNN, XGBoost)
- learning curves
- pipelines (kbest features, polynomial expansion, PCA,...)
- hyperparameters optimisation bu gridsearch

NB: IsolationForest not tried yet. Will be done with more time...
