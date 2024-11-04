# etude_clients-POWER-BI
# Tableau de bord Power BI - Analyse des Données des Clients

## Introduction
Ce projet consiste en un tableau de bord interactif créé avec Power BI pour analyser les données des clients, y compris leur profil démographique, le statut matrimonial, le salaire annuel, la répartition des véhicules possédés, et bien plus. Il a été conçu pour fournir des insights utiles et visuels pour faciliter la prise de décision

## Contexte du Projet
Plusieurs entreprises ont besoin de solutions de visualisation de données pour analyser leur clientèle et optimiser leurs stratégies de vente et de marketing. Ce tableau de bord Power BI a été conçu pour une entreprise fictive spécialisée dans la vente de biens et services haut de gamme, souhaitant améliorer sa connaissance des clients et identifier des opportunités de croissance.

### Objectifs du Projet
- **Analyse des caractéristiques démographiques** : Identifier la répartition de la clientèle par âge, genre, statut matrimonial, et occupation pour personnaliser les offres et campagnes marketing.
- **Étude de la répartition des revenus** : Comprendre comment les salaires des clients se répartissent afin de mieux cibler les segments à fort pouvoir d'achat.
- **Propriétés des clients** : Analyser le nombre de voitures possédées par les clients et identifier les principaux propriétaires pour des stratégies de fidélisation.
- **Prise de décision basée sur les données** : Fournir des insights exploitables pour les équipes de vente et de gestion.

### Cas d'Utilisation
Ce tableau de bord peut être utilisé par les départements de marketing et de vente pour :
- Cibler les campagnes promotionnelles sur des groupes spécifiques de clients.
- Développer des stratégies basées sur le comportement d'achat des clients selon leur profil.
- Identifier des tendances cachées qui pourraient influencer les futures décisions stratégiques de l'entreprise.


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
- **YY somme salaire annuel** = SUM(Customers[YearlyIncome])
- **YY nbreHomme** = COUNTROWS(FILTER(Customers,Customers[Gender]="M"))`
- **YY nbrefemme** = COUNTROWS(FILTER(Customers,Customers[Gender]="M"))
- **YY Clientscelibataires** = CALCULATE(DISTINCTCOUNT(Customers[CustomerKey]),FILTER(Customers,Customers[MaritalStatus]="S"))
- **YY Clientsmariés** = CALCULATE(DISTINCTCOUNT(Customers[CustomerKey]),FILTER(Customers,Customers[MaritalStatus]="M"))
- **YY %hommes** = DIVIDE([YY nbreHomme],([YY nbrefemmes]+[YY nbreHomme]),0)

## Comment Utiliser le Tableau de Bord
1. **Filtrage interactif** : Utilisez les filtres pour affiner les données par date de premier achat, nombre d'enfants, etc.
2. **Exploration des visuels** : Cliquez sur les visuels pour voir les interactions et explorer les détails des données.

## Captures d'écran
Voici un aperçu du tableau de bord Power BI :
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
![Capture d’écran 2024-11-04 174902](https://github.com/user-attachments/assets/ae3bb0e6-2476-41ca-9166-e0aef70b0945)


## Améliorations Futures
- Ajouter de nouvelles visualisations pour l'analyse des tendances de consommation.
- Intégrer des prévisions de données pour une meilleure projection.

## Auteur
Ce projet a été réalisé par Ryan TCHUISSEU, passionné par la visualisation de données et l'analyse décisionnelle.

## Contact
Pour toute question ou collaboration, n'hésitez pas à me contacter via donel.tchuisseu@gmaiL.com ou à visiter mon  http://www.linkedin.com/in/ryan-tchuisseu.

