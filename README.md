# 🧠 Rendu-projet-ML – Prédiction de réponse à une campagne marketing

Ce projet a été réalisé dans le cadre de ma formation en **Data & Intelligence Artificielle**.  
L’objectif est de prédire si un client va répondre ou non à une campagne marketing, en se basant sur quelques données sociodémographiques et comportementales.

## 📁 Fichiers du projet

- `main.ipynb` : Notebook complet avec exploration des données, visualisations, tests de plusieurs modèles de classification, optimisations, et analyse critique.
- `Dataset_Reponse_Marketing.csv` : Jeu de données utilisé dans ce projet (données simulées).
- `.gitignore` : Fichiers et dossiers à exclure du suivi Git.

## 📊 Modèles testés

- Régression Logistique
- KNN avec recherche du meilleur k
- Arbre de Décision (avec et sans GridSearchCV)
- Random Forest (avec et sans GridSearchCV)
- XGBoost (testé mais pas retenu à cause d’un problème d’intégration)

## 🔍 Évaluation

Les modèles sont comparés à l’aide des métriques suivantes :
- Accuracy
- Précision
- Rappel (Recall)
- F1-score
- Matrice de confusion

> **Modèle le plus performant** : Random Forest optimisée, avec un **F1-score ≈ 0.66**

## 🧠 Analyse critique

Malgré une bonne démarche de modélisation, les performances restent limitées par :
- le **faible nombre de variables** disponibles,
- et leur **corrélation modérée avec la variable cible**.

### 💡 Suggestions pour améliorer le modèle :
- Ajouter des variables plus discriminantes (historique d’achat, ancienneté, type de client…)
- Tester des méthodes de feature engineering
