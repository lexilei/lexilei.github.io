---
title: "Learning Reusable Agent Subroutines from Experience"
collection: publications
category: manuscripts
permalink: /publication/2026-inducing-reasoning-primitives
excerpt: 'ARISE: an LLM agent mines its own successful traces into a library of natural-language subroutines, each executed by a separate LLM call. Across five tasks and two models it beats the strongest of six baselines by 6.1–10.8pp on average, and its source ReAct agent by up to 45.4pp.'
date: 2026-06-01
venue: 'Under review (ICLR 2027)'
paperurl: 'https://arxiv.org/abs/2606.02994'
citation: '<b>Lei, Z.</b>, Yan, J., Momo, J., & Cohen, W. W. (2026). "Learning Reusable Agent Subroutines from Experience." <i>arXiv:2606.02994</i>. Under review at ICLR 2027.'
---

ARISE (Agent Routine Induction from Successful Experience) is a gradient-free way for an LLM agent to improve from experience: it identifies recurring procedures in the agent's own successful traces and synthesizes them into a reusable library of agent subroutines. Each subroutine is a natural-language specification behind a callable interface, executed by its own LLM call rather than read in the agent's context or rewritten as code.

Across five tasks in narrative deduction (MuSR), rule application (RuleArena NBA), and constraint planning (Natural Plan), on DeepSeek-V3 and Gemini 2.5 Flash, ARISE beats the strongest of six baselines (including AWM, ACE, and ASI) by 6.1–10.8pp on average, and the ReAct agent that supplied its traces by up to 45.4pp (RuleArena NBA, 28.8% → 74.2%).

A controlled ablation isolates the execution interface: holding the induced text fixed, delivering it as retrievable skill documents or as Python tools scores 7.9–19.1pp lower on average. Libraries also transfer unchanged to a different model (+10.7–32.8pp on all five tasks), need no expert-designed tools, and extend to competition math (AIME).

[arXiv:2606.02994](https://arxiv.org/abs/2606.02994) · [code](https://github.com/lexilei/reasoning-primitives)
