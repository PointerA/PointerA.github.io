---
title: "VFL-Cafe: Communication-Efficient Vertical Federated Learning via Dynamic Caching and Feature Selection"
collection: publications
category: manuscripts
permalink: /publication/paper3
excerpt: 'This work accelerates VFL training via caching and feature selection.'
date: 14 January 2025
venue: 'Entropy'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://www.mdpi.com/1099-4300/27/1/66'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

Vertical Federated Learning (VFL) is a promising category of Federated Learning that enables collaborative model training among distributed parties with data privacy protection. Due to its unique training architecture, a key challenge of VFL is high communication cost due to transmitting intermediate results between the Active Party and Passive Parties. Current communication-efficient VFL methods rely on using stale results without meticulous selection, which can impair model accuracy, particularly in noisy data environments. To address these limitations, this work proposes VFL-Cafe, a new VFL training method that leverages dynamic caching and feature selection to boost communication efficiency and model accuracy. In each communication round, the employed caching scheme allows multiple batches of intermediate results to be cached and strategically reused by different parties, reducing the communication overhead while maintaining model accuracy. Additionally, to eliminate the negative impact of noisy features that may undermine the effectiveness of using stale results to reduce communication rounds and incur significant model degradation, a feature selection strategy is integrated into each round of local updates. Theoretical analysis is then conducted to provide guidance on cache configuration, optimizing performance. Finally, extensive experimental results validate VFL-Cafe’s efficacy, demonstrating remarkable improvements in communication efficiency and model accuracy.