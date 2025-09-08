---
layout:            post
title:             "UE2 M2SEME: Interpolation spatiale"
date:              2025-09-08 17:30:00 +0300
tags:              GIS
category:          GIS Features
author:            tcastel
math:              true
---


### Analyse données géographiques : Interpolation spatiale

**Objectifs :**

Afin de pouvoir estimer la part de contribution du ruissellement des pluies sur la pollution au phosphore, il est nécessaire de connaître le cumul de précipitations en tout point du bassin versant. Malheureusement, cette information n’est pas mesurée au niveau du bassin de la Sorme. Les stations climatiques disponibles sont situées à l’extérieur de ce dernier.

Pour estimer les cumuls de pluie au niveau de bassin versant, nous vous proposons de mobiliser des méthodes d’interpolation spatiale.
L’objet de cette dernière partie de l'UE 2 : traitement de la donnée est de vous faire mobiliser des méthodes et outils standards d’interpolation spatiale des données :

    * La régression multiple
    * Le krigeage ordinaire (technique appartenant à la discipline des géostatistiques)

Vous serez guidés pas à pas pour interpoler les cumuls annuels de pluie mesurés par le réseau des stations de Météo-France. 

  
### Le support du TP, les données (MNT, départements, BV), les scripts pour les 3 premières étapes sont à récupérer ([ici](https://filesender.renater.fr/?s=download&token=f58155b0-666d-4dfd-a363-eb5bfb55d01e)


# Les étapes du travail

### Étape 1 : Traitement et mise en forme des données

* Lecture des données ;
* Agrégation des données climatiques au pas de temps annuel;
* nettoyage des données 

### Étape 2 : Exploration et modèle de régression 

* Construction du modèle linéaire multiple entre variables explicatives (X, Y et altitude) et la variable climatique (corrélations) ;
* Mesure de la significative des variables retenues dans le modèle (r, p-value);
* Évaluation de la qualité du modèle (R2 ajusté, RMSE sur les résidus).

### Étape 3 : Interpolation spatiale par régression linéaire
* Interpolation des cumuls de pluies annuels à l'échelle de la Bourgogne
* Découpage pour le BV de la Sorme et analyse des résultats
* Import des cartes des cumuls moyen des pluies annuelles dans QGIS;

### Étape 4 : Interpolation spatiale basée par régression-krigeage

* Krigeage des résidus
* Régression-Krigeage
* Evaluation de la qualité des trois méthodes d’interpolation : Régression multilinéaire, Krigeage et Régression-Krigeage
* Interpolation des cumuls de pluie annuels moyens de part et d’autre de la rupture 1987/1988.


Nous reviendrons au cours du TP sur les différentes étapes.

