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
* **M.S. in Machine Learning**, Carnegie Mellon University, Dec. 2026 (expected)
  * GPA: 3.6
  * Coursework: Advanced Deep Learning, Convex Optimization, Probabilistic Graphical Models, Advanced Intro. to Machine Learning, Probability & Mathematical Statistics
* **B.S. in Physics**, Emory University, Dec. 2023
  * Minor in Computer Science. GPA: 3.8
  * Awards: Dean's List, Sigma Pi Sigma Physics Honor Society
  * Coursework: Quantum Mechanics, Statistical Mechanics & Thermodynamics, Mathematical Statistics, Computational Modeling, Electromagnetism, Classical Mechanics, Differential Equations, Linear Algebra

Research experience
======
* **Graduate Researcher**, Carnegie Mellon University — *Jan. 2026 – Present*
  * Advisor: Prof. William Cohen
  * Research on LLM reasoning and agentic systems.

* **Researcher**, Emory Machine Learning Lab — *Apr. 2024 – Feb. 2025*
  * Advisor: Prof. Liang Zhao
  * Proposed **GRAG** (NAACL 2025): divide-and-conquer subgraph retrieval with linear-time complexity and dual text-view/graph-view prompting; outperformed SOTA RAG on multi-hop graph reasoning.
  * Developed **CG-RAG** (SIGIR 2025): chunk-level contextual citation graph with Lexical-Semantic Graph Retrieval (LeSeGR) that fuses sparse and dense signals via graph message passing; proved hybrid retrieval is a special case.

Professional experience
======
* **SDE Intern**, Amazon Ads — *Summer 2026*
  * Full-Funnel Agentic Intelligence and Models (FAIM) team. Agentic AI systems for full-funnel advertising optimization — audience modeling, causal attribution, incrementality measurement, A/B experimentation at scale.

* **Software Engineer Intern**, ByteDance — *Jul. 2023 – Sep. 2023*
  * Fine-tuned a face-matching model for account security; precision 62% → 83%, deployed as a real-time identity verification module in production.
  * Modeled user behavioral sequences over millions of daily activities in Spark SQL to build risk-scoring features for scammer detection; surfaced a 10k-user high-risk cohort.
  * Built a 45TB user behavior graph in a Gremlin-based graph database, enabling graph-based anomaly detection and improving downstream analysis efficiency by 40%.

Skills
======
* **ML & Statistical Methods**: Transformer/Attention, RAG, Graph Neural Networks, Mixture-of-Experts, Fine-tuning/LoRA, Causal Inference, A/B Experimentation, Probabilistic Graphical Models, Bayesian Inference, Stochastic Modeling, Time-Series Analysis, Convex Optimization
* **Programming Languages**: Python (NumPy, Pandas, SciPy, statsmodels, Scikit-learn), C++, SQL, Go, R, MATLAB, Java, C
* **Tools & Platforms**: PyTorch, TensorFlow, LangChain/LangGraph, CUDA, Hugging Face, AWS (SageMaker, EC2), Spark, Docker, Git, Linux, Hive, ClickHouse

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
