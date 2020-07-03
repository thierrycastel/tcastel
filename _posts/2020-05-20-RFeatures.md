---
layout:            post
title:             "R climate data practices"
tags:              Read ascii data from Drias site
category:          Code Features
author:            tcastel
math:              true
---
Comment récupérer et lire des données climatiques issues du site de service climatique [Drias](http://www.drias-climat.fr/) de Météo-France. Au préalable il faut ouvrir un compte (gratuit) pour accéder aux données librement. Les détails de l'utilisation seront vus en séance de TP.

Pour rappel :
<ul>
<li>avec R les # permettent de mettre des commentaires dans le code</li>
<li>Pour l'assignement dans un objet on peut utiliser <- ou =</li>
<li>Parmis les fonctions très utiles pour explorer les données : class, str, dim, head, tail</li>
</ul>


```python
## file data from drias : 'tasmintasmaxrstr_metro_CNRM_Aladin_histo_QT_REF_19750101-20051231_1810161527930443.KEYu11UB3Ax3u02D2uxu0D0.zip'
## unzip produces the file : 'tasmintasmaxrstr_metro_CNRM_Aladin_histo_QT_REF_19750101-20051231.txt'
## skip value is estimate by counting header lines up to the data
mydrias <- read.csv("tasmintasmaxrstr_metro_CNRM_Aladin_histo_QT_REF_19750101-20051231.txt", header = FALSE, skip=53)
```

```python
colnames(mydrias) <- c("date","idpt","lat","lon","alti","Tn","Tx","RR") 
## A adapter en fonction de l'ordre que vous avez précisé lors de l'extration des données sur le site Drias
head(mydrias)
```

<table>
<caption>A data.frame: 6 × 8</caption>
<thead>
	<tr><th></th><th scope="col">date</th><th scope="col">idpt</th><th scope="col">lat</th><th scope="col">lon</th><th scope="col">alti</th><th scope="col">Tn</th><th scope="col">Tx</th><th scope="col">RR</th></tr>
	<tr><th></th><th scope="col">&lt;chr&gt;</th><th scope="col">&lt;int&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;int&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;dbl&gt;</th></tr>
</thead>
<tbody>
	<tr><th scope="row">1</th><td>01/01/1975</td><td>9378</td><td>46.2218</td><td>3.94455</td><td>302</td><td> 0.2</td><td> 7.3</td><td>3.58</td></tr>
	<tr><th scope="row">2</th><td>01/02/1975</td><td>9378</td><td>46.2218</td><td>3.94455</td><td>302</td><td> 6.4</td><td> 7.5</td><td>0.00</td></tr>
	<tr><th scope="row">3</th><td>01/03/1975</td><td>9378</td><td>46.2218</td><td>3.94455</td><td>302</td><td> 0.5</td><td> 8.3</td><td>0.00</td></tr>
	<tr><th scope="row">4</th><td>01/04/1975</td><td>9378</td><td>46.2218</td><td>3.94455</td><td>302</td><td> 1.6</td><td> 3.8</td><td>1.00</td></tr>
	<tr><th scope="row">5</th><td>01/05/1975</td><td>9378</td><td>46.2218</td><td>3.94455</td><td>302</td><td>-0.3</td><td> 1.5</td><td>0.13</td></tr>
	<tr><th scope="row">6</th><td>01/06/1975</td><td>9378</td><td>46.2218</td><td>3.94455</td><td>302</td><td> 0.8</td><td>-0.6</td><td>0.51</td></tr>
</tbody>
</table>

```python
hist(mydrias$Tn)
```

![png]({{ site.baseurl }}{{"/jupyter/output.png"}}){: .center-image }

```python

```
