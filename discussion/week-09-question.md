---
id: w09-hx27-radial-kernel-that-acts-linear
title: "If the winning radial kernel is almost linear, is it really the better model?"
author: "Haoran Xu (hx27)"
---

In Homework 9 Question 1, the radial kernel with a tiny $\gamma = 0.01$ had the
lowest CV error on the SAheart data, yet it behaved almost identically to the
linear kernel, while $\gamma = 1$ collapsed to predicting the majority class at
every cost $C$. When a flexible kernel wins only by imitating a linear one, and
the gap is within one standard error, should we still prefer it on predictive
grounds, or does the bias-variance picture say the linear SVM is the
better-supported choice?
