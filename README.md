# Credit card fraud detection realtime - Front end

This is front-end source code (React) of our Credit card Fraud detection system. This is a high scalability and intelligent system, heavily rely on AWS architecture.

Our architecture

![architecture](https://github.com/yurri775/system_detection_fraud_credit_card/assets/129472198/63143732-c0ee-4ef4-82b7-816e602827a2)



# Détection de Fraude par Carte de Crédit

La sécurité des fonds des clients est la priorité absolue de toute institution financière. La fraude par carte de crédit engendre non seulement des pertes monétaires, mais également des dommages à la réputation sur le marché et à la confiance des clients.

## Présentation du Projet

Le système de machine learning développé dans le cadre de ce projet vise à détecter les fraudes par carte de crédit en utilisant une approche basée sur des modèles d'apprentissage automatique. Voici un aperçu du fonctionnement du système :

### Fonctionnalités Clés

- **Prétraitement des Données :** Les données des transactions par carte de crédit sont nettoyées et préparées pour l'entrée dans les modèles de machine learning.
  
- **Exploration des Données :** Une analyse approfondie des données est effectuée pour comprendre les distributions et détecter les schémas de fraude potentiels.

- **Entraînement des Modèles :** Plusieurs algorithmes de machine learning sont entraînés sur un ensemble de données pour prédire la probabilité de fraude.

- **Évaluation des Performances :** Les modèles sont évalués en utilisant des métriques telles que la précision, le rappel et l'aire sous la courbe ROC (ROC-AUC).

- **Détection en Temps Réel :** Une fois entraînés et validés, les modèles sont déployés pour analyser les transactions en temps réel et détecter toute activité frauduleuse.

### Équipe de Développement

Ce projet est développé par :

- AKRAM LOULIDI LAHKIM
- MOUAD EL KABIR

## Technologies Utilisées

Le système est développé en utilisant les technologies suivantes :

- Python pour la mise en œuvre des algorithmes de machine learning.
- UML pour la modélisation des données et des processus.
- Jupyter Notebook pour l'analyse exploratoire des données et la visualisation.

## Dataset

Le dataset utilisé dans ce projet provient de Kaggle : [Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud).

## Prétraitement des Données

Les données sont prétraitées pour assurer leur qualité et leur pertinence pour l'entraînement des modèles.

## Modèles de Machine Learning

Les modèles suivants sont utilisés pour la détection de fraude :

- Régression Logistique
- XGBoost
- Arbre de Décision
- Forêt Aléatoire

## Évaluation des Modèles

Chaque modèle est évalué en fonction de plusieurs métriques, fournissant ainsi une indication de sa performance dans la détection de fraudes.

## Feature

- Use ReactJS/ Redux
- Real time update map/chart (polling)
- Map cluster (marker will be join with each other, inspired by [this](https://github.com/istarkov/google-map-clustering-example))
- Data table with pagination
- Ready to integrated with backend

## Installation

To start webpack-dev-server:
```
> npm install
> npm start
```

To start nodejs with dummy data:
```
> node server.js
```

## Demo

Please check our demo at http://creditcard-frauddetection.coddeine.com/

### Screenshot

![fullscreen](https://github.com/yurri775/system_detection_fraud_credit_card/assets/129472198/ce111a57-fa75-43c0-8454-dc118b9ac5ed)


## Date de Livraison

La plateforme sera disponible le 16 mai 2024. Restez à l'écoute pour plus de mises à jour !

---
Ce document est le fruit d'un travail collaboratif entre des experts en apprentissage automatique et des professionnels de la sécurité financière, dans le but de fournir une solution robuste et efficace pour la détection des fraudes par carte de crédit.
