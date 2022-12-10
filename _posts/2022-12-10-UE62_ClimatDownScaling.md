---
layout:            post
title:             "M2SEME UE6.2"
tag:         Downscaling climatique statistique
category:          Climate Downscaling
author:            tcastel
---


## UE6.2 Downscaling Climatique Statistique

Après avoir présenté les principes de la désagrégation climatique dynamique et statistique nous appliquerons la méthode de descente d'échelle statistique Quantile Mapping. Nous mobiliserons cette méthode pour désagréger les simulations climatiques globales CMIP6. Le projet d’inter-comparaison de modèles couplés (CMIP) s’est développé sous l’égide du Programme mondial de recherche sur le climat. Ces données mobilisées dans le cadre des rapports du GIEC par la communauté internationale sont accessibles via divers portails de service climatique. Nous mobiliserons le portail Européen [**Climate4Impact**](https://climate4impact.eu/impactportal/data/esgfsearch.jsp#) pour récupérer ces données climatiques. Nous reviendrons sur la récupération des données au cours de la première séance.

Les scripts, les données des stations Météo-France et un article dec présentation de la méthode de downscaling sont à récupérer [**ici**](https://filesender.renater.fr/?s=download&token=4957dec7-2207-46f7-8454-22eea557096f)

Le travail se découpe en 5 principales étapes :

### 1-Récupération et post-traitement des données de Tn, Tx et Pluie de CMIP6 et des stations Météo-France
La descente d'échelle et le débiaisage des données se fera sur la région Bourgogne Franche-Comté

Pour la lecture et la récupération des données CMIP6 nous utiliserons le package R : **ncdf4**

Les étapes de cette partie sont illustrées pour la température minimale Tn et sont présentées sur le [**Notebook_CMIP6**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE62/UE62_readCMIP6.ipynb)

### 2-Ajustement et application des fonctions de transfert par percentile

Nous utiliserons le package R : **qmap** qui implémente la méthode du Quantile Mapping

Les étapes de cette partie sont illustrées pour la température minimale Tn et sont présentées sur le [**Notebook QMapping**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE62/UE62_QMappingCMIP6.ipynb)

### 3-Récupération et post-traitement des données projetées CMIP6 SSP585

Les étapes de cette partie sont illustrées pour la température minimale Tn et sont présentées sur le [**Notebook CMIP6SSP**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE62/UE62_readSSPCMIP6.ipynb)

### 4-Application du modèle de Quantile-Mapping ajusté pour les données projetées

Les étapes de cette partie sont illustrées pour la température minimale Tn et sont présentées sur le [**Notebook_QMappingSSP**](https://github.com/thierrycastel/tcnotebook/blob/master/M2SEME_UE62/UE62_QMapping_CMIP6SSP.ipynb)

### 5-Quelle évolution des températures et des pluies pour la région BFC à l'horizon 2100 ?

Après application de la méthode vous évaluerez quelles évolutions des températures et des pluies sont projetées pour la région BFC. Vous regarderez cela pour la trajectoire SSP585 et SSP245.
