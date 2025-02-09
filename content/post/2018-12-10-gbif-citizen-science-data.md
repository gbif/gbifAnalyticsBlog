---
title: Will citizen science take over? 
author: John Waller
date: '2019-01-21'
slug: gbif-citizen-science-data
categories:
  - GBIF
tags:
  - citizen science
  - rstats
lastmod: '2018-12-10T11:34:10+01:00'
keywords: []
description: ''
comment: no
toc: ''
autoCollapseToc: no
postMetaInFooter: no
hiddenFromHomePage: no
contentCopyright: no
reward: no
mathjax: no
mathjaxEnableSingleDollar: no
mathjaxEnableAutoNumber: no
hideHeaderAndFooter: no
flowchartDiagrams:
  enable: no
  options: ''
sequenceDiagrams:
  enable: no
  options: ''
---

Citizen science is scientific research conducted, in whole or in part, by amateur (or non-professional) scientists. Biodiversity observations by citizen scientists have become significant in the last 10 years thanks to projects like: 

<!--more-->

* [eBird](https://ebird.org/home)
* [iNaturalist](https://www.inaturalist.org/home)
* [Artportalen Sweden](https://www.artportalen.se/)
* [Artsdatabanken Norway](https://www.artsdatabanken.no/)
* [Southern African Bird Atlas](http://sabap2.adu.org.za/)
* [Bird Life Austrailia](https://birdlife.org.au/)
* [Dansk Ornitologisk Forening](http://www.dof.dk/)
* [Great Back Yard Bird Count](http://gbbc.birdcount.org/)

> Citizen science is scientific research conducted, in whole or in part, by amateur (or non-professional) scientists. Citizen science is sometimes described as “public participation in scientific research,” participatory monitoring, and participatory action research (wikipedia).

# The rise of citizen science on the GBIF network

![](/post/2018-12-10-gbif-citizen-science-data_files/growthOfCitizenScienceWeb.jpg)

Citizen scientists have been contributing a large and growing percentage of records to the GBIF network.

# 50% of occurrence records on GBIF are citizen science observations

![](/post/2018-12-10-gbif-citizen-science-data_files/percentageOfGBIFWeb.jpg)

For the last few years, citizen science observations make up around 50% of the biodiversity knowledge on the GBIF network. The [eBird](http://www.birds.cornell.edu/Page.aspx?pid=1478#_ga=2.205672981.721396792.1547556286-1941218201.1542284276) dataset is by far the largest contributor and when this dataset is updated we can see a spike in the percentage graph. In between eBird updates, non-citizen science datasets decrease the percentage. 

# Largest datasets on GBIF are citizen science datasets

![](/post/2018-12-10-gbif-citizen-science-data_files/citizenScienceBarplotWeb.jpg)

**6 of the top 10** datasets on the GBIF network are citizen science datasets. 

# Birds are very popular in citizen science

**617 of the top 800 species** observed by citizen scientists are birds. 

* Top **bird** 1st place (seagull, 8M records)
* Top **insect** 426th place (red admiral butterfly, 200k records)
* Top **mammal** 540th place (row deer, 140k records)
* Top **plant** 645th place (common nettle, 100k records)

Here I plot the top 800 species in citizen science in terms of occurrence count. 

![](/post/2018-12-10-gbif-citizen-science-data_files/top800speciesBarplotWeb.jpg)

[interactive version of graph above](https://jhnwllr.github.io/charts/csPlotTopSpecies.html)

# There are > 8 000 000 seagull occurrence records 

<img src="/post/2018-12-10-gbif-citizen-science-data_files/LarusArgentatus.JPG" alt="roe deer" width="50%">

[*Larus argentatus* subsp. *argenteus*](https://www.gbif.org/occurrence/1913125694) by G.Droege via Botanic Garden and Botanical Museum Berlin-Dahlem. Photo licensed under [CC BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/)

# Top insect is the red admiral butterfly 200k records 

<img src="/post/2018-12-10-gbif-citizen-science-data_files/VanessaAtalanta.JPG" alt="roe deer" width="50%">

[*Vanessa atalanta*](https://www.gbif.org/occurrence/1913125579) by W.-H. Kusber via BoBO - Botanic Garden and Botanical Museum Berlin-Dahlem Observations. Photo licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

# Top mammal is the roe deer 140k records 

<img src="/post/2018-12-10-gbif-citizen-science-data_files/CapreolusCapreolus.JPG" alt="roe deer" width=50%">

[*Capreolus capreolus*](https://www.gbif.org/occurrence/1883110155) by Trine Brevig via the Norwegian Species Observation Service. Photo licensed under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

# Top plant is the common nettle 100k records

<img src="/post/2018-12-10-gbif-citizen-science-data_files/UrticaDioica.jpg" alt="common nettle" width=50%">

[*Urtica dioica* subsp. *dioica*](https://www.gbif.org/occurrence/1802757183) by Peter de Lange via iNaturalist. No copyright.

# Citizen science is less biodiverse than professional science

![](/post/2018-12-10-gbif-citizen-science-data_files/genusCountsCSWeb.jpg)


Here I plot the number of unique genera observed by citizen scientists against those recorded by non-citizen science datasets or likely collected by professional scientists.

>So while citizen science is an important and growing part of biodiversity data, it cannot replace well-curated professional museum collections and other professional sources.
 
While citizen scientists have observed over **50% of GBIF records** (500 Million!), they have **only 20% of the genera** observed by professional scientists (50k out of around 200k genera). **So while citizen science will probably not replace professional science**, it is still and important and growing part of biodiveristy monitoring and data collection. No doubt the biodiversity of citizen science observations will continue to increase as more specialists start using apps like [iNaturalist](https://www.inaturalist.org/home).  Perhaps citizen scientists will observe 60k or 70k genera by the end of 2019, and do it for free! 

# Technical details 

* [Link](https://github.com/jhnwllr/citizen-science) to gitHub with data and R code.  
* [Link](https://data-blog.gbif.org/post/gbif-citizen-science/) to a previous blog post where we describe how we classified citizen science datasets. 
* As of the writing of this blog there are **412 datasets** classified as citizen science on the GBIF network. 

You too can get a list of the citizen science datasets using the gbif api. Paste the following link into a web browser and get a list of citizen science datasets via the GBIF api. 

```
http://api.gbif.org/v1/dataset?machineTagNamespace=citizenScience.mgrosjean.gbif.org&limit=500

```
There is also a static csv table [here](https://github.com/jhnwllr/citizen-science/blob/master/data/citizenScienceTable.csv). 

Do you know a citizen science dataset that is not in the list? Leave a comment. 



<!--more-->
