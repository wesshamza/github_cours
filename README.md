Téléchargement de l'ensemble de données

L'application Web prend en charge :

     CSV (délimiteur : ',')
     TXT (délimiteur : tabulation)

Résumé de l'ensemble de données

Cette page affichera :

     5 premières lignes pour voir l'aspect général du jeu de données.
     Résumé statistique de chaque colonne.

Prétraitement

Nous pouvons créer un nouveau jeu de données (il sera enregistré au format CSV) avec les options suivantes :

Sélection de fonctionnalité:

     Sélection automatique basée sur l'estimateur Chi-Squared (le nom sera créé en fonction des paramètres choisis) :
         Nombre de fonctionnalités
         Variable de réponse
     Sélection manuelle :
         Nom du nouveau jeu de données
         Sélection des variables

Valeurs nulles et colonnes avec une valeur unique :

     Supprimez les lignes avec des valeurs nulles :
         Null dans TOUTES les colonnes
         Null dans TOUTE colonne
         Jamais
     Supprimez les variables avec une valeur unique :
         Oui
         Non

     Un prétraitement supplémentaire (normalisation, variables fictives...) sera effectué dans les étapes de modélisation et de prédiction.

Graphiques

Visualisations disponibles pour les variables choisies :

     Histogrammes
     Boîtes à moustaches
     Tracés de corrélation

Des modèles

Modèles pour les tâches de classification et de régression. Il ne prend pas en charge la classification multiclasse pour le moment (code supplémentaire pour gérer certaines métriques et graphiques)

Algorithmes disponibles :

     Régression logistique (classification)
     Régression linéaire (Régression)
     Forêts aléatoires (les deux)
     K voisins les plus proches (les deux)
     AdaBoost (les deux)
     Amplification extrême des dégradés (les deux)
     Perceptron multicouche (les deux)

Validation croisée en K (3, 5, 10)

Mise à l'échelle standard (Oui, Non)

Sélection manuelle des fonctionnalités

Résultat des tâches de classification :

     Temps d'ajustement
     Marquer du temps
     Précision (tester et former)
     Rappel (test et formation)
     Score F1 (Test et Train)
     Précision (tester et former)
     ROC AUC (test et formation)
     Tracé des courbes ROC

Sortie des tâches de régression :

     Temps d'ajustement
     Marquer du temps
     Variance expliquée (tester et former)
     R2 (tester et former)
     Erreur quadratique moyenne (test et apprentissage)
     Diagramme des valeurs mesurées et prédites

Prédictions

Construction du modèle (avec le jeu de données complet) et prédiction pour un ensemble de valeurs introduites. Le modèle n'inclura que les variables avec une valeur introduite. Les algorithmes disponibles sont les mêmes que ceux mentionnés dans "Modèles". Il prend également en charge les problèmes multiclasses.

Quelques idées d'amélioration :

     Ajouter des formats et des délimiteurs
     Plus d'estimateurs de fonctionnalités
     Possibilité de choisir entre Train/Test Splits et Cross-Validation
     Ajouter des algorithmes de clustering.
     Réglage des paramètres
     Classification multiclasse dans "Modèles"
     Enregistrer les résultats du modèle dans une base de données
     Prédisez en utilisant toutes les colonnes, en remplissant les variables vides avec la moyenne ou un autre estimateur (cela ne fonctionnerait que pour les variables numériques).
     Personnalisation de la sortie
     Erreur personnalisée pour donner plus d'informations sur ce qui s'est passé (essayer de prédire une variable catégorielle avec un algorithme de régression, etc.)
     Téléchargez un fichier avec des données à prédire.
     Forme du jeu de données et nombre de variables catégorielles et numériques.
