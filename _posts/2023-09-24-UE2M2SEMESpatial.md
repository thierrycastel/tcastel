---
layout:            post
title:             "UE2 M2SEME: analyse spatiale avec QGIS"
date:              2023-09-24 18:30:00 +0300
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

  
### Le support du TP et les données sont à récupérer [ici](https://filesender.renater.fr/?s=download&token=8a8583c3-ee88-45cb-89cc-423c8d4eb1ca)

### Séance 3 : interpolation mécaniste

* Exploration et mise en forme des données;
* Agrégation des données climatiques au pas de temps annuel;
* Construction du modèle linéaire multiple entre variables explicatives (X, Y et altitude) et la variable climatique (corrélations, partielles ou non) ;
* Mesure de la significative des variables retenues dans le modèle (r, p-value);
* Évaluation de la qualité du modèle (R2 ajusté, RMSE sur les résidus).

### Séance 4 : interpolation géostatistique (à venir)


Nous reviendrons au cours du TP sur les différentes étapes.


