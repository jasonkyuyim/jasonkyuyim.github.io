---
title: 'GGS'
---

We started off wanting to do reinforcement learning (RL) for protein sequence optimization but it turned into a big benchmarking project of 7 different methods after we found serious flaws in the previous benchmarks: sometimes the test examples were 99% similar to examples in train. We constructed a new de-leaked benchmark and evaluated each method.
We observed that each method had merits but the real issue was the noisy predictions of the reward model. We explored different regularization strategies and found minimizing the total variation (i.e. increasing the smoothness) ([Zhou et al.](https://dennyzhou.github.io/papers/RFLG.pdf)) could greatly improve test performance.
We also found a very simple approach of using Gibbs With Gradients ([Grathwohl et al.](https://arxiv.org/abs/2102.04509)) with a good reward model would outperform all the more complicated methods using RL, GFlowNets, LLMs, etc. The takeaway? A good reward model is all you need.

