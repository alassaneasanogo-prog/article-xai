# Explicabilité en Intelligence Artificielle (XAI)
## 📑 Table des matières

- [Introduction](#1-introduction)
- [Problématique](#2-problématique)
- [Méthodes d’explicabilité](#3-méthodes-dexplicabilité)
  - [Valeurs de Shapley](#31-valeurs-de-shapley)
  - [Méthodes de gradient](#32-méthodes-de-gradient)
  - [Méthodes de visualisation](#33-méthodes-de-visualisation)
- [Analyse](#4-analyse)
- [Conclusion](#5-conclusion)
## Résumé

L’intelligence artificielle est de plus en plus utilisée dans des domaines critiques comme la santé et la finance. Cependant, les modèles complexes sont souvent difficiles à comprendre. Cet article présente les principales méthodes d’explicabilité ainsi que leurs avantages et limites.

---

## 1. Introduction

Les modèles d’intelligence artificielle modernes, notamment les réseaux de neurones, offrent de très bonnes performances. Cependant, ils sont souvent considérés comme des "boîtes noires", ce qui rend leurs décisions difficiles à interpréter.

---

## 2. Problématique

Comment expliquer les décisions prises par un modèle complexe ?

Cette question est essentielle pour :

* comprendre les prédictions
* détecter les erreurs
* renforcer la confiance des utilisateurs

---

## 3. Méthodes d’explicabilité

### 3.1 Valeurs de Shapley

Les valeurs de Shapley permettent de mesurer la contribution de chaque variable dans une prédiction.

$$
\phi_i = \sum_{S \subseteq N \setminus {i}} \frac{|S|!(n-|S|-1)!}{n!} [f(S \cup {i}) - f(S)]
$$

---

### 3.2 Méthodes de gradient

Ces méthodes mesurent l’importance d’une variable en calculant la dérivée de la sortie par rapport à cette variable.

$$
\frac{\partial f(x)}{\partial x_i}
$$

---

### 3.3 Méthodes de visualisation

Elles permettent d’identifier les zones importantes dans les données, notamment pour les images.

---

## 4. Analyse

### Avantages

* Meilleure compréhension des modèles
* Augmentation de la confiance
* Détection des biais

### Limites

* Coût de calcul élevé
* Difficulté d’interprétation
* Certaines méthodes sont approximatives

---

## 5. Conclusion

L’explicabilité est un élément clé pour une utilisation responsable de l’intelligence artificielle. Cependant, aucune méthode n’est parfaite et un compromis est nécessaire entre performance et interprétabilité.

---

## 6. Références

* Lundberg & Lee (2017) - SHAP
* Goodfellow et al. - Deep Learning
* https://christophm.github.io/interpretable-ml-book
* http://lineardigressions.com/episodes/2018/5/13/shap-shapley-values-in-machine-learning
* https://github.com/shap/shap
