# Projet bancaire de bout en bout avec Dataiku

## Contexte

Une banque dispose de données relatives à ses agences, clients,
comptes et transactions.

L'objectif du projet est d'utiliser Dataiku afin de préparer,
fiabiliser, analyser et visualiser ces données dans un Flow complet.

## Données

Le projet utilise quatre sources principales :

- `branches.csv` : informations sur les agences
- `customers.csv` : informations sur les clients
- `accounts.csv` : comptes bancaires
- `transactions.csv` : transactions financières

## Architecture du projet

CSV
↓
Dataiku datasets
↓
Préparation des données
↓
Contrôles qualité
↓
Jointures
↓
Dataset analytique
↓
Agrégations et KPI
↓
Dashboard
↓
Scenario d'automatisation

## Objectifs

- Importer les données dans Dataiku
- Explorer et comprendre les datasets
- Nettoyer les données
- Corriger les types
- Supprimer les doublons
- Contrôler les valeurs manquantes
- Joindre les données clients, comptes et transactions
- Construire des indicateurs financiers
- Créer un dashboard métier
- Automatiser le Flow avec un Scenario Dataiku

## Analyses métier

Le projet doit permettre notamment d'analyser :

- le nombre total de transactions
- le montant total des transactions
- le montant moyen des transactions
- le nombre de clients actifs
- les transactions par type
- les transactions par canal
- les clients générant les montants les plus importants

## Extension avancée

Une extension Machine Learning peut être ajoutée afin
d'identifier des transactions potentiellement atypiques à partir
du montant, du canal, du type de transaction et du comportement
des comptes.

## Technologies

- Dataiku DSS
- Visual Recipes
- Prepare Recipe
- Join Recipe
- Group Recipe
- Python / SQL en complément
- Dataiku Scenarios
- Dataiku Dashboards

## Résultat attendu

Un Flow Dataiku complet permettant de passer des données bancaires
brutes à des datasets fiables, des indicateurs métier et un
dashboard financier automatisé.
