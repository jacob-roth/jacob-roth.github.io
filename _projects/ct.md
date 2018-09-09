---
title: "CT Image Reconstruction"
collection: projects
permalink: /projects/ct
excerpt: "Efficiently solving ill-conditioned linear systems | [SPIE Proceedings, March 2018](https://doi.org/10.1117/12.2293805)"
date: 2018-03-07
venue: "SPIE Proceedings"
paperurl: "https://doi.org/10.1117/12.2293805"
---
### Overview
We studied and implemented various algorithms for solving systems of equations arising from an ill-posed, linear reconstruction problem.
The forward model $Xf = g$ with forward-projector $X$, object $f$, and (sinogram) data $g$ gave rise to various reconstruction operators $R$, and the main focus of the project was in analyzing the efficiency with which a given $R$ could classify data $g$ as coming from one of two cases.
This could be phrased in a hypothesis testing framework, but the ideal test-statistic would give a (nonlinear) MLE problem to distinguish between signal-positive and signal-negative cases for a particular $R$
As a computationally tractable alternative, we used a (linear) Hotelling observer framework.
This resulted in a linearly constrained QP (where $R$ was not needed explicitly).
However, the problem involved the ill-conditioned (discretized integral) operator $X^T X$, and the resulting KKT system was poorly conditioned.
The ill-conditioning motivated using Tikhonov regularization to approximate the ill-posed problem by a family of well-posed problems, which is where our project began.

### Outcomes
We implemented line search methods (preconditioned CG, quasi-Newton), projection methods (POCS, Douglas-Rachford, [RAAR](https://arxiv.org/abs/math/0405208)), and compared them to MINRES, LSQR, and existing convex solvers (MOSEK, Gurobi).
