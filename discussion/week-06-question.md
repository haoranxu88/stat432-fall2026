---
id: w06-hx27-crossing-roc-curves
title: "Comparing models when ROC curves cross"
author: "Haoran Xu (hx27)"
---

In my Homework 6 Question 1, the KNN ($k=45$) and logistic regression ROC
curves cross: KNN is higher at false positive rates below about $0.05$, logistic
catches up above that, and their AUCs differ by only $0.004$. If a cancer screen
will only ever operate at low false positive rates, should we compare partial
AUC over that range (or sensitivity at a fixed specificity) instead of total
AUC, and how do we choose that range before looking at the test data?
