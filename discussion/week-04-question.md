---
id: w04-hx27-lasso-duplicate-predictors
title: "Lasso selection with near-duplicate predictors"
author: "Haoran Xu (hx27)"
---

If two standardized predictors are exact copies, $x_1 = x_2$, then any same-sign
coefficients with $\beta_1 + \beta_2 = c$ give the same fit and the same lasso
penalty $\lambda|c|$, so the lasso cannot tell $(c, 0)$ from $(0, c)$. Ridge
breaks the tie, because $\beta_1^2 + \beta_2^2$ is smallest at the even split.

At correlation $0.99$ the lasso solution is unique again, but which variable
enters seems to be decided by sampling noise: a different sample or a nearby
$\lambda$ can swap $x_1$ for $x_2$ while test error barely moves.

If prediction is stable and selection is not, is "the lasso chose $x_1$" a
finding about $x_1$ at all? Should we instead report selection frequencies
across bootstrap samples, or use the elastic net so the correlated pair enters
together?
