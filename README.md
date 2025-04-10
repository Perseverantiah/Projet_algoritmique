# Projet d’algorithmique – Problème du sac à dos 
Auteur : Ninette Hounkponou, Alexandre Colombeau, Mohtadi HAMMAMI

Ce projet a été réalisé dans le cadre du cours d’algorithmique de M2DS.

Nous étudions ici le **problème classique du sac à dos **, en proposant **trois approches algorithmiques différentes**, implémentées à la fois en **C++** et en **R** dans le but de comparer leur **efficacité computationnelle selon le langage** utilisé.

---

## 📌 Objectifs

- Implémenter plusieurs stratégies pour résoudre le problème du sac à dos :
  - méthode **naive** (parcours exhaustif)
  - méthode **gloutonne** (heuristique)
  - méthode par **programmation dynamique** (optimisation)
- Comparer les **temps d'exécution** selon la **taille des données** et le **langage** utilisé (C++ vs R)
- Observer les compromis entre **temps de calcul**, **qualité de la solution**, et **complexité algorithmique**

---

## Quick Start
Conditions préalables au développement du paquet
Pour développer et utiliser le paquet, installez les dépendances nécessaires :

``` install.packages(c("Rcpp", "RcppArmadillo", "devtools", "roxygen2", "testthat"))```

** NB : Il faut que vous ayez la derniere version de Rcpp **

## Pour installer le package depuis GitHub
``` devtools::install_github("Perseverantiah/Projet_algoritmique")```

Pour pouvoir l'utiliser :

``` library(knapsack2)```


## [Exemples ](#-exemples)
### Algo naive


## Exemple

```{r exemple_naif}
set.seed(42)
n = 10
poids <- sample(10,n)
valeur <- sample(30,n)
poids_max <- 20
sac_a_dos(poids, valeur, poids_max)
```

```
$combinaison
 [1] 1 1 0 0 1 0 0 1 0 1

$poids_total
[1] 20

$valeur_totale
[1] 114

```

### Algo glouton


```{r exemple_glouton}
set.seed(42)
n = 100000
poids <- sample(n)
valeur <- sample(n)
poids_max <- 20
sac_a_dos_glouton(poids, valeur, poids_max)
```

```
$poids_total
[1] 19

$valeur_totale
[1] 306440
```
### Algo dynamique
