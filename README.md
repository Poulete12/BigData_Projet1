# Analyse Stylométrique de La Comédie Humaine

Ce projet réalise une analyse stylométrique de **La Comédie Humaine** d’Honoré de Balzac. Il s’appuie sur l’extraction, le nettoyage et l’annotation linguistique des textes pour explorer les caractéristiques stylistiques de l’œuvre via plusieurs visualisations graphiques.

## Contenu du Projet
- **Extraction des Données** : Clonage du dépôt Git contenant environ 92 textes et le fichier `metadata.csv`.
- **Prétraitement** : Nettoyage des fichiers texte pour normaliser la mise en forme.
- **Annotation Linguistique** : Utilisation du modèle `fr_core_news_md` de spaCy pour extraire diverses statistiques (tokens, mots, phrases, parties du discours, répartition des temps verbaux, etc.).
- **Analyse Stylométrique** :  
  - Visualisation de la distribution moyenne des parties du discours (camembert).
  - Boxplot de la distribution du nombre de verbes selon le genre littéraire.
  - Bar plot de la répartition des temps verbaux.
  - Analyse en composantes principales (ACP) pour distinguer les tendances descriptives et narratives.
  - Dendrogramme hiérarchique illustrant la similarité stylistique entre les textes.

## Prérequis
- **Python 3.x**
- **Bibliothèques** :
  - gitpython
  - pandas
  - dask
  - spaCy (avec le modèle `fr_core_news_md`)
  - scikit-learn
  - plotly
  - matplotlib

## Installation et Exécution
1. **Clonage du dépôt** :  
   Le script se charge de cloner le dépôt situé à `https://github.com/dh-trier/balzac.git` dans le dossier `./DATA/`.

2. **Exécution du Notebook** :  
   Lancez le notebook dans un environnement Jupyter. Le pipeline complet exécutera :
   - L'extraction des textes et des métadonnées.
   - Le nettoyage et l'annotation des textes.
   - La génération des visualisations et analyses.

## Auteurs
**Asso** et **Antony**

## Date
12/05/2025
