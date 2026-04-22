---
title: "From Agent Traces to Reasoning Primitives: Automatic Discovery of Reusable Reasoning Subroutines"
collection: publications
category: manuscripts
permalink: /publication/2026-reasoning-primitives
excerpt: 'Bottom-up discovery of composable reasoning primitives from ReAct agent traces. Induced workflows achieve 81.3% on MUSR narrative reasoning vs. 68% ReAct and 75% hand-designed baselines.'
date: 2026-01-01
venue: 'In preparation (NeurIPS 2026)'
citation: '<b>Lei, Z.</b> & Cohen, W. (2026). "From Agent Traces to Reasoning Primitives: Automatic Discovery of Reusable Reasoning Subroutines." <i>In preparation.</i>'
published: false
---

Open-ended ReAct agents are flexible but expensive and inconsistent. This work recovers the structure: we mine traces of successful ReAct runs, cluster recurring reasoning motifs, and distill them into composable primitives that can be re-used as fixed-cost subroutines.

On MUSR narrative reasoning, induced workflows reach 81.3% vs. 68% for raw ReAct and 75% for hand-designed baselines. Ablations localize the gain — conclusion aggregation is the critical bottleneck; a single induced primitive accounts for most of the improvement, and primitives function as implicit prompt scaffolding (+6.7% even when not explicitly invoked). Composed into fixed-cost pipelines, primitives give predictable token budgets and a clean accuracy–cost frontier against open-ended chains.

*In preparation for NeurIPS 2026.*
