# valeo-competition-project
Classé 13 ième de la compétition (ma première).

Compétition organisée par l'ENS, à partir de données réelles de l'entreprise VALEO recueillies par des capteurs sur une chaine de montage industrielle.
Il s'agit d'un problème de classification avec classes très déséquilibrées (0.1% / 99,9%).

EDA pour guider la tactique à venir et le choix des modèles:
- localisation des valeurs manquantes
- observation des distributions des variables selon la classe positive ou négative
- observation de la corrélation des variables

Le deuxième est une méthodologie simple appliquée pour proposer un modèle final optimal.
(prise de décision en évaluant le meilleur choix à chaque étape grâce à unique indicateur chiffré)
- nettoyage des colonnes peu renseignées
- essais d' imputation sur les valeurs manquantes (médiane, moyenne, zéro, etc...)
- normalisation du set
- over sampling (SMOTE, ADASYN, UNDER et OVERSAMPLING) pour palier le déséquilibre de classes
- implémentation d'une fonction d'évaluation de la performance (à base de score AUC)
- comparaison de nombreux modèles (régression logistique, naïve bayes, arbres, forêts, adaboost, SVM, proches voisins, xgboost)
- courbes d'apprentissage sur les meilleurs modèles
- pipelines aves kbest features, pca, expansion polynomiale pour adresser l'overfitting ou l'underfitting selon le modèle
- optimisation du meilleur modèle par un gridsearch implémenté à la main

NB : tester un isolation forest aurait du être fait (appris trop tard)
