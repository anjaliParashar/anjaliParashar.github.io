---
title: "Testing in real: Sample-efficient failure discovery of contextual failures with Bayesian active learning "
excerpt: "Discovering failures that cannot be expressed analytically, in limited samples, using coverage-driven active learning<br/><img src='/images/BED_corl.png width="50%"'>"
collection: portfolio
---
[Project Website](https://mit-realm.github.io/contextual-website/)
Experts can participate in root-cause analysis of failures by observing failures and providing possible failure modes. 
<img src='/images/expert.png'>

In this work, we look at how we can combine expert-driven analysis for a multi-modal failure discovery in real-world platforms. Our pipeline consists of learning expert based feedback using GPs as surrogate models, and coverage-based active learning strategy called Expected Coverage Improvement (ECI) for limited data evaluation. 
<img src='/images/BED_corl.png'>

By balancing coverage with failure discovery in targeted regions we are performing efficient exploration with ECI. An example of what different techniques (optimization, ECI, and random walk) look like in a 2D search space for Push-T task in sim.
<img src='/images/example_pushT_corl.png'>

