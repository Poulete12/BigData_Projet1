# Analyse Stylométrique de La Comédie Humaine

## Présentation du projet

Ce projet réalise une analyse stylométrique complète de La Comédie Humaine d'Honoré de Balzac, qui regroupe environ 92 textes dressant un portrait détaillé de la société française du XIXe siècle. L'objectif est d'extraire les caractéristiques linguistiques des œuvres pour révéler les tendances stylistiques de l'auteur à travers des analyses quantitatives et visuelles.

## Méthodologie

Le projet suit une démarche structurée en plusieurs étapes :

1. **Extraction des données**
   - Clonage du dépôt GitHub contenant les textes bruts de La Comédie Humaine
   - Conservation uniquement des fichiers texte et des métadonnées associées

2. **Prétraitement des textes**
   - Nettoyage des textes : suppression des astérisques, remplacement des retours à la ligne
   - Normalisation des espaces multiples
   - Création d'un DataFrame pour faciliter l'analyse

3. **Annotation linguistique avec spaCy**
   - Utilisation du modèle `fr_core_news_md` pour l'analyse linguistique approfondie
   - Extraction de caractéristiques clés :
     - Comptage des tokens, mots et phrases
     - Distribution des parties du discours (verbes, noms, adjectifs, pronoms)
     - Répartition des temps verbaux (passé, présent, futur)
     - Calcul de ratios et moyennes statistiques

4. **Analyses stylométriques**
   - Visualisations des distributions lexicales
   - Analyses comparatives par genre littéraire
   - Analyse en Composantes Principales (ACP)
   - Classification hiérarchique (dendrogramme)

## Principaux résultats

### Distribution des parties du discours

L'analyse révèle une prédominance des verbes dans l'œuvre de Balzac, indiquant un style narratif orienté vers l'action et le dynamisme. La part significative des noms propres souligne l'importance accordée à la caractérisation des personnages, tandis que la proportion relativement faible d'adjectifs suggère que les descriptions restent secondaires par rapport à la narration.

### Variations stylistiques par genre

Le projet met en évidence une grande variabilité dans l'usage des verbes selon les genres littéraires. Les romans présentent une diversité stylistique marquée, tandis que les essais affichent une plus grande homogénéité. Cette observation ouvre des perspectives sur la relation entre le genre et les choix stylistiques de l'auteur.

### Temporalité narrative

L'analyse des temps verbaux montre un usage équilibré du passé et du présent dans l'ensemble de l'œuvre, avec une utilisation marginale du futur. Cette répartition temporelle révèle une dynamique narrative où la rétrospection et l'immédiateté coexistent, créant la richesse temporelle caractéristique de l'écriture balzacienne.

### Tendances stylistiques majeures

L'ACP permet d'identifier un continuum stylistique allant d'une écriture descriptive (faible usage de verbes) à une écriture plus narrative et dynamique (forte densité verbale). Cette observation est renforcée par le dendrogramme, qui distingue nettement deux grands clusters d'œuvres, confirmant l'existence de deux orientations stylistiques principales dans La Comédie Humaine.

## Dépendances requises

```
pandas
git
spacy (avec le modèle fr_core_news_md)
dask
plotly
matplotlib
scikit-learn
scipy
```

## Structure du code

Le projet est organisé en sections correspondant aux étapes de l'analyse :

1. **Extraction des données** : clonage du dépôt et récupération des textes
2. **Prétraitement** : nettoyage et normalisation des textes
3. **Annotation linguistique** : analyse avec spaCy et calcul des métriques
4. **Visualisations et analyses** : représentations graphiques et interprétations

## Exécution du projet

Le code peut être exécuté dans un environnement Jupyter ou via un moteur compatible (comme Quarto). Les résultats d'annotation sont sauvegardés dans un fichier CSV pour éviter de répéter les traitements intensifs lors des analyses ultérieures.

## Perspectives

Ce projet ouvre la voie à des analyses plus approfondies de l'œuvre de Balzac, notamment :
- Études diachroniques pour observer l'évolution du style au cours de sa carrière
- Analyse des réseaux de personnages et leur relation avec les choix stylistiques
- Comparaison avec d'autres auteurs de la même période

---

*Projet réalisé par Asso et Antony (2025)*
