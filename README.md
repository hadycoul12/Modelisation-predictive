# Modélisation prédictive de la demande de vélos en libre-service

Projet de statistique en R : expliquer et prédire le nombre de locations de vélos à partir de variables météorologiques et calendaires.

## Données

`day.csv` (agrégation journalière) et `hour.csv` (agrégation horaire) : nombre de locations, saison, mois, jour de la semaine, température, humidité, vent.

## Démarche (`Projet Reg.Rmd`)

1. **Analyse exploratoire** : distribution des locations par heure, saisonnalité, effet de la température et du jour de la semaine.
2. **Modélisation** avec séparation entraînement / test (80 % / 20 %) :
   - modèle de Poisson, test de surdispersion ;
   - modèle binomial négatif ;
   - modèle additif généralisé (GAM) pour les relations non linéaires ;
   - modèle ARIMA simple.
3. **Comparaison des modèles** : test du rapport de vraisemblance, vérification de la multicolinéarité, erreur de prédiction sur l'échantillon test.
4. **Prédictions et recommandations.**

## Outils

R, ggplot2, dplyr, MASS, mgcv, car, AER, forecast, corrplot.

## Reproduire

Ouvrir `Projet Reg.Rmd` dans RStudio, installer les packages listés en tête de fichier, puis « Knit ».

## Auteur

**Hady Coulibaly**, Data Analyst & Data Scientist, titulaire d'un Master Chef de projet Data & IA (Nexa Digital School). Contact : hady.coulibaly.data@gmail.com · [LinkedIn](https://www.linkedin.com/in/hady-coulibaly-data-ia-france-cdi/)
