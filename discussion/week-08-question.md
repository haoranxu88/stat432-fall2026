---
id: w08-hx27-margin-set-by-four-points
title: "When only four points set the margin, how fragile is the boundary?"
author: "Haoran Xu (hx27)"
---

In Homework 8 Question 2, the geometric margin $M = 1$ was attained by just four
of the 50 observations (two per class), and the other 46 could move freely without
changing the boundary. If one of those four were mislabeled or shifted slightly,
the maximal-margin boundary could change a lot. Does lowering the cost parameter
$C$ fix this by letting more points become support vectors, and is there a rule
of thumb for how many support vectors a well-tuned linear SVM should have
relative to $n$?
