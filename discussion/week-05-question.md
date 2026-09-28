---
id: w05-hx27-knn-duplicate-predictors
title: "Does a duplicated predictor count twice in KNN?"
author: "Haoran Xu (hx27)"
---

If I copy one predictor so that it appears twice, $x_2 = x_1$, its squared
difference enters the Euclidean distance twice:
$d^2 = 2(x_{01} - x_{i1})^2 + \sum_{j \ge 3}(x_{0j} - x_{ij})^2$. KNN then
treats $x_1$ as twice as important, even though no information was added. In
linear regression a duplicate column does not change the fitted values at all.

The same thing happens less visibly with strongly correlated predictors: a
group of them acts like one variable with a large weight in the distance.

Should we remove or down-weight strongly correlated predictors before running
KNN? And how would we choose the weights without looking at the response?
