---
title: "CT Image Reconstruction"
collection: projects
permalink: /projects/ct
excerpt: "Efficiently solving ill-conditioned linear systems"
date: "Summer 2017"
venue: "SPIE"
paperurl: "https://doi.org/10.1117/12.2293805"
---
We studied and implemented various algorithms for solving systems of equations arising from an ill-posed, linear reconstruction problem.
The forward model $Xf = g$ with forward-projector $X$, object $f$, and (sinogram) data $g$ gave rise to various reconstruction operators $R$, and the main focus of the project was in analyzing the efficiency with which a given $R$ could classify data $g$ as coming from one of two cases.
Naturally, this could be phrased in a hypothesis testing framework.
The ideal test-statistic would give a (nonlinear) MLE problem to optimize the parameters of the likelihood model to distinguish between signal-positive and signal-negative cases for a particular $R$, but as a computationally tractable model, we used a (linear) Hotelling observer framework.
This resulted in its own optimization problem, which a colleague formulated as a linearly constrained QP (where we didn't need to have $R$ in explicit form).
However, the problem implicitly involved the ill-conditioned (approximate/discretized integral) operator $X^T X$, and the resulting KKT system was poorly conditioned.
The ill-conditioning motivated using some form of regularization to approximate the ill-posed problem by a family of well-posed problems, which is where our project began.
