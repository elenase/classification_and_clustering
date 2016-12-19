---
title       : Classification and Clustering
subtitle    : 
author      : Elena Seydel
job         : 
framework   : shower        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

# General Information about Classification and Clustering

> Classification is a major step in creating maps. Behind every classification mechanism (that might be done automatically by most GIS Software) a complex mathematical algorithm is used.


> Regarding to which classification algorithm you choose the product will look totally different as the data breaks between the classes change. To decide which classification is the best you should understand what happens behind.

--- 

## Understanding Classification in ArcGIS

[Explanation of automated classification methods in ArcGIS](https://pro.arcgis.com/en/pro-app/help/mapping/symbols-and-styles/data-classification-methods.htm)

--- 


## Classification and Clustering

Clustering:
Classification:

>In general there are two major classification and clustering methodologies:
1. Supervised Classification
2. Unsupervised Classification


--- 

## Unsupervised Classification Algorithms 

> Explanation

[Clustering: Basics](https://www.youtube.com/watch?v=6R16reLVl3I)



--- 

# Unsupervised Classification Algorithms

[K-Means](https://www.youtube.com/watch?v=_aWzGGNrcic)


    + PRO: Entire feature space can be classified
    + CONTRA: Description of cluster determined by radial shape, starting points must be selected as cluster center

--- 

## Hierarchical Clustering

[Hierarchical Clustering](https://www.youtube.com/watch?v=OcoE7JlbXvY)
Hierarchical clustering creates a [Dendrogram](http://www.ncss.com/wp-content/themes/ncss/pdf/Procedures/NCSS/Hierarchical_Clustering-Dendrograms.pdf) which is a tree diagram. It shows the euklidian distance between data points. The Dendrogram can be used to decide how many clusters you want to create. You can choose between different possibilities to define the distance between clusters:

      + Single link = Minimal euklidian distance
      + Average link = Average euklidian distance
      + Complete link = Maximum euklidian distance

--- 

## Mixture of Gaussian

[Mixture of Gaussian](https://www.youtube.com/watch?v=qMTuMa86NzU)
  
  
--- 

# Supervised Classification Algorithms

> Explanation

--- 

## Naive Bayes

[Naive Bayes](https://www.youtube.com/watch?v=OqmJhPQYRc8)
PROBLEM: Classes often overlap
IDEA of Naive Bayes Theorem: Probability maximisation of correct classification of each data point
GIVEN PARAMETER:

    + A-priori probability that each data point is realated to a specific class 
    + Feature probability that one data point within a specific class has a specific feature vector
    

---

## Maximum Likelihood

  * [Maximum Likelihood Classification: Used if a-priori probability isn't given](https://www.youtube.com/watch?v=RPtYRm2tboA)

---


## K-nn

[K-nn = K-nearest neighbor](https://www.youtube.com/watch?v=k_7gMp5wh5A)

A [Voronoi Diagramm](http://www.pi6.fernuni-hagen.de/downloads/publ/tr198.pdf) decribes areas, that are nearest to a certain data point (within a defined distance)
1. For the k-nn classification you choose an uneven number of neighbors=k
2. The algorithm starts at a random point
3. This starting point gets the value that most appears in the "neighborhood" (for that reason k should always be uneven)


    + PRO: Easy concept
    + CONTRA: Distance parameter often difficult

---

## Support Vector Machines (SVM)

[Support Vektor Machines (SVM)](https://www.youtube.com/watch?v=1NxnPkZM9bc)

    + PRO: Unlinear classification possible, less parameter required, no a-priori knowledge required, applicable for large feature space
    + CONTRA: Slow classification 

---

## Support Vector Machines (SVM)

[AdaBoost](https://www.youtube.com/watch?v=ix6IvwbVpw0)
is a combination of multiple weak classifiers to build one strong classifier

---


