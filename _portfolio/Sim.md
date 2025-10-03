---
title: "Testing in sim: Failure discovery with sampling-based techniques "
excerpt: "Improving the efficiency of sampling based evaluation using data-driven techniques<br/><img src='/images/sim_only_1.png' width="50%">"
collection: portfolio
---
[Project Website](https://mit-realm.github.io/neural-langevin-website/)
[Conference Paper/Letters](/publication/ICRA_2025)
[Journal Paper (related project)](/publication/TRO_2025)

Sampling methods are inefficient in high-dimensional and low volume exploration. Using a data-driven model to predict failures will only return failures that are observed in training data. Using such models as a pre-processing step, and combining with sampling methods allows generalizability beyond training data due to exploration and mitigates the drawbacks of sampling methods.

## Neural Projection Operator (NPO) for low volume exploration for finding obstacles for collision
We consider falsification of MPPI by placing obstacles on Autorally racetrack for collisions. The track is a region of low volume, but the boundary for the track can be learnt easily using synthetically generated data. We use a NPO to project samples within the track, and apply 2nd order Langevin to generate obstacles for failure. 
<img src='/images/npo.png'>

Examples of obstacle locations observed using our method tested on the track
<img src='/images/autorally.png'>

## VAE for low dimensional latent space exploration to generate failure trajectories
We use a VAE to learn a nominal low-dimensional representation of trajectories, and sample falsifying trajectories in the learnt stationary latent space to falsify LQR trajectory tracking controller on F1-Tenth. 
<img src='/images/vae.png'>

Using sampling allows us to go beyond what we have observed in training data and discover newer failures.
<img src='/images/sim_only_vae.png'>

