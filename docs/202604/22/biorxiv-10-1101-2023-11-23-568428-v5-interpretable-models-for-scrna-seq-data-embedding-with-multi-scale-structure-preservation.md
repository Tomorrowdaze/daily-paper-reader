---
title: Interpretable models for scRNA-seq data embedding with multi-scale structure preservation
title_zh: 具有多尺度结构保留的可解释 scRNA-seq 数据嵌入模型
authors: "Novak, D., de Bodt, C., Lambert, P., Lee, J. A., Van Gassen, S., Saeys, Y."
date: 2026-04-17
pdf: "https://www.biorxiv.org/content/10.1101/2023.11.23.568428v5.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 用于高维数据嵌入和结构保留的可解释模型
tldr: 本文针对单细胞转录组数据降维中结构保真度不足的问题，提出了ViScore评分框架和ViVAE模型，前者提升了评价的公正性和可扩展性，后者结合深度学习实现多尺度结构保持与良好可解释性，显著提高了分析的可信度。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有降维方法在结构保真和评价标准的可靠性上存在不足，影响数据分析的可信度。
method: 提出了ViScore评分框架和ViVAE深度学习模型，用于保持单细胞转录组数据的多尺度结构并提升解释性。
result: 实验证明ViScore和ViVAE在多尺度结构保持和解释性方面优于现有方法。
conclusion: 研究提供了更可信且可解释的单细胞数据嵌入方法，有望成为降维分析的新标准。
---

## 摘要
在许多生物学研究中，高效探索高维单细胞转录组学数据的能力至关重要。因此，降维技术已成为分析工作流程的基本组成部分。它们生成低维嵌入，以捕捉数据中的重要结构，并常用于发现、质量控制和下游分析。然而，当前方法的可信度以及流行评估标准的严格性仍然有限。我们通过对结构保留型数据嵌入的实证研究来解决这一问题，并提供两种工具。首先，我们提出 ViScore：一个稳健的评分框架，改进了无监督和有监督的质量度量，重点关注可扩展性和公平性。其次，我们提出 ViVAE：一种深度学习模型，能够更好地保留多尺度结构，并配备新的可解释性工具。我们通过定量比较和针对性案例研究展示了这些成果提升单细胞降维可信度的潜力。

## Abstract
The ability to explore high-dimensional single-cell transcriptomics data efficiently is crucial in many biological studies. Dimensionality reduction techniques have therefore emerged as a basic building block of analytical workflows. They generate low-dimensional embeddings that capture important structures in the data, and are often used in discovery, quality control, and downstream analysis. However, the trustworthiness of current methods and the rigour of popular evaluation criteria are limited. We tackle this in an empirical study of structure-preserving data embeddings, delivering two tools. First, we introduce ViScore: a robust scoring framework that improves both unsupervised and supervised quality metrics, with emphasis on scalability and fairness. Second, we introduce ViVAE : a deep learning model that achieves better multi-scale structure preservation and is equipped with new tools for interpretability. We demonstrate the potential of these contributions to advance the trustworthiness of single-cell dimensionality reduction in a quantitative comparison and focused case studies.