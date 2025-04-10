# Projet d’algorithmique – Problème du sac à dos 
Auteur : Ninette Hounkponou, Alexandre Colombeau, Mohtadi HAMMAMI

Ce projet a été réalisé dans le cadre du cours d’algorithmique de M2DS.

Nous étudions ici le **problème classique du sac à dos **, en proposant **trois approches algorithmiques différentes**, implémentées à la fois en **C++** et en **R** dans le but de comparer leur **efficacité computationnelle selon le langage** utilisé.

---

## 📌 Objectifs

- Implémenter plusieurs stratégies pour résoudre le problème du sac à dos :
  - méthode **naïve** (parcours exhaustif)
  - méthode **gloutonne** (heuristique)
  - méthode par **programmation dynamique** (optimisation)
- Comparer les **temps d'exécution** selon la **taille des données** et le **langage** utilisé (C++ vs R)
- Observer les compromis entre **temps de calcul**, **qualité de la solution**, et **complexité algorithmique**

---

## Quick Start
Conditions préalables au développement du paquet
Pour développer et utiliser le paquet, installez les dépendances nécessaires :

install.packages(c("Rcpp", "RcppArmadillo", "devtools", "roxygen2", "testthat"))

** NB : Il faut que vous ayez la derniere version de Rcpp **

## Pour installer le package depuis GitHub
devtools::install_github("Perseverantiah/Projet_algoritmique")

Pour pouvoir l'utiliser :

library(knapsack2)


## [Exemples ](#-exemples)
### Algo naive

### Algo glouton

### Algo dynamique
