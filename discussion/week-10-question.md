---
id: w10-hx27-mtry-one-wins-on-pca-scores
title: "Why did mtry = 1 win on PCA scores when it was the worst setting in the simulation?"
author: "Haoran Xu (hx27)"
---

In Homework 10, `mtry = 1` had the largest squared bias in the five-predictor
simulation, yet on the MNIST principal components the OOB error rose steadily
with `mtry`, from about 2% at `mtry = 1` to about 5% at `mtry = 20`. My guess is
that with a few dominant, uncorrelated components a large `mtry` makes every
tree split on PC1 and PC2 at the same places. Is the rule that `mtry` should be
small whenever a few strong predictors dominate, and since `mtry = 1` sat on the
edge of my grid, can OOB error alone tell us when the trees have become too random?
