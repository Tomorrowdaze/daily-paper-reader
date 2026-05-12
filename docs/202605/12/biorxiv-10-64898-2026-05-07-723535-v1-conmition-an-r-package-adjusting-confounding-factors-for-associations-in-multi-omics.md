---
title: "conMItion: an R package adjusting confounding factors for associations in multi-omics"
title_zh: conMItion：一个用于校正多组学关联中混杂因素的R软件包
authors: "Wang, G., Liu, F., Chen, Z., Davoli, T."
date: 2026-05-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.07.723535v1.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 使用条件互信息评估关联并处理混杂因素
tldr: 本研究针对癌症多组学关联分析中混杂因素造成的偏差，提出并实现了基于条件互信息的R包conMItion，可灵活调整混杂因素并显著提高关联分析的准确性，在膀胱癌和肺癌数据中验证了其实用性。
source: biorxiv
selection_source: fresh_fetch
motivation: 多组学关联分析易受肿瘤纯度和突变负荷等混杂因素影响，导致关联偏差。
method: 研究开发了R包conMItion，用条件互信息方法调整一至两个混杂因素并评估统计显著性。
result: 使用示例显示conMItion能识别膀胱癌基因协同变化及肺癌单细胞类型关联。
conclusion: conMItion为多组学数据分析提供了有效方法，可在控制混杂因素的同时揭示生物分子间真实关联。
---

## 摘要
关联度量（如互信息，MI）在癌症多组学数据分析中具有基础性作用，用于识别与癌症相关的基因、基因特征和基因调控网络，从而揭示肿瘤的发生、发展和治疗机制。混杂因素（包括肿瘤纯度和突变负荷）可能会使MI的关联评估产生偏差，从而导致乘客事件被误判为驱动事件。条件互信息（CMI）提供了一个稳健的框架，用于评估线性和非线性关联，同时能够有效控制不同的混杂因素。本文介绍了一个名为 conMItion 的R软件包，用于估算多组学数据的CMI及其统计显著性，且可灵活调整一个或两个混杂因素。我们通过两个应用实例展示了 conMItion 的使用方法。首先，我们在膀胱癌基因组数据中识别了共发生的体细胞变异。其次，我们将 conMItion 应用于肺癌患者的单细胞RNA测序数据，识别出了肺癌肿瘤微环境中呈正相关或负相关的细胞类型。

## Abstract
Association measurements, such as mutual information (MI), are fundamental in the analysis of cancer multi-omics data for identifying cancer-related genes, gene signatures, and gene regulatory networks, thereby shedding light on tumor development, progression, and treatment. Confounding factors, including tumor purity and mutation burden, can bias association measurements in MI, potentially leading to the misclassification of passenger events as drivers. Conditional mutual information (CMI) provides a robust framework for assessing both linear and non-linear associations while effectively accounting for different confounding factors. An R package called conMItion is introduced to estimate CMI and its statistical significance for multi-omics data, with flexibility to adjust for one or two confounding factors. We demonstrated the utilization of conMItion through two use cases. First, we identified co-occurring somatic alterations in bladder cancer genomic data. Second, we applied conMItion to a single-cell RNA sequencing dataset of lung cancer patients and identified positively or negatively associated cell types within the lung cancer tumor microenvironment.