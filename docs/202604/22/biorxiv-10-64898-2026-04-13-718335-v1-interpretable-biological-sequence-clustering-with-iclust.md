---
title: Interpretable Biological Sequence Clustering with iClust
title_zh: 具有可解释性的生物序列聚类方法 iClust
authors: "Zhang, S., Liu, X., Lou, J., Jiang, M., He, Z."
date: 2026-04-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.13.718335v1.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 可解释的聚类方法用于提供可解释的分组
tldr: 本文提出了iClust算法，用于生物序列的可解释聚类。该方法通过代表性原型和自适应半径描述每个簇，结合局部结构特性进行动态聚类，并在后处理阶段整合碎小簇以增强稳定性。实验证明，iClust在保持聚类精度的同时显著提升了聚类结果的可解释性。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有生物序列聚类方法缺乏对聚类成因的解释能力，限制了其在下游生物分析中的实用性。
method: iClust以代表性原型和自适应半径为核心，通过局部结构自调节及后续整合步骤实现高解释性聚类。
result: iClust在模拟和真实生物序列数据上表现出与传统方法相当的聚类性能，并显著提高了聚类解释性。
conclusion: iClust为生物序列聚类提供了兼顾性能与可解释性的全新思路，有助于拓展可解释机器学习在生物信息学中的应用。
---

## 摘要
生物序列聚类是生物信息学中的一个基础问题，但现有的大多数方法主要致力于优化聚类质量或效率，对序列为何被聚到一起缺乏深入解释。这限制了其在下游分析中的实用性，因为这些分析通常需要代表性序列和清晰的聚类边界。为了解决这一问题，我们提出了 iClust，一种可解释的聚类方法，它通过代表性原型和自适应半径来刻画每个聚类。通过适应局部序列结构，而非依赖单一的全局阈值，iClust 能生成既有意义又可解释的聚类。最终的整合步骤进一步减少了微小碎片并提升了结构稳定性。在模拟数据和真实生物序列数据集上的实验表明，iClust 在聚类性能上具有竞争力，同时比传统的基于阈值的方法提供了更清晰的聚类层面解释。除了作为一种实用的生物序列聚类方法的经验性价值之外，本文还为从可解释机器学习的视角发展生物序列聚类方法开辟了新的方向。

## Abstract
Biological sequence clustering is a fundamental problem in bioinformatics, yet most existing methods mainly optimize clustering quality or efficiency while offering limited insight into why sequences are grouped together. This restricts their usefulness in downstream analysis, where representative sequences and clear cluster boundaries are often needed. To address this issue, we propose iClust, an interpretable clustering method that characterizes each cluster by a representative prototype and an adaptive radius. By adapting to local sequence structure rather than relying on a single global threshold, iClust produces clusters that are both meaningful and explainable. A final consolidation step further reduces tiny fragments and improves structural stability. Experiments on simulated and real biological sequence datasets show that iClust achieves competitive clustering performance while providing clearer cluster-level explanations than conventional threshold-based methods. In addition to its empirical impact as a practical clustering method for biological sequences, this article opens up new avenues for developing biological sequence clustering approaches from the viewpoint of interpretable machine learning.