---
title: "Testing with Sim and Real: Failure prediction using both sources"
excerpt: "Combining sample-extensive failure search in sim and sample efficient exploration in real-world platform for model validation<br/><img src='/images/overview.png'>"
collection: portfolio
---
[Project Website](https://mit-realm.github.io/few-demo/)

Sim to real gap leads to failures that cannot be discovered by extensive sampling based techniques alone. Here, we investigate combination of sampling methods and active learning with Gaussian processes (GPs) to learn failure prediction models. 
<img src='/images/sim_and_real_T.png'>

We first sample failures using MC sampling in simulation, and learn the boundary between fail and safe using a Normalizing Flows based classification. This is followed by a projection in the latent space to sample exclusively from predicted 'safe' regions in sim. This is our testbed for failures in real system.
<img src='/images/flow_gmm.png'>

We use Gaussian Processes, while collecting data sequentially from the 'safe' region in sim, and optimizing a coverage metric to validate safety of real-world system.
<img src='/images/BED_allerton.png'>

Our method enables efficient discovery of failures that cannot be observed in sim
<img src='/images/failure_T.png'>