---
title: "SP-MoE: Speculative Decoding and Prefetching for Accelerating MoE-based Model Inference"
collection: publications
category: conferences
permalink: /publication/paper0
authors: Liangkun Chen, Zijian Wen, Tian Wu, Xiaoxi Zhang, Chuan Wu
excerpt: 'This paper introduce an efficient MoE inference framework for single machine even if the gpu resource is restricted.'
date: 11 Oct 2025
venue: 'Arxiv'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2510.10302'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
The Mixture-of-Experts (MoE) architecture has been widely adopted in large language models (LLMs) to reduce computation cost through model sparsity. Employing speculative decoding (SD) can further accelerate MoE inference by drafting multiple tokens per step and verifying them in parallel. However, combining MoE with SD inflates GPU memory and aggravates CPU-GPU bandwidth contention during multi-token verification. Existing MoE offloading systems are SD-agnostic and do not address this bottleneck. We present SP-MoE, the first SD-aware expert-offloading and compute-communication pipelining framework. SP-MoE introduces: (1) speculative expert prefetching that exploits structural correspondence between the draft and target models to prefetch likely experts ahead of verification; (2) a cutoff-layer policy that bounds per-layer prefetch depth based on empirical profiles and an analytical latency model, guaranteeing just-in-time availability without overfetch; and (3) a pipelined runtime with asynchronous prefetch threads and batched I/O to hide loading latency. Extensive experiments demonstrate that SP-MoE achieves a 1.07-3.5 times TPOT speedup over state-of-the-art methods across diverse datasets, environments, and MoE-based models.