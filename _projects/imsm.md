---
title: "* Coastal Engineering"
collection: projects
permalink: /projects/ce
excerpt: "  * Exploring empirically-driven surrogate models ~ [SAMSI Workshop, July 2018](https://www.samsi.info/programs-and-activities/2017-2018-education-and-outreach-programs-and-workshops/2018-industrial-math-stat-modeling-workshop-for-graduate-students-july-15-25-2018/)"
date: 2018-03-07
venue: "IMSM"
paperurl: "https://www.samsi.info/programs-and-activities/2017-2018-education-and-outreach-programs-and-workshops/2018-industrial-math-stat-modeling-workshop-for-graduate-students-july-15-25-2018/"
---
### Overview
During an industrial math modeling workshop, we focused on a problem from coastal engineering.
Our goal was to efficiently and robustly estimate near-shore hydrodynamics (wave breaking: height, period, direction, and location) given off-shore conditions, and we sought an inexpensive, parametric model which could compete with computationally intensive physical simulation models.
To simulate wave dynamics, we built a simplified (linear) physical model for our baseline.
The physical model allowed us to generate a low-fidelity dataset of near-shore estimated conditions from historical off-shore conditions.
After validating the physical model against historical near-shore conditions, we built a synthetic dataset covering the off-shore condition parameter space and used this data to build empirical regression models (SVR, NNs) for approximating the physical dynamics.

### Outcomes
We observed that the regression techniques were able to map off-shore conditions to map our physical model's near-shore conditions.
As a next step, we proposed introducing probabilistic estimates through using Gaussian Process sampling and stochastic simulation to quantify the effect of off-shore parameter uncertainty.

* test
    * test
