---
title: Interpretable models for scRNA-seq data embedding with multi-scale structure preservation
title_zh: 具备多尺度结构保持的可解释单细胞 RNA 测序数据嵌入模型
authors: "Novak, D., de Bodt, C., Lambert, P., Lee, J. A., Van Gassen, S., Saeys, Y."
date: 2026-04-17
pdf: "https://www.biorxiv.org/content/10.1101/2023.11.23.568428v5.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 高维数据嵌入的可解释模型
tldr: 本文针对单细胞转录组学数据分析中降维结果可信度不足的问题，提出了ViScore评分框架以改进质量指标的公正性与可扩展性，并提出可解释的深度学习模型ViVAE以更好地保持多尺度数据结构，从而提升单细胞数据嵌入的可靠性。
source: biorxiv
selection_source: fresh_fetch
motivation: 当前单细胞转录组学高维数据的降维方法在结构保持性和评估指标的可靠性方面存在不足。
method: 研究提出了ViScore评分框架与ViVAE深度模型来优化降维的结构保持性与可解释性。
result: ViVAE在多尺度结构保持和解释性上表现优异，ViScore提供了更公平、可扩展的质量评估。
conclusion: 研究提高了单细胞降维的可信度，促进了高维生物数据的可解释分析。
---

## 摘要
高效探索高维单细胞转录组学数据的能力在众多生物学研究中至关重要。因此，降维技术已成为分析流程的基本组成部分。这些方法生成的低维嵌入能够捕捉数据中的重要结构，常用于发现、质量控制及下游分析。然而，当前方法的可靠性以及常用评估标准的严格性仍然有限。我们通过对结构保持型数据嵌入的实证研究来解决这一问题，并提出了两种工具。首先，我们介绍 ViScore：一种稳健的评分框架，改进了无监督与有监督的质量度量，重点关注可扩展性与公平性。其次，我们提出 ViVAE：一种能够实现更优多尺度结构保持并配备新型可解释性工具的深度学习模型。我们通过定量比较与重点案例研究展示了这些工作在提升单细胞降维可信度方面的潜力。

## Abstract
The ability to explore high-dimensional single-cell transcriptomics data efficiently is crucial in many biological studies. Dimensionality reduction techniques have therefore emerged as a basic building block of analytical workflows. They generate low-dimensional embeddings that capture important structures in the data, and are often used in discovery, quality control, and downstream analysis. However, the trustworthiness of current methods and the rigour of popular evaluation criteria are limited. We tackle this in an empirical study of structure-preserving data embeddings, delivering two tools. First, we introduce ViScore: a robust scoring framework that improves both unsupervised and supervised quality metrics, with emphasis on scalability and fairness. Second, we introduce ViVAE : a deep learning model that achieves better multi-scale structure preservation and is equipped with new tools for interpretability. We demonstrate the potential of these contributions to advance the trustworthiness of single-cell dimensionality reduction in a quantitative comparison and focused case studies.