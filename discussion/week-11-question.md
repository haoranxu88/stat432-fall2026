---
id: w11-hx27-binary-flags-after-standardizing
title: "After standardizing, do 0/1 variables get too much say in what 'close' means?"
author: "Haoran Xu (hx27)"
---

In Homework 11 Question 3, standardizing `mtcars` gave the binary flags `am` and
`vs` the same variance as `disp` and `hp`, so two cars that differ only in
transmission sit about two units apart, as far as a 250 cubic inch gap in
displacement, and my four-cluster solution split almost perfectly along those
two flags. When a few binary variables can dominate Euclidean distance this
way, is standardizing still the right default, or should we downweight them or
switch to a distance built for mixed data such as Gower's?
