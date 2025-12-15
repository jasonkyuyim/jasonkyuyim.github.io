---
title: 'framediff'
---

I wanted to develop a generative model over AlphaFold's SE(3) protein representation with the goal of enabling structure-based protein design with generative models. I collaborated with the authors of Riemannian score matching ([Bortoli et al.](https://arxiv.org/abs/2202.02763)) to extend their theory to SE(3) then developed a modified version of AlphaFold's SE(3)-invariant attention-based neural network for SE(3) diffusion. We introduced a widely used benchmark that measured generation quality, diversity, and novelty to assess protein structure generation. This work was used as the foundation of RFdiffusion (see below) in collaboration with David Baker.
