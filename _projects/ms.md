---
title: "MS Project"
collection: projects
permalink: /projects/ms
excerpt: "Distributionally Robust Chance-Constrained Optimization"
date: 2018-08-23
venue: "UChicago"
paperurl: "https://jacob-roth.github.io/files/mspaper.pdf"
---
### Overview
For my independent project, I worked with Professor Mihai Anitescu on optimization approaches to decision making under uncertainty.
We studied a distributionally robust chance-constrained (DRCC) framework and contextualized it with two well-known optimization paradigms: (1) robust optimization and (2) stochastic optimization (SO).
The project was motivated by a semi-infinite problem with a PDE constraints.
Instead of enforcing the constraint in its original form, we took a probabilistic approach and required it to hold with high probability based on the empirical distribution of the control variables.
We
 1. applied this approach to a linear toy problem and solved it analytically
 2. studied various constraint relaxations in preparation for scaling up to a more realistic model.

### Outcomes
For (1), we were able to obtain a representation of the optimum that then allowed us to study and identify the most adverse distribution for the problem.
For (2), we discretized the semi-infinite chance-constraint, then applied a convex relaxation based on Nemirovski & Shapiro’s CVaR approach, and ultimately analyzed the impact of each relaxation.
Our findings suggested that that the convex relaxation contributed most significantly to the optimality gap. It was rewarding to answer concrete questions that drew on both both mathematical and computational approaches.
