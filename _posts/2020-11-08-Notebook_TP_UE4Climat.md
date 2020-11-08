---
layout:            post
title:             "Notebook TP UE4 Climat : de la donnée à l'adaptation"
tags:              Notebooks commentés avec résultats 
category:          Climate Features
author:            tcastel
math:              true
---

## Notebooks des TPs de l'UE4

### TP#1 EDA : Analyse Exploratoire des Données [**ici**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE4/UE4_TP1_EDA.ipynb)

Ce Notebook présente les travaux conduits dans les première séances qui ont visé entres autre à 1) récupérer les données Drias, 2) lire les données Drias avec R, 3) mettre en forme ces données, 4) faire le calcul des moyennes annuelles et mensuelles, 5) Comparer ces données avec des données observées étant au pas de temps mensuel, 6) Evaluation des données Drias , calcul des statistiques (R2, RSME, bias, régression linéaire)

### TP Réserve Utile

Ce TP a été conduit avec QGIS. Les actions conduites ont permis de lire la carte de réserve utile (format image Geotiff) à la résolution de 50m pour toute la Bourgogne. Une carte des point de grille Drias a été créée à partir des coordonnées récupérées lors du TP#1. La réserve utile a ensuite été calculé pour chaque point de grille. La carte a été enregistrée au format shapefile pour être ensuite récupérée sous R. 

### TP#2 Kc : Calcul du coefficient cultural [**ici**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE4/UE4_TP2_Kc.ipynb)

Récupération de Kc au pas de temps mensuel pour 4 occupations du sol. Interpolation de ces données mensuelles au pas de temps journalier. 4 méthodes d'interpolation ont été appliquées.

### TP#3 ETP : Calcul de l'EvapoTranspiration Potentielle [**ici**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE4/UE4_TP3_ETP.ipynb)

Ce TP sera conduit au cours ds séances du lundi 9 novembre et du mardi 10 novembre en distanciel. On cherchera à calculer pour chaque point de grille Drias et à partir des données climatiques simulées l'ETP; Nous utiliserons l'équation de Hargreaves basée sur les températures min et max, la latitude et le jour de l'année.
Vous chercherez également à compléter les données en récupérant le Kc pour chaque jour et la réserve utile pour chaque point de grille.

A l'issu de ce TP toute les données nécessaires pour le calcul du Bilan Hydrique seront disponibles dans le dataframe 'mydrias'

### TP#4 BH : Calcul de l'EvapoTranspiration Potentielle [**ici**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE4/UE4_TP4_BH.ipynb)

Dernière étape qui vise à calculer le Bilan Hydrique à partir des données climatiques Drias, du Kc et de la réserve utile i.e. taille du réservoir.
Une fois le calcul effectué vous explorerez les résultats en traçant le bilan hydrique et d'autres variables.

A partir de là vous aurez en main toutes les étapes pour (re)produire le calcul du bilan sur vos données Drias et de Kc qui dépend de votre choix.

Il conviendra enfin de réfléchir à des indices synthétique pertinent qui permettront de 1) synthétiser l'information sur le BH et 2) en utilisant ces indices calculés sur le période historique (1975-2005) et sur la période projetée (2070-2100) d'évaluer l'impact du CC sur ce bilan.
