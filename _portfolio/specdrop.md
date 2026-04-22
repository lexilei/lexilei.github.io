---
title: "SpecDrop: Modular Specialization via Category-Conditioned Dropout"
excerpt: "Repurposing dropout as a module-level signal to drive specialization in modular networks and MoE language models."
collection: portfolio
published: false
---

SpecDrop treats dropout not as a regularizer but as a *structured signal*: by conditioning which modules are dropped on the input's category, gradients push each module to specialize on the categories where it is most often kept. A stability-guided freezing rule locks in specialized modules once they converge, preventing re-mixing.

Validated on multi-branch CNNs on CIFAR-100, then scaled to Mixture-of-Experts language models (60M–125M parameters, 8 experts) on domain-tagged SlimPajama using OLMoE/MegaBlocks on AWS. Evaluation covers per-domain perplexity and downstream tasks including HellaSwag, ARC-Easy, and PIQA.
