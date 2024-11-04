# etude_clients-POWER-BI
# Tableau de bord Power BI - Analyse des Données des Clients

## Introduction
Ce projet consiste en un tableau de bord interactif créé avec Power BI pour analyser les données des clients, y compris leur profil démographique, le statut matrimonial, le salaire annuel, la répartition des véhicules possédés, et bien plus. Il a été conçu pour fournir des insights utiles et visuels pour faciliter la prise de décision.

## Fonctionnalités Principales
- **Nombre total de clients** : Indique le nombre total de clients analysés.
- **Analyse démographique** : Répartition des clients par sexe (hommes/femmes), statut marital (mariés/célibataires).
- **Répartition des salaires** : Distribution des salaires par tranche d'âge.
- **Statistiques par occupation** : Répartition des salaires selon l'occupation des clients (ex. Management, Professionnel).
- **Propriétaires de véhicules** : Analyse des propriétaires de voitures, avec un classement des 5 principaux propriétaires.

## Visualisations Incluses
- **KPI Cards** : Indicateurs de performance clés pour des données telles que le nombre de clients, le nombre de voitures et les salaires totaux.
- **Graphiques à barres** : Utilisés pour représenter la répartition salariale par occupation et les plus grands propriétaires de voitures.
- **Histogramme** : Représentation de la distribution salariale par âge.
- **Tableau** : Visualisation détaillée des clients avec leurs données telles que le nom, le salaire annuel, le genre, et le statut matrimonial.

## Technologies Utilisées
- **Power BI** : Pour la création de visuels interactifs et de rapports.
- **DAX** : Langage de formule utilisé pour les mesures et les colonnes calculées.

## Mesures Importantes
- **Nombre de clients** : `NbreClients = COUNT(Customers[CustomerKey])`
- **Total des salaires** : `TotalSalaires = SUM(Salaries[Amount])`
- **Pourcentage des mariés/célibataires** : Utilisation de la fonction `CALCULATE()` avec des filtres.

## Comment Utiliser le Tableau de Bord
1. **Filtrage interactif** : Utilisez les filtres pour affiner les données par date de premier achat, nombre d'enfants, etc.
2. **Exploration des visuels** : Cliquez sur les visuels pour voir les interactions et explorer les détails des données.

## Captures d'écran
Voici un aperçu du tableau de bord Power BI :
![Aperçu du tableau de bord](chemin/vers/ton/image.png)

## Améliorations Futures
- Ajouter de nouvelles visualisations pour l'analyse des tendances de consommation.
- Intégrer des prévisions de données pour une meilleure projection.

## Auteur
Ce projet a été réalisé par [Ton Nom], passionné par la visualisation de données et l'analyse décisionnelle.

## Contact
Pour toute question ou collaboration, n'hésitez pas à me contacter via [ton email] ou à visiter mon [LinkedIn](ton-lien-linkedin).

