---
title: 'RFdiffusion2'
---

RFdiffusion works for many cases but struggles with enzyme design. Enzymes require atomistic precision to achieve a desired reaction. We extended RFdiffusion with a atomistic representation and my SE(3) flow matching model to achieve atomistic precision when designing enzymes. We developed a novel conditioning approach that separates the design problem into designing the catalytic residues and the scaffold separately but conditioning the diffusion to make sure the catalytic residues and scaffold are compatible. The new model, RFdiffusion2, achieved state-of-the-art results on computational benchmarks for enzyme design and is used inside David Baker's lab for designing novel enzymes. *De novo* enzyme design can unlock new chemical reactions not possible through traditional methods such as plastic degradation and new therapeutics.


