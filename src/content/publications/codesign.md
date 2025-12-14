---
title: 'Codesign'
---

We sought to extend flow matching to discrete state spaces. The theory and construction of discrete flows simplifies discrete diffusion which allows for greater flexibility in probability paths, sampling, and target/source couplings. [Gat et al.](https://arxiv.org/abs/2407.15595) extended our work by scaling it to larger models, experimenting on more domains (coding, images), and developing more extensions. (In retrospect we should've called our method discrete flow matching 🥲.)

Next, we combined discrete and Riemannian flow matching into a multimodal diffusion model called Multiflow for jointly generating protein sequence (tokens) and structure (SE(3)). We achieved state-of-the-art results at the time for protein generation. We briefly investigated co-dependency and mutual information properties between the discrete and continuous flows. There is still a lot to understand in multimodal generation.
