---
title: AI-readiness criteria for biomedical data
title_zh: 生物医学数据的 AI 准备标准
authors: "Clark, T., Caufield, H., Parker, J. A., Al Manir, S., Amorim, E., Eddy, J., Gim, N., Gow, B., Goar, W., Hansen, J. N., Harris, N., Hermjakob, H., Joachimiak, M., Jordan, G., Lee, I.-H., McWeeney, S. K., Nebeker, C., Nikolov, M., Reese, J., Shaffer, J., Sheffield, N., Sheynkman, G., Stevenson, J., Chen, J. Y., Mungall, C., Wagner, A., Kong, S. W., Ghosh, S. S., Patel, B., Williams, A., Munoz-Torres, M. C."
date: 2026-04-24
pdf: "https://www.biorxiv.org/content/10.1101/2024.10.23.619844v6.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 定义了复杂数据中可解释人工智能(XAI)和模型前可解释性的标准。
tldr: 本文针对生物医学AI应用中数据准备复杂、伦理和可解释性不足的问题，提出了一套涵盖FAIR性、溯源、特征、伦理、预模型可解释性、可持续性和计算性七个维度的AI准备度标准，并在多个NIH Bridge2AI数据集上验证其有效性，为AI建模前阶段的数据质量和伦理治理提供统一框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 生物医学数据复杂且仅符合FAIR原则不足以确保AI的伦理和可解释性，因此需要建立更全面的预建模阶段标准。
method: 研究由NIH Bridge2AI标准工作组制定了七个核心维度的AI准备度标准，并在四个旗舰数据集上进行评估和元数据编码。
result: 提出的七维度标准体系应用于多种数据类型，证明可提升数据的科学严谨性和伦理完整性。
conclusion: 该研究确立了生物医学数据AI可用性的系统框架，为道德、可解释和可重复的AI研究奠定基础。
---

## 摘要
生物医学研究正在迅速采用人工智能（AI）。然而，生物医学数据准备过程的复杂性需要在“模型前”（pre-model）阶段实施可操作且稳健的标准，以确保伦理性和可解释性人工智能（XAI），涵盖数据采集、详细数据转换及伦理治理。仅仅遵循 FAIR 原则（可发现、可获取、可互操作、可重复使用）是不足的。

本文由 NIH Bridge to Artificial Intelligence（Bridge2AI）标准工作组制定可靠的生物医学数据 AI 准备标准和实践，在数据集的七个核心维度定义了 AI 准备要求：FAIRness（可发现性与可用性）、Provenance（来源溯源）、Characterization（特征描述）、Ethics（伦理）、Pre-model Explainability（模型前可解释性）、Sustainability（可持续性）以及 Computability（可计算性）。遵守这些标准为模型前的科学严谨性和伦理完整性奠定基础，在 AI 建模之前减少偏差和错误带来的下游风险。我们将这些标准应用并评估于四个 Bridge2AI 旗舰数据集，涵盖从功能基因组学到临床医学领域，并将其编码为机器可操作的元数据绑定到数据集中。

该框架为准备符合伦理且可复用的生物医学 AI 数据集设立了基准，并提供了标准化方法用于可靠的模型前数据评估。

## Abstract
Biomedical research is rapidly adopting artificial intelligence (AI). Yet the inherent complexity of biomedical data preparation requires implementing actionable, robust criteria for ethical and explainable AI (XAI) at the "pre-model" stage, encompassing data acquisition, detailed transformations, and ethical governance. Simple conformance to FAIR (Findable, Accessible, Interoperable, Reusable) Principles is insufficient.

Here, we define criteria and practices for reliable AI-readiness of biomedical data, developed by the NIH Bridge to Artificial Intelligence (Bridge2AI) Standards Working Group across seven core dimensions of dataset AI-readiness: FAIRness, Provenance, Characterization, Ethics, Pre-model Explainability, Sustainability, and Computability. Conformance to these criteria provides a basis for pre-model scientific rigor and ethical integrity, mitigating downstream risks of bias and error prior to AI modeling. We apply and evaluate these standards across all four Bridge2AI flagship datasets, spanning functional genomics to clinical medicine, and encode them in machine-actionable metadata bound to the datasets.

This framework sets a benchmark for preparing ethical, reusable datasets in biomedical AI and provides standardized methods for reliable pre-model data evaluation.