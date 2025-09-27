---
title: "PASTA: Training Acceleration for Vertical Federated Learning via Adaptive Pipeline Parallelism"
collection: publications
category: conferences
permalink: /publication/paper2
authors: Tian Wu, Weijie Liu, Han Liang, Ziwei Zhan, Jingpu Duan, Chuan Wu, Jinhang Zuo, Xu Chen, Xiaoxi Zhang
excerpt: 'This paper is a framework named PASTA to accelerate VFL training.'
date: 02-04 July 2025
venue: '2025 IEEE/ACM 33rd International Symposium on Quality of Service (IWQoS)'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://ieeexplore.ieee.org/document/11143476'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

Vertical federated learning (VFL) enables collaborative model training among geo-distributed participants, each with different features of the same samples, but only one party possesses the labels. Communication delays between active and passive parties in VFL significantly hinder its training efficiency. Existing VFL methods adopt asynchronous schemes or multiple local updates per communication round, but they either introduce heavy computation overhead or fail to adapt to dynamic network conditions. This work proposes PASTA, a novel framework employing Adaptive Pipeline Parallelism with Staleness Control for VFL, designed to mitigate these delays and balance training efficiency and model performance. PASTA enables concurrent communication and computation, maximizing resource utilization and minimizing idle time by strategically using stale gradients. Each passive party can send one or more batches of embeddings per communication and conduct stale local training, so that computation times can overlap with communication latency. Since staleness impedes model accuracy despite its benefits in reducing time, a dynamic feedback-based mechanism is proposed to adjust the numbers of embeddings sent and local training iterations based on system heterogeneity. Extensive experiments across various datasets demonstrate that PASTA significantly enhances convergence speed by 1.8× to 4.6× compared to leading VFL systems, without compromising final accuracy. The source code is available at https://github.com/PointerA/PASTA.
