# Mini-Projet Datawarehouse

## Mise en œuvre d’un Data Mart en utilisant Pentaho Data Integration et MySQL

Ce projet consiste en la création et la mise en œuvre d’un Data Mart pour l'analyse des ventes en utilisant Pentaho Data Integration (PDI) et MySQL.

### Membres du Projet

- **Étudiant**: Fedi Bellakhel
- **Tutor**: Mme Zeyneb Trabelsi

### Table des Matières

1. [Introduction Générale](#introduction-générale)
2. [Préparation de la Base de Données en Production](#préparation-de-la-base-de-données-en-production)
3. [Conception du Datamart pour l’Analyse des Ventes](#conception-du-datamart-pour-lanalyse-des-ventes)
4. [Intégration des Données](#intégration-des-données)
5. [Conclusion Générale](#conclusion-générale)

## Introduction Générale

La création et la préparation d’une base de données en production ainsi que la conception d’un Datamart pour l’analyse des ventes constituent des étapes cruciales dans le processus d’analyse de données. L’intégration des données provenant de différentes sources est également une phase essentielle pour garantir la qualité et la cohérence des informations disponibles dans le Datamart.

## Préparation de la Base de Données en Production

1. **Création de la Base de Données**:
   - Ouvrir MySQL Workbench.
   - Se connecter au serveur MySQL.
   - Créer la base de données à partir du fichier SQL `ProductionDumpExemple.sql`.

## Conception du Datamart pour l’Analyse des Ventes

1. **Schéma en Étoile**:
   - Proposer un schéma en étoile pour le Datamart `ventesDM`.
   - Utiliser MySQL Workbench pour créer le modèle de données.

## Intégration des Données

1. **Outils Nécessaires**:
   - Pentaho Data Integration (PDI): Télécharger la dernière version depuis [sourceforge.net](http://sourceforge.net/projects/pentaho).
   - MySQL JDBC Driver: Télécharger et placer le fichier `.jar` dans le répertoire d'intégration.

2. **Processus ETL**:
   - Créer une nouvelle transformation dans PDI.
   - Ajouter une fonction d’extraction et renommer-la `ExtractProduits`.
   - Créer une nouvelle connexion à la base de données `prod`.
   - Alimenter les différentes tables de dimensions (clients, produits, temps) et la table de faits (ventes).

### Conclusion Générale

Ce projet offre un aperçu complet du processus de création, de conception et d’intégration des données pour faciliter l’analyse des ventes. Il met en évidence l’importance de chaque étape dans la création d’un environnement de données robuste et prêt à être exploité pour des analyses approfondies et des prises de décision éclairées.

---

## Instructions de Configuration et d'Exécution

1. **Installation de MySQL**:
   - Télécharger et installer MySQL depuis [mysql.com](https://www.mysql.com/downloads/).

2. **Installation de Pentaho Data Integration**:
   - Télécharger et extraire Pentaho Data Integration depuis [sourceforge.net](http://sourceforge.net/projects/pentaho).
   - Placer le connecteur MySQL JDBC dans le répertoire approprié.

3. **Chargement des Données**:
   - Utiliser MySQL Workbench pour exécuter le script `ProductionDumpExemple.sql` et créer la base de données de production.

4. **Exécution du Processus ETL**:
   - Ouvrir Pentaho Data Integration.
   - Créer une nouvelle transformation et suivre les étapes décrites dans la section [Intégration des Données](#intégration-des-données).

5. **Vérification des Données**:
   - Utiliser MySQL Workbench pour vérifier l'alimentation correcte des tables du Datamart.

---

## Références

- [Pentaho Data Integration Documentation](https://help.pentaho.com/Documentation/9.4/Products/Data_Integration)
- [MySQL Documentation](https://dev.mysql.com/doc/)

Pour toute question ou assistance, veuillez contacter @bellakhelfedi@gmail.com
