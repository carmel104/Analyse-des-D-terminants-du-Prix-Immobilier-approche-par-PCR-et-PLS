# 🏡 Analyse des Déterminants du Prix Immobilier

Ce projet vise à identifier et à modéliser les facteurs influençant le prix de vente des biens immobiliers en utilisant différentes approches de régression, notamment pour gérer les problèmes de multicolinéarité.

---

## 📋 Objectifs du Projet

L'objectif principal est d'explorer les relations entre les caractéristiques structurelles, environnementales et fonctionnelles des logements et leur prix de vente final.

---

## 📊 Jeu de Données

L'étude s'appuie sur une série de variables descriptives incluant :

### 🏠 Surfaces
- Superficie du terrain (LotArea)
- Surface habitable (GrLivArea)
- Surface du sous-sol (TotalBsmtSF), etc.

### 🚿 Équipements
- Nombre de salles de bain (FullBath, BsmtFullBath)
- Capacité du garage (GarageCars)
- Nombre de cheminées

### 🧱 Configuration
- Nombre de chambres (BedroomAbvGr)
- Nombre total de pièces (TotRmsAbvGrd)

---

## 🛠️ Méthodologie

Le projet compare trois méthodes de régression pour prédire la variable cible **SalePrice** :

### 📌 Régression Linéaire Classique
Utilisée comme base, avec un traitement préalable pour retirer les variables fortement corrélées afin d'éviter la multicolinéarité.

### 📌 Régression sur Composantes Principales (PCR)
Réduit la dimensionnalité en extrayant des composantes orthogonales qui maximisent la variance des covariables.

### 📌 Régression des Moindres Carrés Partiels (PLS)
Construit des composantes latentes en maximisant la covariance entre les variables explicatives et la variable cible.

---

## 📈 Résultats Clés

### 🔎 Facteurs Déterminants
Les surfaces habitables, le sous-sol, le garage et le nombre de pièces d'eau sont les prédicteurs les plus influents du prix.

### ⚠️ Multicolinéarité
L'analyse a révélé de fortes corrélations, notamment entre les variables de surface et celles liées au garage.

### 📊 Performance des modèles
- La première composante des modèles PCR/PLS explique à elle seule près de **70 %** de la variance du prix de vente.
- Les méthodes par composantes latentes (PCR et PLS) se sont révélées plus robustes pour gérer la redondance des informations que la régression classique.

---

## 👥 Auteurs

* Carmel AWANDE  
* Yves GNONHOUE 
