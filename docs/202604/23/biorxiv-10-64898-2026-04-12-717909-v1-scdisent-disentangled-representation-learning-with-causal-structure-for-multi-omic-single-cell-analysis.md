---
title: "scDisent: disentangled representation learning with causal structure for multi-omic single-cell analysis"
title_zh: scDisent：用于多组学单细胞分析的具备因果结构的可分解表示学习
authors: "Xi, G."
date: 2026-04-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.12.717909v1.full.pdf"
tags: ["query:q6"]
score: 6.5
evidence: 具有因果结构的解耦表示学习，用于机制解释
tldr: 本文提出scDisent，一种可将单细胞多组学数据中表达和调控变量解耦的生成框架，通过稀疏因果映射和变分解耦提高数据整合质量并增强生物学可解释性，在基准数据上验证了其优越性能。
source: biorxiv
selection_source: fresh_fetch
motivation: 大多数单细胞多组学整合模型将多模态信号压缩到纠缠的潜空间中，限制了对调控机制的解释能力。
method: 该方法采用模态特异编码、变分解耦约束和基于Gumbel门控的因果模块来学习稀疏定向映射。
result: scDisent在多个基准数据集上实现了最佳整合性能，并揭示出竞争方法无法显式建模的调控结构。
conclusion: scDisent有效提升了单细胞多组学整合的质量和可解释性，为机制研究和计算假设生成提供了有力工具。
---

## 摘要
单细胞多组学技术能够测量细胞身份和调控状态的互补方面，但现有的大多数整合模型将这些信号压缩为一个纠缠的潜在空间。这样的表示虽然有助于聚类，但不利于机制解释或以扰动为导向的分析。我们提出了 scDisent（https://github.com/xiguoren/scDisent），一个用于可分解表示学习的生成式框架，它将与表达相关的变量（zexpr）与与调控相关的变量（zreg）分离，并通过一个稀疏的有向映射将它们连接起来。scDisent 结合了特定模态的编码、具有总相关与正交约束的变分解耦，以及一个由 detach 基于梯度隔离机制保护的 Gumbel 门控因果模块。我们在匹配的模态基准数据集上评估了 scDisent，结果显示其达到了最佳的整合性能，同时揭示了竞争整合方法未显式建模的调控结构。学习到的因果图谱保持稀疏，扰动分析恢复了生物学上连贯的谱系相关程序，而跨数据集的发现分析突出显示了可解释的免疫、神经和发育特征。定量分支分离分析进一步表明，基准标签信息集中在 zexpr 而非 zreg 中。总体而言，这些结果表明，scDisent 是一种能够提升整合质量并增强生物学可解释性的计算方法，使单细胞多组学表示更适合回答生物学问题和进行计算假设生成。

## Abstract
Single-cell multi-omic technologies measure complementary aspects of cellular identity and regulatory state, yet most integration models compress these signals into one entangled latent space. Such representations are useful for clustering but poorly suited for mechanistic interpretation or perturbation-oriented analysis. We present scDisent (https://github.com/xiguoren/scDisent), a generative framework for disentangled representation learning that separates expression-associated variables (zexpr) from regulation-associated variables (zreg) and links them through a sparse directed mapping. scDisent combines modality-specific encoding, variational disentanglement with total-correlation and orthogonality constraints, and a Gumbelgated causal module protected by detach-based gradient isolation. Evaluated on benchmark datasets with matched modalities, scDisent achieved best-in-benchmark integration performance while exposing regulatory structure that competing integration methods do not model explicitly. The learned causal atlas remained sparse, perturbation analyses recovered biologically coherent lineage-associated programs, and cross-dataset discovery analyses highlighted interpretable immune, neural and developmental signatures. Quantitative branch-separation analyses further showed that benchmark-label information concentrated in zexpr rather than zreg. Together, these results position scDisent as a computational method that improves not only integration quality but also biological interpretability, making single-cell multi-omic representations better suited to biological question answering and in silico hypothesis generation.