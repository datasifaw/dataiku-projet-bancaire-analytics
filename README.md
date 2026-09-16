# Projet bancaire de bout en bout avec Dataiku

## Contexte

Une banque dispose de données relatives à ses agences, clients,
comptes et transactions.

L'objectif du projet est d'utiliser Dataiku afin de préparer,
fiabiliser, analyser et exploiter ces données dans un Flow complet,
puis d'ajouter une couche de Machine Learning pour produire des
prédictions et segmentations utiles aux analystes.

## Données

Le projet utilise quatre sources principales :

- `branches.csv` : informations sur les agences
- `customers.csv` : informations sur les clients
- `accounts.csv` : informations sur les comptes bancaires
- `transactions.csv` : transactions financières

## Architecture du projet

CSV
↓
Dataiku Datasets
↓
Préparation et nettoyage
↓
Contrôles qualité
↓
Jointures
↓
Dataset analytique
↓
KPI financiers
↓
Dashboard
↓
Machine Learning
↓
Prédictions / Segmentation
↓
Scenario Dataiku

## Objectifs du projet

- Importer les données dans Dataiku
- Explorer les datasets
- Nettoyer les données
- Corriger les types
- Gérer les valeurs manquantes
- Supprimer les doublons
- Joindre les données clients, comptes et transactions
- Construire un dataset analytique bancaire
- Calculer des indicateurs financiers
- Créer un dashboard métier
- Construire un modèle de Machine Learning
- Produire des prédictions
- Segmenter les clients
- Automatiser le Flow avec un Scenario Dataiku

## Partie Data Preparation

Les traitements principaux sont réalisés avec les recettes visuelles
de Dataiku :

- Prepare Recipe
- Join Recipe
- Group Recipe
- Filter Recipe
- Stack Recipe si nécessaire

Les transformations peuvent également être complétées avec Python ou SQL.

## Analyse métier

Le projet permet notamment d'analyser :

- le nombre total de transactions
- le montant total des transactions
- le montant moyen des transactions
- le nombre de clients actifs
- les transactions par type
- les transactions par canal
- les clients générant les montants les plus importants
- la répartition de l'activité par agence
- l'activité des comptes bancaires

## Machine Learning

### 1. Classification des transactions à fort montant

Un premier modèle peut être construit pour prédire si une transaction
appartient à la catégorie "montant élevé".

Exemple de variable cible :

`transaction_elevee`

- `1` : transaction à fort montant
- `0` : transaction classique

Le seuil peut être défini à partir de la distribution des montants
ou d'une règle métier.

Variables possibles :

- montant
- type de transaction
- canal
- compte
- agence
- statut
- caractéristiques du client

Le modèle peut être construit avec Visual Machine Learning de Dataiku.

### 2. Segmentation des clients

Une deuxième analyse peut utiliser un algorithme de clustering afin
de créer différents profils de clients.

Exemples de variables :

- nombre de transactions
- montant total
- montant moyen
- nombre de comptes
- type de compte
- fréquence d'activité

Exemples de segments obtenus :

- clients très actifs
- clients à forte valeur
- clients occasionnels
- clients à faible activité

## Prédictions

Une fois le modèle entraîné, Dataiku peut générer un dataset de scoring
contenant notamment :

- la prédiction
- la probabilité associée
- les principales variables utilisées par le modèle

Ces résultats peuvent ensuite être exploités dans le dashboard.

## Dashboard

Le dashboard doit présenter au minimum :

- Nombre total de transactions
- Montant total
- Montant moyen
- Nombre de clients actifs
- Transactions par type
- Transactions par canal
- Top clients
- Répartition de l'activité
- Résultats du modèle de Machine Learning
- Segments clients

## Automatisation

Un Scenario Dataiku permet d'automatiser le projet.

Exemple de scénario :

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

## Technologies utilisées

- Dataiku DSS
- Visual Recipes
- Prepare Recipe
- Join Recipe
- Group Recipe
- Dataiku Visual Machine Learning
- Classification
- Clustering
- Python
- SQL
- Dataiku Scenarios
- Dataiku Dashboards

## Résultat attendu

À la fin du projet, le Flow Dataiku doit permettre de passer de données
bancaires brutes à :

- des données nettoyées et fiables
- un dataset analytique
- des indicateurs financiers
- un dashboard métier
- un modèle prédictif
- une segmentation des clients
- un processus automatisé avec Dataiku Scenarios

## Extension avancée

Des extensions peuvent être ajoutées :

- prédiction du montant des transactions
- prévision du volume de transactions
- détection de transactions atypiques
- scoring client
- comparaison de plusieurs modèles
- analyse de l'importance des variables
- suivi des performances du modèle
