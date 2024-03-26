
# Détection de Fraude par Carte de Crédit

La sécurité des fonds des clients est la principale préoccupation de toute banque. Toute fraude avec une carte de crédit se traduit par une perte pour la banque en termes d'argent, de réputation sur le marché et de confiance des clients.

Le système de machine learning dans ce projet de détection de fraudes par carte de crédit utilise un ensemble de modèles d'apprentissage automatique pour analyser les transactions par carte de crédit et identifier celles qui sont potentiellement frauduleuses. Voici comment le système fonctionne :

Prétraitement des données : Les données des transactions par carte de crédit sont prétraitées pour les rendre appropriées à l'entrée des modèles d'apprentissage automatique. Cela peut inclure des étapes telles que la standardisation des données, la gestion des valeurs manquantes et la suppression des caractéristiques non pertinentes.

Exploration des données : Une analyse exploratoire est effectuée pour comprendre la distribution des données, identifier les tendances et détecter les déséquilibres de classes entre les transactions frauduleuses et non frauduleuses.

Sélection et entraînement des modèles : Plusieurs modèles d'apprentissage automatique sont sélectionnés, tels que la régression logistique, XGBoost, les arbres de décision et les forêts aléatoires. Ces modèles sont ensuite entraînés sur un ensemble de données d'entraînement qui comprend à la fois des transactions frauduleuses et non frauduleuses.

Évaluation des modèles : Les performances de chaque modèle sont évaluées en utilisant des métriques telles que la précision, le rappel, le F1-score et l'aire sous la courbe ROC (ROC-AUC) sur un ensemble de données de test distinct. Cela permet de déterminer quel modèle fonctionne le mieux pour la détection des fraudes.

Sélection du modèle : Le modèle offrant les meilleures performances est sélectionné pour être utilisé dans la détection en temps réel des fraudes sur de nouvelles transactions.

Détection des fraudes en temps réel : Une fois que le modèle est entraîné et sélectionné, il est déployé pour analyser en temps réel les nouvelles transactions par carte de crédit. Le modèle attribue à chaque transaction une probabilité de fraude, et si cette probabilité dépasse un seuil prédéfini, la transaction est marquée comme potentiellement frauduleuse et des mesures appropriées peuvent être prises pour la vérifier.

# Système de Détection de Fraude sur les Cartes de Crédit

## Aperçu du Projet

Ce dépôt contient le code source et la documentation pour un système de détection de fraude sur les cartes de crédit. Il est en cours de développement par :

- Ayoub AMRANI
- AKRAM LOULIDI LAHKIM
- MOUAD EL KABIR

## Fonctionnalités Proposées

Le système comprend les fonctionnalités suivantes, décrites sous forme de User Stories :

1. Détection des transactions suspectes.
2. Analyse des schémas de fraude potentiels.
3. Identification des activités frauduleuses récurrentes.
4. Notification en temps réel des anomalies détectées.
5. Génération de rapports détaillés sur les fraudes.
6. Intégration de techniques avancées de machine learning pour améliorer la précision de la détection.
7. Interface utilisateur conviviale pour la visualisation des données et la gestion des alertes.

## Technologies Utilisées

Le système est développé en utilisant les technologies suivantes :

- Python pour le développement de l'algorithme de détection de fraude.
- UML pour la modélisation des données et des processus.
- Jupyter Notebook pour l'analyse exploratoire des données et la visualisation.



## Dataset
Le dataset utilisé dans ce projet est disponible sur Kaggle : [Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud).

## Prétraitement des données
Le prétraitement des données comprend les étapes suivantes :
- Lecture du dataset
- Gestion des valeurs manquantes
- Analyse de la distribution des données

## Modèles
Les modèles de machine learning utilisés dans ce projet sont :
- Régression logistique
- XGBoost
- Arbre de décision
- Forêt aléatoire

## Évaluation des Modèles
Chaque modèle est évalué en utilisant les métriques suivantes :
- Matrice de confusion
- Rapport de classification
- Précision, Sensibilité, Spécificité, F1-Score
- Courbe ROC

Les résultats sont résumés dans le tableau ci-dessous :

| Modèle                | Précision | F1-Score | ROC     |
|-----------------------|-----------|----------|---------|
| Régression Logistique | 0.9989    | 0.6250   | 0.9764  |
| XGBoost               | 0.9994    | 0.8114   | 0.9724  |
| Forêt Aléatoire       | 0.9989    | 0.6703   | 0.9598  |
| Arbre de Décision     | 0.9988    | 0.6154   | 0.9218  |

---



Voici les détails spécifiques de chaque modèle utilisé dans le projet de détection de fraude par carte de crédit, ainsi que d'autres détails pertinents :

### Régression Logistique
- **Paramètres utilisés :** C=0.01
- **Prétraitement des données :** Standardisation de la colonne "Amount"
- **Évaluation du modèle :**
  - Précision : 99.89%
  - F1-Score : 62.50%
  - ROC : 97.64%
- **Analyse :** La régression logistique offre une précision élevée avec une F1-score et une ROC raisonnables.

### XGBoost
- **Paramètres utilisés :** 
  - learning_rate=0.2
  - max_depth=2
  - n_estimators=200
  - subsample=0.9
- **Prétraitement des données :** Aucun prétraitement supplémentaire nécessaire
- **Évaluation du modèle :**
  - Précision : 99.94%
  - F1-Score : 81.14%
  - ROC : 97.24%
- **Analyse :** XGBoost présente la meilleure performance en termes de F1-score, avec une ROC élevée.

### Arbre de Décision
- **Paramètres utilisés :**
  - max_depth=5
  - min_samples_leaf=100
  - min_samples_split=100
- **Prétraitement des données :** Aucun prétraitement supplémentaire nécessaire
- **Évaluation du modèle :**
  - Précision : 99.88%
  - F1-Score : 61.54%
  - ROC : 92.18%
- **Analyse :** L'arbre de décision offre une précision élevée mais un F1-score relativement faible par rapport aux autres modèles.

### Forêt Aléatoire
- **Paramètres utilisés :**
  - max_depth=5
  - min_samples_leaf=50
  - min_samples_split=50
  - max_features=10
  - n_estimators=100
- **Prétraitement des données :** Aucun prétraitement supplémentaire nécessaire
- **Évaluation du modèle :**
  - Précision : 99.89%
  - F1-Score : 67.03%
  - ROC : 95.98%
- **Analyse :** La forêt aléatoire présente un bon équilibre entre la précision et le F1-score, avec une ROC raisonnable.

### Autres Détails Pertinents
- **Dataset :** Le dataset contient 284,807 transactions, dont seulement 492 sont des fraudes, ce qui montre un fort déséquilibre de classes.
- **Prétraitement des Données :** Les valeurs manquantes ont été vérifiées et aucune n'a été trouvée. La colonne "Time" a été supprimée car aucune tendance claire n'a été observée entre les transactions frauduleuses et non frauduleuses.
- **Évaluation :** Les modèles ont été évalués en utilisant une division train-test avec une taille de train de 80% et une taille de test de 20%. Les performances ont été mesurées en utilisant des métriques telles que la précision, le F1-score et l'aire sous la courbe ROC (ROC-AUC).
- **Conclusion :** Les modèles de machine learning ont été capables de détecter les fraudes avec des performances globalement élevées, bien que certains modèles aient présenté des avantages par rapport à d'autres en termes de F1-score et de ROC.


Date de sortie du JEU
La plateforme sera disponible le 1er Septembre 2024 , Tenez vous prêt !

