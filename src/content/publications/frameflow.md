---
title: 'frameflow'
---


This work was an continuation of my SE(3) diffusion model where I extended Riemannian flow matching ([Chen et al.](https://arxiv.org/abs/2302.03660)) to SE(3). As expected, the theory and methodology were much simpler than Riemannian diffusion. My co-authors fixed some numerical instability with exponential and logarithmic maps that greatly improved training stability. Concurrent works ([Bose et al.](https://arxiv.org/abs/2310.02391), [Ajay et al.](https://arxiv.org/abs/2211.15657)) demonstrated a low-tempearture sampling trick by scaling the vector field during reverse integration that we also found to improve performance.
We applied the model to a protein inpainting task called motif-scaffolding and demonstrated state-of-the-art results. We investigated guided sampling with twised sequential monte carlo ([Wu et al.](https://arxiv.org/abs/2306.17775)) but found this did not work well without a large number of particles.
