---
title: "DCAFA: Differential Community Abundance and Feature Analysis for Histological Images"
title_zh: DCAFA：用于组织学图像的差异群体丰度与特征分析
authors: "Wright, G., Keller, P., Muter, J., Brosens, J., Tejpar, S., Minhas, F."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721329v1.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 基于回归的特征归因分析框架
tldr: 该研究提出DCAFA框架，用于在层级生物医学数据中同时分析社区组成变化与特征贡献，以捕捉组织结构和临床结局之间的联系，结合回归建模、协变量调控和统计推断，实现可解释的差异分析，在多种病理和分子成像任务中验证其有效性。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有方法多关注单个特征，忽略组织内不同结构的组成变化对生物学过程的影响。
method: DCAFA采用基于回归的框架，将样本中的局部结构聚类为潜在社区，并结合广义线性与混合效应模型进行差异分析。
result: DCAFA在多种生物医学数据上揭示了具有临床意义的组成变化和情境特异的特征关联。
conclusion: DCAFA为链接组织组成与临床或分子结果提供了统一、可解释且实用的分析工具。
---

## 摘要
组织学图像由多种局部结构组成，例如细胞、腺体或组织片段，其组织方式和相对丰度反映了潜在的生物过程。虽然大多数计算方法侧重于分析单个特征，但许多与临床相关的信号源自这些结构成分的变化，而非孤立的测量结果。这促使我们有必要显式建模相似实例群体在样本间的变化及其与结果的关系。我们提出了 DCAFA（Differential Community Abundance and Feature Attribution Analysis，差异群体丰度与特征归因分析），一个基于回归的框架，用于从组成和特征两个层面分析分层生物医学数据。DCAFA 将实例分组为潜在群体，这些群体代表了重复出现的形态学或表型模式，然后执行两种互补分析：（i）群体组成分析，用于识别在不同结果中富集或耗竭的群体；以及（ii）特征归因分析，用于定量评估实例级特征如何直接或在特定群体内与结果相关。这两种分析均采用广义线性模型和混合效应模型，能够进行协变量调整，并通过效应量、置信区间及虚假发现率控制进行推断。我们在多个生物医学场景中展示了 DCAFA 的实用性，包括子宫内膜组织病理学、空间转录组学、多重免疫荧光成像以及结直肠癌预定义细胞类型分析。这些示例揭示了传统特征方法未能捕捉到的可解释的组成变化和情境特异性特征关联。通过在同一统计框架中统一差异丰度检验与特征归因分析，DCAFA 作为一个开放可用的工具箱，为生物医学影像数据中组织组成与临床或分子结果的联系提供了实用且可解释的分析途径。代码地址：https://github.com/wgrgwrght/DCAFA

## Abstract
Histological images are composed of diverse local structures such as cells, glands, or tissue patches, whose organisation and relative abundance reflect underlying biological processes. While most computational approaches focus on analysing individual features, many clinically relevant signals arise from changes in the composition of these structures rather than isolated measurements. This motivates the need for explicitly modelling how groups of similar instances vary across samples and relate to outcomes. We present DCAFA (Differential Community Abundance and Feature Attribution Analysis), a regression-based framework for analysing hierarchical biomedical data through both compositional and feature-level perspectives. DCAFA groups instances into latent communities representing recurring morphological or phenotypic patterns, and then performs two complementary analyses: (i) community composition analysis, which identifies groups that are enriched or depleted across outcomes, and (ii) feature attribution analysis, which quantifies how instance-level features relate to outcomes directly or within specific communities. Both use generalised linear and mixed-effects models, enabling covariate adjustment and inference through effect sizes, confidence intervals, and false discovery rate control. We demonstrate the utility of DCAFA across multiple biomedical settings, including endometrial histopathology, spatial transcriptomics, multiplex immunofluorescence imaging, and predefined cell-type analyses in colorectal cancer. These examples identify interpretable compositional shifts and context-specific feature associations that are not captured by conventional feature-based approaches. By unifying differential abundance testing and feature attribution within a single statistical framework, DCAFA serves as an openly available toolbox that provides a practical and interpretable means of linking tissue composition with clinical or molecular outcomes in biomedical imaging data. Code available at: https://github.com/wgrgwrght/DCAFA