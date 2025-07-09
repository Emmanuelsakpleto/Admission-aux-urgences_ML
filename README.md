# Projet : Admission aux urgences

## Description

Ce projet analyse une base de données d'environ 32 000 lignes sur les admissions de patients aux urgences. L'objectif principal est d'identifier des patients similaires afin de comprendre les tendances au sein des services d'urgence.

## Installation

Pour exécuter ce projet, vous devez installer les bibliothèques Python suivantes :

  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - (D'autres bibliothèques de scikit-learn pourraient être nécessaires pour DBSCAN et K-Means, bien que non explicitement importées dans le snippet initial, elles sont mentionnées dans la conclusion du notebook)

Vous pouvez les installer via pip :

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Utilisation

1.  **Téléchargez le jeu de données** : Le projet utilise un fichier Excel nommé `2020 09 14 - Admission Urgences.xlsx`. Assurez-vous d'avoir ce fichier et de mettre à jour le chemin d'accès dans le notebook si nécessaire.

2.  **Ouvrez le notebook Jupyter** : Exécutez toutes les cellules du fichier `Admission aux urgences.ipynb` dans un environnement Jupyter Notebook ou JupyterLab.

    ```bash
    jupyter notebook "Admission aux urgences.ipynb"
    ```

## Fichiers Principaux

  - `Admission aux urgences.ipynb`: Le notebook Jupyter contenant l'analyse complète, le prétraitement et la modélisation.
  - `2020 09 14 - Admission Urgences.xlsx`: La base de données des admissions aux urgences.

## Techniques Utilisées

  - **Prétraitement des Données** : Gestion des valeurs manquantes (remplacement par la moyenne pour l'âge, par "Inconnu" pour la catégorie) et suppression des âges aberrants (négatifs).
  - **Visualisation de Données** : Exploration de la structure de la base de données et des distributions.
  - **Clustering** : Utilisation des algorithmes **DBSCAN** et **K-Means** pour identifier des groupes homogènes de patients et des cas atypiques.

## Conclusion

L'application de l'intelligence artificielle à ce domaine de la santé s'est avérée très bénéfique et pertinente, notamment pour améliorer la gestion des urgences dans les pays où elles sont souvent surpeuplées. L'analyse par clustering permet de mieux comprendre les tendances et d'améliorer l'accès aux soins.