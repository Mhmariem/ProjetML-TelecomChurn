# ProjetML-TelecomChurn
# 📉 Projet : Prédiction du Churn Client dans le Secteur des Télécommunications

## 🌟 Vue d'Ensemble du Projet

> **Et si nous pouvions prédire l'avenir de nos clients avant qu'ils ne décident de partir ?**

Ce projet ambitieux a pour objectif de relever le défi stratégique de la **Prédiction du Churn (Désabonnement) Client** dans le secteur des Télécommunications. En utilisant des techniques avancées d'apprentissage automatique, l'objectif est d'identifier et de retenir les clients à haut risque avant qu'il ne soit trop tard, maximisant ainsi la rétention et la valeur client (CLV).

## 💡 Approche Hybride et Méthodologie

Notre solution repose sur une approche en deux piliers pour une analyse complète :

### 1. Prédiction Supervisée (Identifier qui va partir)

* **Objectif :** Développer un modèle de classification robuste capable de prédire la probabilité de désabonnement pour chaque client.
* **Techniques :**
    * Le déséquilibre des classes a été géré en utilisant la technique **SMOTE** (*Synthetic Minority Over-sampling Technique*).
    * Optimisation des performances de plusieurs algorithmes, notamment **Random Forest** et **Decision Tree**.
* **Validation :** L'approche a permis d'atteindre une précision quasiment égale à celle rapportée dans l'article scientifique de référence, validant la pertinence de la modélisation.

### 2. Analyse Non Supervisée (Comprendre pourquoi ils partent)

* **Objectif :** Découvrir les facteurs et les profils cachés qui influencent le *churn* pour orienter les stratégies de rétention.
* **Techniques :** Combinaison de l'**Analyse en Composantes Principales (PCA)** pour la réduction de dimensionnalité, suivie du **Clustering K-Means** pour segmenter les clients selon les causes d'attrition.

## ⚙️ Technologies et Déploiement

Le projet a mis l'accent sur la robustesse et la capacité à passer en production.

| Catégorie | Outils & Bibliothèques | Utilisation Spécifique |
| :--- | :--- | :--- |
| **Langage** | `Python` | Langage principal de développement. |
| **Modélisation** | `Random Forest`, `Decision Tree` | Modèles de prédiction supervisée. |
| **Techniques ML**| `SMOTE`, `PCA`, `K-Means` | Équilibrage des données, réduction de dimension, segmentation. |
| **Déploiement** | `joblib` | Utilisé pour sérialiser et préserver les objets critiques (ex: `min-max scalers`) pour un déploiement fluide en production. |

## ✅ Impact et Résultats

* **Précision Élevée :** Performance de l'exactitude de la classification comparable aux références scientifiques du domaine.
* **Stratégie Actionnable :** Identification claire des profils clients à cibler (via l'analyse supervisée) et des leviers à activer (via l'analyse non supervisée).
* **Production *Ready* :** Mise en place d'un processus de déploiement optimisé via `joblib`.

