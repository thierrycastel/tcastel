---
layout:            post
title:             "UE2 M2SEME: Interpolation spatiale"
date:              2024-09-17 21:00:00 +0300
tags:              GIS
category:          GIS Features
author:            tcastel
math:              true
---


### Analyse données géographiques : Interpolation spatiale

**Objectifs :**

Afin de pouvoir estimer la part de contribution du ruissellement des pluies sur la pollution au phosphore, il est nécessaire de connaître le cumul de précipitations en tout point du bassin versant. Malheureusement, cette information n’est pas mesurée au niveau du bassin versant. Les stations climatiques disponibles sont situées à l’extérieur de ce dernier.

Pour estimer les cumuls de pluie au niveau de bassin versant, et pour tous les pixels du MNT nous allons procéder à l’interpolation spatiale.
L’objet de cette séance est de connaître des techniques communes d’interpolation spatiale des données :

    * La régression multiple
    * Le krigeage ordinaire (technique appartenant à la discipline des géostatistiques)

Vous serez guidés pas à pas pour interpoler les cumuls annuels de pluie avant et après 1987/1988. 

  
### Le support du TP et les données sont à récupérer [ici](https://filesender.renater.fr/?s=download&token=29175ade-96d5-426b-b985-7d865f172689)

### Séance 3 : interpolation mécaniste

* Exploration et mise en forme des données;
* Agrégation des données climatiques au pas de temps annuel;
* Construction du modèle linéaire multiple entre variables explicatives (X, Y et altitude) et la variable climatique (corrélations, partielles ou non) ;
* Mesure de la significative des variables retenues dans le modèle (r, p-value);
* Évaluation de la qualité du modèle (R2 ajusté, RMSE sur les résidus).

### Séance 4 : interpolation géostatistique ([ici](https://filesender.renater.fr/?s=download&token=29175ade-96d5-426b-b985-7d865f172689))


* Régression multilinéaire
* Krigeage des résidus
* Régression-Krigeage
* Evaluation de la qualité des trois méthodes d’interpolation : Régression multilinéaire, Krigeage et Régression-Krigeage
* Interpolation des cumuls de pluie annuels moyens de part et d’autre de la rupture 1987/1988.


### Séance 5 : Cartographie des cumuls moyen des pluies annuelles

* Import des cartes des cumuls moyen des pluies annuelles dans QGIS;
* Calcul du facteur d'érosivité pluviométrique;
* Croisement avec la carte des risques de fuite du phosphore sur le BV;

* Attendu pour l'évaluation de la partie traitement des données de l'[**UE2**]({{ site.baseurl }}{% link /media/M2SEMEvalUE2/TD5-Evaluation_UE2-DonneesSpatiales_M2SEME.pdf %})
* Données pour l'évaluation [**ici**]({{ site.baseurl }}{% link /media/M2SEMEvalUE2/Pour_Etudiants_Evaluation.zip %})


Nous reviendrons au cours du TP sur les différentes étapes.

