---
title: 'LSD'
---

Latent diffusion excels at capturing semantically rich features in the latent space then uses a powerful decoder to generate data conditioned on the latent. We sought to learn a semantically rich latent space of protein topologies then train a hierarchical two-stage diffusion model. First, latent diffusion generates a protein topology. Second, conditioned on the sampled latent, structure diffusion generates the protein structure that adheres to the topology. We found reward optimization to be effective in this framework by doing the guidance in the latent space first then generating diverse protein structures conditioned on the latents. This approach was a proof of concept of how reward guidance could more effective in the latent rather than ambient space. Unfortunately I did not see this project to completion before graduating.
