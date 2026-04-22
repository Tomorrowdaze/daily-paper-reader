---
title: "scDisent: disentangled representation learning with causal structure for multi-omic single-cell analysis"
title_zh: scDisent：用于多组学单细胞分析的具备因果结构的解缠表示学习
authors: "Xi, G."
date: 2026-04-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.12.717909v1.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 具有因果结构的解耦表示学习，用于机制解释
tldr: 本文提出scDisent，一种面向单细胞多组学分析的生成式解缠学习框架，通过区分表达和调控变量并建立稀疏因果映射，实现更高质量的模态整合与更强的生物机制解释，在多数据集验证中表现最佳。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有多组学集成模型将不同信号压缩为单一潜空间，缺乏解释性和对调控机制的刻画。
method: 该方法基于生成框架实现表达和调控变量的解缠表示，结合模态特征编码、变分解缠约束和基于Gumbel门控的因果模块。
result: scDisent在基准数据集上获得最佳整合表现，并揭示显式调控结构与生物学一致的谱系程序。
conclusion: scDisent显著提升多组学单细胞数据的整合质量与生物学解释性，使表征更适用于机制研究与假设生成。
---

## 摘要
单细胞多组学技术能够测量细胞身份和调控状态的互补方面，但大多数整合模型将这些信号压缩为一个纠缠的潜在空间。这类表示对于聚类分析有用，但不适合机制解释或以扰动为导向的分析。我们提出了 scDisent (https://github.com/xiguoren/scDisent)，这是一种用于解缠表示学习的生成框架，它将与表达相关的变量 (zexpr) 与与调控相关的变量 (zreg) 分离，并通过稀疏的有向映射将它们连接起来。scDisent 结合了特定模态编码、带有总相关和正交约束的变分解缠过程，以及通过基于 detach 的梯度隔离保护的 Gumbel 门控因果模块。在具有匹配模态的基准数据集上评估结果表明，scDisent 在整合性能上达到了最优表现，同时揭示了其他整合方法未显式建模的调控结构。学习到的因果图谱保持稀疏，扰动分析恢复了生物学一致的谱系相关程序，跨数据集的发现分析揭示了可解释的免疫、神经和发育特征。定量的分支分离分析进一步表明，基准标签信息集中在 zexpr 而非 zreg 中。总体而言，这些结果表明，scDisent 不仅能够提高整合质量，还能增强生物学可解释性，使单细胞多组学表示更适合回答生物学问题和进行计算假设生成。

## Abstract
Single-cell multi-omic technologies measure complementary aspects of cellular identity and regulatory state, yet most integration models compress these signals into one entangled latent space. Such representations are useful for clustering but poorly suited for mechanistic interpretation or perturbation-oriented analysis. We present scDisent (https://github.com/xiguoren/scDisent), a generative framework for disentangled representation learning that separates expression-associated variables (zexpr) from regulation-associated variables (zreg) and links them through a sparse directed mapping. scDisent combines modality-specific encoding, variational disentanglement with total-correlation and orthogonality constraints, and a Gumbelgated causal module protected by detach-based gradient isolation. Evaluated on benchmark datasets with matched modalities, scDisent achieved best-in-benchmark integration performance while exposing regulatory structure that competing integration methods do not model explicitly. The learned causal atlas remained sparse, perturbation analyses recovered biologically coherent lineage-associated programs, and cross-dataset discovery analyses highlighted interpretable immune, neural and developmental signatures. Quantitative branch-separation analyses further showed that benchmark-label information concentrated in zexpr rather than zreg. Together, these results position scDisent as a computational method that improves not only integration quality but also biological interpretability, making single-cell multi-omic representations better suited to biological question answering and in silico hypothesis generation.