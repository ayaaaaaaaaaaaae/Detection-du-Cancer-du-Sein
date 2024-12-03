# Détection du Cancer par Méthodes Ensemblistes

## Introduction

Ce projet explore l'utilisation de techniques d'apprentissage ensembliste pour la détection précoce du cancer du sein, en s'appuyant sur la Wisconsin Breast Cancer Database.

## Contexte

Le cancer reste l'une des principales causes de mortalité mondiale. Ce projet vise à démontrer comment l'intelligence artificielle, et plus particulièrement les méthodes ensemblistes, peuvent améliorer la précision du diagnostic précoce.

## Jeu de Données

### Source
- **Wisconsin Breast Cancer Database (Original)**
- Collectée par le Dr William H. Wolberg à l'Université du Wisconsin à Madison
- 699 observations avec 10 attributs cliniques et pathologiques

### Attributs Principaux
- Épaisseur de la grappe
- Uniformité de la taille des cellules
- Uniformité de la forme des cellules
- Adhérence marginale
- Taille des cellules épithéliales
- Etc.

## Méthodologie

### Prétraitement des Données
- Remplacement des valeurs manquantes
- Normalisation Min-Max
- Conversion des valeurs codées '?' en NaN

### Méthodes Ensemblistes Explorées

#### 1. Boosting
- Technique de création d'un classificateur fort à partir de classificateurs faibles
- Algorithme AdaBoost utilisé
- Focus sur la correction itérative des erreurs

#### 2. Bagging (Bootstrap Aggregating)
- Agrégation des prédictions de modèles indépendants
- Réduction du risque de surajustement

#### 3. Stacking
- Combinaison de modèles de base (KNN, ANN, Decision Tree)
- Utilisation d'un méta-modèle (Naive Bayes Classifier)

## Résultats

### Performance Comparative

| Méthode  | Précision |
|----------|-----------|
| Bagging  | 97%       |
| Stacking | 96%       |
| Boosting | 95%       |

### Observations Clés
- Bagging a montré la précision la plus élevée
- Stacking offre une grande flexibilité
- Boosting se concentre sur la correction des erreurs précédentes

## Technologies Utilisées
- Python
- Pandas
- Scikit-learn
- Méthodes d'apprentissage automatique



## Références
- Wisconsin Breast Cancer Database
- Documentation scikit-learn
