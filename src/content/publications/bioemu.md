---
title: 'bioemu'
---

During my Microsoft internship, I worked with Frank Noe on a protein structure SE(3) diffusion model called BioEmu for sampling protein dynamics. Protein (or molecular) dynamics in simple terms is simulating how proteins move and interact with other molecules to understand their functions. The main idea of BioEmu is to investigate data scaling by first pre-train on publicly available protein structure datasets and then fine-tune on protein dynamics data, both public and in-house generated with large scale compute from Microsoft Azure. The goal is to learn a distribution that samples proportionally to the equilibrium distribution, i.e. sampling proportionally to the amount of time a protein is in a certain pose. BioEmu achieved state-of-the-art performance on capturing the equilibrium distribution of out-of-distribution proteins. If molecular dynamics can scale and generalize to new proteins, then lots of new therapeutic would become possible to develop.

