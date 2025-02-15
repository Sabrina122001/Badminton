Projet d'Analyse de Données Sportives
Ce projet consiste à analyser des données sportives, en particulier des matchs de tennis en simple et en double, pour prédire les résultats des matchs et évaluer les performances des joueurs. Le projet est divisé en plusieurs notebooks Jupyter, chacun traitant un aspect spécifique de l'analyse.

Fichiers du Projet
  1. ModeleS.ipynb
Ce notebook traite des matchs de tennis en simple. Il comprend les étapes suivantes :

Chargement des données : Les données sont chargées à partir d'un fichier Excel (Singles.xlsx).

Prétraitement des données : Les colonnes Grade et Level sont analysées pour déterminer les valeurs uniques. La colonne Date est convertie en format datetime et les données sont filtrées pour inclure uniquement les matchs entre le 1er janvier 2018 et le 31 décembre 2024.

Calcul des multiplicateurs : Un dictionnaire de multiplicateurs est créé en fonction des colonnes Grade et Level. Ces multiplicateurs sont ensuite appliqués pour créer une nouvelle colonne multiplicateurs.

Encodage des colonnes : Les colonnes Round et Duration sont encodées pour faciliter l'analyse.

Calcul des victoires cumulées : Le nombre de victoires cumulées pour chaque joueur est calculé et utilisé pour classer les joueurs.

Calcul des scores : Un système de score est mis en place pour évaluer les performances des joueurs en fonction de leurs victoires, des rounds joués, et de la durée des matchs.

Modèle de régression logistique : Un modèle de régression logistique est entraîné pour prédire les résultats des matchs en fonction des caractéristiques encodées.

    2. modeleD.ipynb
Ce notebook traite des matchs de tennis en double. Il suit une structure similaire à ModeleS.ipynb mais adaptée aux matchs en double. Les étapes incluent :

Chargement des données : Les données sont chargées à partir d'un fichier Excel (Double.xlsx).

Prétraitement des données : Les colonnes Grade et Level sont analysées et les données sont filtrées par date.

Calcul des multiplicateurs : Un dictionnaire de multiplicateurs est appliqué en fonction des colonnes Grade et Level.

Encodage des colonnes : Les colonnes Round et Duration sont encodées.

Calcul des victoires cumulées : Le nombre de victoires cumulées pour chaque joueur est calculé et utilisé pour classer les joueurs.

Calcul des scores : Un système de score est mis en place pour évaluer les performances des paires de joueurs.

Modèle de régression logistique : Un modèle de régression logistique est entraîné pour prédire les résultats des matchs en double.

    3. analyses.ipynb
Ce notebook est actuellement vide et peut être utilisé pour des analyses supplémentaires ou des visualisations de données.

Installation et Exécution
Pour exécuter ce projet, vous aurez besoin des éléments suivants :

Python 3.x : Assurez-vous d'avoir Python installé sur votre machine.

Jupyter Notebook : Installez Jupyter Notebook pour exécuter les notebooks.

Bibliothèques Python : Les bibliothèques suivantes sont nécessaires :

pandas

numpy

matplotlib

scikit-learn

