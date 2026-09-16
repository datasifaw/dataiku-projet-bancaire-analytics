# Projet bancaire de bout en bout avec Dataiku

## Data Preparation, Analytics, Machine Learning et MLOps

## Contexte

Une banque dispose de données relatives à ses agences, clients,
comptes et transactions.

L'objectif du projet est d'utiliser Dataiku afin de préparer,
fiabiliser, analyser et exploiter ces données dans un Flow complet,
puis de construire des modèles de Machine Learning pour produire
des prédictions, segmenter les clients et automatiser le scoring.

## Données

Le projet utilise quatre sources principales :

- `branches.csv` : informations sur les agences
- `customers.csv` : informations sur les clients
- `accounts.csv` : informations sur les comptes bancaires
- `transactions.csv` : transactions financières

## Architecture du projet

Données bancaires
↓
Data Preparation
↓
Dataset analytique
↓
Dashboard BI
↓
Machine Learning
↙             ↘
Classification   Clustering
↓                ↓
Prédictions      Segments clients
↓
Scoring
↓
Scenario / MLOps

## Objectifs

- Importer les données dans Dataiku
- Explorer et profiler les datasets
- Nettoyer et typer les données
- Gérer les valeurs manquantes et les doublons
- Joindre clients, comptes, agences et transactions
- Construire un dataset analytique
- Créer des KPI financiers
- Construire un dashboard métier
- Créer un modèle de classification
- Segmenter les clients avec du clustering
- Réaliser du scoring
- Automatiser le Flow avec Dataiku Scenarios

## Machine Learning

### Classification

Construire un modèle permettant de prédire si une transaction
appartient à la catégorie des transactions à fort montant.

### Clustering

Segmenter les clients selon leur comportement bancaire, par exemple :

- clients très actifs
- clients à forte valeur
- clients occasionnels
- clients à faible activité

## Dashboard

Le dashboard doit présenter notamment :

- nombre total de transactions
- montant total des transactions
- montant moyen
- nombre de clients actifs
- transactions par type
- transactions par canal
- top clients
- résultats du scoring
- segments clients

## Automatisation

Un Scenario Dataiku permettra d'automatiser :

Nouvelles données
↓
Mise à jour des datasets
↓
Exécution des recettes
↓
Mise à jour du dataset analytique
↓
Scoring Machine Learning
↓
Rafraîchissement du dashboard

## Technologies

- Dataiku
- Visual Recipes
- Prepare Recipe
- Join Recipe
- Group Recipe
- Visual Machine Learning
- Classification
- Clustering
- Python
- SQL
- Dataiku Scenarios
- Dataiku Dashboards
