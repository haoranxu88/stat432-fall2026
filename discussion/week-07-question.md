---
id: w07-hx27-when-to-prefer-qda
title: "Can we tell from the training data alone whether QDA is worth it?"
author: "Haoran Xu (hx27)"
---

In Homework 7 Question 3, LDA's test error stayed near $0.17$ for every $\rho$
while QDA's dropped from $0.20$ to $0.10$ as the two class covariances grew
apart. Is there a simple check on the training data, such as comparing the
estimated class covariance matrices, that tells us when to prefer QDA over LDA
without running cross-validation on both?
