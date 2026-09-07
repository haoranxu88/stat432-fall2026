---
id: w02-hx27-aic-bic-disagreement
title: "When AIC and BIC disagree, which should we trust?"
author: "Haoran Xu (hx27)"
---

AIC penalizes each extra parameter by $2$ and BIC by $\log(n)$, so BIC usually
prefers smaller models. On a borderline predictor the two can select differently.
Which should we follow, and does the answer depend on whether our goal is
prediction accuracy or identifying the true model?
