---
title: "CT Image Reconstruction"
collection: projects
permalink: /projects/ct
excerpt: "Efficiently solving ill-conditioned linear systems"
date: 2018-03-07
venue: "SPIE Proceedings"
paperurl: ""
---
### Overview
The goal of the project was to use signal detectability metrics to analyze how effectively a reconstruction operator $R$ could classify observational data into one of two classes.
We studied a discretized system which gave rise to a forward model $Xf = g$ with forward-projector $X$, object $f$, (sinogram) data $g$, and reconstruction operators $R$ (s.t. $Rg \approx f$).
This could be phrased in a hypothesis testing framework, but the ideal test-statistic would give a (nonlinear) MLE problem to distinguish between signal-positive and signal-negative cases for a particular $R$.
In this formulation, the primary bottleneck was storing and working with $X$ (and therefore $R$) explicitly since $X$ could have $100,000$ rows/columns.

### Outcomes
For smaller toy problems, we implemented line search methods (preconditioned CG, quasi-Newton), projection methods (POCS, Douglas-Rachford, [RAAR](https://arxiv.org/abs/math/0405208)), and compared them to MINRES, LSQR, and existing convex solvers (MOSEK, Gurobi).
For the larger problem, we considered a formulation which represented $R$ implicitly and avoided expensive storage of $R$.
This resulted in a large, convex (but poorly-conditioned) linearly constrained QP that we were able to solve iteratively with MINRES.

[Download](https://jacob-roth.github.io/files/spie.pdf)
