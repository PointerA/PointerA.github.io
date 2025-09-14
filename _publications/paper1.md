---
title: "Accelerating Edge Inference for Distributed MoE Models with Latency-Optimized Expert Placement"
collection: publications
category: conferences
permalink: /publication/paper1
authors: Tian Wu, Liming Wang, Zijian Wen, Xiaoxi Zhang, Jingpu Duan, Xianwei Zhang, Jinhang Zuo
excerpt: 'This paper introduce an efficient MoE inference framework that enables activation-aware expert placement across heterogeneous edge servers.'
date: 18 Aug 2025
venue: 'Arxiv'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2508.12851'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
Mixture-of-Experts (MoE) have become a cornerstone for training and scaling large language models (LLMs), offering substantial gains in model capacity and efficiency through sparse expert activation. However, serving these models remains challenging in practice, particularly in resource-constrained edge environments, due to their large memory footprint and complex communication demands. While centralized cloud inference is common, it incurs high infrastructure costs, along with latency and privacy concerns. A few recent edge MoE works propose memory-efficient strategies but typically focus on single-device or homogeneous setups. This paper presents DanceMoE, an efficient MoE inference framework that enables activation-aware expert placement across collaborative, heterogeneous, GPU-equipped edge servers. DanceMoE leverages the inherent sparsity of MoE models and workload locality to minimize cross-server communication and enable efficient expert placement under heterogeneous resource constraints. It introduces a data-driven, activation-aware placement algorithm that balances local coverage and memory usage across servers, alongside a lightweight migration mechanism that adapts expert assignments under evolving workloads. We evaluate DanceMoE on modern MoE models and widely used datasets, demonstrating up to 30.6\% lower inference latency, and substantial communication reduction compared to state-of-the-art baselines, showcasing the effectiveness of collaborative edge-based MoE inference.