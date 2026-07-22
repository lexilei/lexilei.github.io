---
title: "Inducing Reasoning Primitives from Agent Traces"
collection: publications
category: manuscripts
permalink: /publication/2026-inducing-reasoning-primitives
excerpt: 'A self-improvement method: an LLM agent mines its own successful traces into reusable reasoning subroutines invoked as tools at test time. Induced libraries beat their source ReAct agent by +44pp on RuleArena NBA, +30pp on MuSR, +22pp on NatPlan, and beat the AWM agent-memory baseline at ~24% lower inference cost.'
date: 2026-06-01
venue: 'Under review (NeurIPS 2026)'
paperurl: 'https://arxiv.org/abs/2606.02994'
citation: '<b>Lei, Z.</b>, et al. (2026). "Inducing Reasoning Primitives from Agent Traces." <i>arXiv:2606.02994</i>. Under review at NeurIPS 2026.'
---

A gradient-free, test-time route to agent gains, complementary to RL post-training: the agent mines its own successful traces into reusable tools it invokes at test time.

Induced libraries beat their own source ReAct agent (DeepSeek-V3) — RuleArena NBA 30%→74% (+44pp), +30pp MuSR, +22pp NatPlan, with paired-Δ 95% bootstrap CIs strictly positive — and beat the prior agent-memory baseline (AWM) at ~24% lower inference cost.

Ablations isolate where the gains come from: replacing tool descriptions with adversarial text causes 20–32pp drops on content-critical tasks but no degradation on structure-only ones (cross-judge agreement 96.6%).

[arXiv:2606.02994](https://arxiv.org/abs/2606.02994)
