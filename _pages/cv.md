---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

A PDF version is available [here](/files/cv.pdf).

Education
======
* **M.S. in Machine Learning**, Carnegie Mellon University — Dec. 2026 (expected)
  * GPA: 3.7
  * Coursework: Advanced Deep Learning, Convex Optimization, Probabilistic Graphical Models, Advanced Intro. to Machine Learning, Probability & Mathematical Statistics
* **B.S. in Physics**, minor in Computer Science, Emory University — 2021 – Dec. 2023
  * GPA: 3.8. Dean's List; Sigma Pi Sigma Physics Honor Society; Society of Physics Students
  * Physics coursework: Quantum Mechanics, Statistical Mechanics & Thermodynamics, Electrodynamics, Classical Mechanics, Mathematical Statistics, Computational Modeling, Differential Equations, Linear Algebra, Advanced Laboratory
  * CS coursework: System Programming, Data Structures & Algorithms, Analysis of Algorithms, Computer Architecture & Assembly, Machine Learning, Quantum Computing
* **Reed College**, Physics — 2019 – 2021 (transferred to Emory)

Research experience
======
* **Graduate Researcher**, Carnegie Mellon University — LLM agents & reasoning — *Jan. 2026 – Present*
  * Advisor: Prof. William Cohen
  * **Reasoning Primitive Induction** (first author, under review at NeurIPS 2026; led a team of 4): automatically extracts reusable reasoning subroutines from an LLM agent's successful traces and packages them as tools the agent calls at test time — a gradient-free, test-time route to agent gains, complementary to RL post-training.
  * Induced libraries beat their own source ReAct agent (DeepSeek-V3): RuleArena NBA 30%→74% (+44pp), +30pp MuSR, +22pp NatPlan (paired-Δ 95% bootstrap CIs strictly positive); beat the AWM agent-memory baseline at ~24% lower inference cost.
  * Discovery matches expert design: with no per-task authoring, induced libraries match or exceed hand-authored decompositions on every comparable subtask across MuSR, RuleArena, and NatPlan.
  * Ablations: replacing tool descriptions with adversarial text causes 20–32pp drops on content-critical tasks but no degradation on structure-only ones; cross-judge agreement 96.6%.
  * **Learning to Construct** (co-first author, under review at NeurIPS 2026; co-led a team of 7): casts agent systems as code, enabling automatic construction of efficient agent systems; the cross-benchmark study maps induction across 19 reasoning tasks — gains scale with baseline-tool weakness, e.g. +8.2pp on MedCalc at ~60% fewer input tokens.
* **Research Assistant**, Rice University — *Sep. 2024 – May 2025*
  * Advisor: Prof. Xia "Ben" Hu
  * Adaptive framework mitigating relational bias in heterogeneous knowledge graphs: dynamic bias modeling with relational attention and a self-regularizing scheme improving performance on low-frequency relations; evaluated on ACM and BioKG.
* **Researcher**, Emory Machine Learning Lab — graph learning & retrieval — *Apr. 2024 – Feb. 2025*
  * Advisor: Prof. Liang Zhao
  * Proposed **GRAG** (NAACL 2025): divide-and-conquer subgraph retrieval with linear-time complexity and dual text-view/graph-view prompting; outperformed SOTA RAG on multi-hop graph reasoning.
  * Developed **CG-RAG** (SIGIR 2025): chunk-level contextual citation graph with Lexical-Semantic Graph Retrieval (LeSeGR) that fuses sparse and dense signals via graph message passing; proved hybrid retrieval is a special case.
  * Built the lab's scientific-QA RAG stack ([SciQA](https://github.com/HuieL/SciQA)) on AWS SageMaker with GCN/GAT retrievers over citation graphs; established sentence-transformer baselines and cut training time ~60% with multi-GPU distributed methods.
* **Software Engineer**, Emory NLP Research Lab — *Jan. 2023 – May 2023*
  * Advisor: Prof. Jinho Choi
  * Built a peer-help chatbot platform in Python with secure integration of official student data; ChatGPT integration raised sentiment-analysis accuracy by 45%.
* **Research Assistant**, Emory Math Department — *Aug. 2022 – Dec. 2022*
  * Advisor: Prof. Difeng Cai
  * Trained deep vision models on multiple GPUs (TensorFlow/PyTorch) with pseudo-labeling, cross-validation, and model fusion; implemented a first-order attention model from the paper up — multi-head self-attention, transformer blocks, embedding layers.
* **Research Assistant**, Emory Physics Department — *May 2022 – Aug. 2022*
  * Advisor: Prof. Sergei Urazhdin
  * Built a compact, cost-effective variable magnetic-field source from Halbach arrays — strong uniform fields up to 0.5 T over centimeter-scale regions with no power or cooling — and a Python control system for reproducible field adjustment without feedback, eliminating remanence effects.
* **Research Assistant**, Reed College Math Department — *May 2021 – Aug. 2021*
  * Advisor: Prof. David Perkinson
  * Studied firing posets and their generating functions, finding isomorphic mappings between poset structure and algebraic properties; built an algorithm that renders partial-order relations as graphs.

Quantitative research
======
Independent research, 2026 – Present. Kept deliberately high-level here; specifics on request.

* **Text-based equity signals** — signal research on SEC filings, with an emphasis on evaluation hygiene: point-in-time data, purged walk-forward validation, factor-model attribution, and explicit multiple-testing control.
* **Options volatility** — relative-value research on index options: surface fitting, delta-hedged backtesting, regime conditioning.
* **Statistical arbitrage** — cointegration-based pair strategies with dynamically estimated hedge ratios under sector and beta neutrality.

Professional experience
======
* **Software Engineer Intern**, Amazon — Ads org, FAIM team — *May 2026 – Aug. 2026*
  * Building a schema-grounded Redshift-to-PartiQL transpiler driven by an LLM agent: transpiles queries, validates semantic correctness by executing against benchmark cases, and auto-generates analytics dashboards from context hints.
* **Machine Learning Engineer Intern**, ByteDance — Trust & Safety — *Jul. 2023 – Sep. 2023*
  * Diagnosed an offline-to-live precision gap masked by clean training data; fine-tuned a real-time face-matching verifier, lifting live (human-review-confirmed) precision 62% → 83%, deployed as a production identity-verification module.
  * Modeled user behavioral sequences over millions of daily activities in Spark SQL to build risk-scoring features for scammer detection; surfaced a 10k-user high-risk cohort for downstream enforcement.
  * Built a 45TB user behavior graph in a Gremlin-based graph database (migrated from Hive via Spark, with Python tools verifying data accuracy), enabling graph-based anomaly detection and improving downstream analysis efficiency by 40%.
  * Built a data API (Pandas/NumPy) that parses the user event log into auto-generated dashboards; deployed as a cloud service.

Earlier experience
======
* **Nuclear Reactor Technician**, Reed Research Reactor — *Sep. 2020 – May 2021*
  * Conducted regular inspections of the campus research reactor under strict safety protocols.
* **Academic Tutor**, Reed College — *Sep. 2020 – May 2021*
  * Drop-in tutor for Physics 101/102; separately selected as one-on-one tutor for math and physics courses.

Projects
======
* **SpecDrop: parameter-free modular specialization** — CMU, second author, under review at NeurIPS 2026 — *Feb. 2026 – May 2026*
  * Repurposes dropout for category-conditioned routing with no learned gating network; stability-guided freezing locks converged modules to cut training compute.
  * Designed the specialization metrics (module–category mutual information, pruning sensitivity) and per-domain evaluation; validated on CIFAR-100 ResNets and 60–125M-parameter MoE LMs.
* **Peer-help web platform**, Emory Goizueta Business School — *Feb. 2024 – Apr. 2024*
  * React + Spring Boot application serving 1000+ users; RESTful APIs and database optimization cut retrieval times ~30%; Docker/Kubernetes deployment on GCP with 99% uptime.

Skills
======
* **Research areas**: LLM agents & reasoning, test-time compute, self-improving agents, tool synthesis & skill discovery, LLM evaluation, mixture-of-experts / modular specialization, retrieval-augmented generation, graph neural networks
* **Quant methods**: signal evaluation (rank-IC), backtesting (walk-forward, purged CV), multiple-testing control (Deflated Sharpe), factor models (Fama-French, Carhart), gradient boosting (LightGBM)
* **ML & statistical methods**: Transformer/attention, fine-tuning/LoRA, probabilistic graphical models, Bayesian inference, causal inference, A/B experimentation, convex optimization, stochastic modeling, time-series analysis
* **Languages**: Python (PyTorch, Hugging Face, NumPy, Pandas, SciPy, statsmodels, scikit-learn), C++, C, SQL, Java, Go, R, MATLAB
* **Tools & platforms**: TensorFlow, LangChain/LangGraph, CUDA, AWS (SageMaker, EC2), GCP, Spark, Docker, Kubernetes, Git, Linux, Hive, ClickHouse, Oracle Cloud, React, Spring Boot

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
