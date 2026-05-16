---
title: "conMItion: an R package adjusting confounding factors for associations in multi-omics"
title_zh: conMItion：一个用于调整多组学关联分析中混杂因素的 R 软件包
authors: "Wang, G., Liu, F., Chen, Z., Davoli, T."
date: 2026-05-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.07.723535v1.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 使用条件互信息调整关联分析中的混杂因素
tldr: 本研究提出R包conMItion，基于条件互信息方法校正多组学数据中的混杂因素如肿瘤纯度和突变负荷。通过在膀胱癌和肺癌数据的应用，验证了该工具在揭示关键基因关联和细胞类型关系中的有效性，提升了癌症多组学分析的可靠性。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有癌症多组学关联分析易受肿瘤纯度、突变负荷等混杂因素干扰，影响结果准确性。
method: 研究开发了R包conMItion，基于条件互信息计算并校正一至两个混杂因素的影响。
result: conMItion在膀胱癌基因组数据和肺癌单细胞RNA测序数据中成功识别了相关的体细胞改变和细胞类型关联。
conclusion: conMItion为多组学数据研究提供了一个有效校正混杂因素的工具，有助于提高癌症数据关联分析的准确性。
---

## 摘要
摘要 关联性度量（如互信息，Mutual Information，MI）是癌症多组学数据分析的基础，用于识别与癌症相关的基因、基因特征以及基因调控网络，从而深入理解肿瘤的发生、发展和治疗。诸如肿瘤纯度和突变负担等混杂因素可能会使MI中的关联性度量产生偏差，进而导致将乘客事件误判为驱动事件。条件互信息（Conditional Mutual Information，CMI）提供了一个稳健的框架，能够在同时考虑不同混杂因素的情况下，评估线性和非线性关联。本文介绍了一个名为 **conMItion** 的 R 软件包，用于估算多组学数据的 CMI 及其统计显著性，并能灵活地调整一个或两个混杂因素。我们通过两个应用实例展示了 conMItion 的使用。首先，我们在膀胱癌基因组数据显示中识别了共发生的体细胞突变。其次，我们将 conMItion 应用于肺癌患者的单细胞 RNA 测序数据，识别出在肺癌肿瘤微环境中呈正相关或负相关的细胞类型。

可获得性与实现 conMItion 软件包可在 CRAN 免费获取，网址为 https://CRAN.R-project.org/package=conMItion。文中描述的两个应用实例可在 https://github.com/GJYWang/conMItion 获取。在线提供补充文档。

## Abstract
SummaryAssociation measurements, such as mutual information (MI), are fundamental in the analysis of cancer multi-omics data for identifying cancer-related genes, gene signatures, and gene regulatory networks, thereby shedding light on tumor development, progression, and treatment. Confounding factors, including tumor purity and mutation burden, can bias association measurements in MI, potentially leading to the misclassification of passenger events as drivers. Conditional mutual information (CMI) provides a robust framework for assessing both linear and non-linear associations while effectively accounting for different confounding factors. An R package called conMItion is introduced to estimate CMI and its statistical significance for multi-omics data, with flexibility to adjust for one or two confounding factors. We demonstrated the utilization of conMItion through two use cases. First, we identified co-occurring somatic alterations in bladder cancer genomic data. Second, we applied conMItion to a single-cell RNA sequencing dataset of lung cancer patients and identified positively or negatively associated cell types within the lung cancer tumor microenvironment.

Availability and ImplementationThe conMItion package is freely available on CRAN at https://CRAN.R-project.org/package=conMItion. The two use cases described in the paper can be accessed at https://github.com/GJYWang/conMItion. A supplementary document is available online.