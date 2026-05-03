---
title: Interpretable sequence-based machine learning consolidates candidate H3N2 hemagglutinin antigenic sites
title_zh: 可解释的基于序列的机器学习整合了 H3N2 血凝素候选抗原位点
authors: "Meyer, A. G., Santillana, M."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721429v1.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 基于SHAP归因的可解释机器学习模型
tldr: 本文通过可解释的机器学习方法（梯度提升树及SHAP分析）对两个H3N2血凝素数据集进行研究，整合并统一不同文献定义的抗原位点排名，为流感疫苗株选择及抗原监测提供新的数据驱动依据。
source: biorxiv
selection_source: fresh_fetch
motivation: 不同已发表的抗原位点定义在H3N2血凝素上的关键位点认定差异巨大，需要统一和整合。
method: 利用可解释的梯度提升树模型及SHAP方法分析两种血凝抑制数据集，确定候选的抗原位点。
result: 模型在基准数据集上准确恢复已知关键位点，并在经过过滤的WIC数据集中与多个参考位点集高度一致。
conclusion: 可解释的序列模型可整合不同数据源与分析方法，提供更一致的H3N2抗原位点排名，有助于流感疫情监测与疫苗选株。
---

## 摘要
季节性流感 A(H3N2) 疫苗毒株的选择取决于了解哪些血凝素（HA）替换最可能削弱中和抗体的识别。然而，已发表的抗原位点集合在最重要的位置上存在显著分歧。我们将基于序列的可解释梯度提升树模型与基于 SHAP 的位点归因应用于两个互补的血凝抑制（HI）数据集，以生成更一致的候选抗原位点排序。利用 Neher/Bedford 基准数据集训练的模型可以复现先前分析所确定的典型簇转换位点。此外，在对 WIC 数据集进行混杂因素过滤后，我们的模型能够复现四个主要参考集合（Koel、Neher/Bedford、Harvey 和 Shah）中的大多数位点，并提升了从 Neher/Bedford 和 WIC 数据集导出的排序之间的一致性。我们的模型所得排序与用于预测采样时间或传代身份的模型相比，与标准检测多样化选择的进化指标的一致性更强。我们的结果表明，可解释的基于序列的模型能够在不同数据源和建模方法之间提供更综合的候选抗原位点排序。本研究有助于优先筛选用于流行监测的 H3N2 替换。

## Abstract
Vaccine strain selection for seasonal influenza A(H3N2) depends on knowing which hemagglutinin (HA) substitutions are most likely to erode neutralizing antibody recognition, yet published antigenic site sets disagree substantially on which positions matter most. We applied interpretable gradient-boosted tree models with SHAP-based site attribution to two complementary hemagglutination inhibition (HI) datasets to produce a more consolidated ranking of candidate antigenic positions. Models trained on a Neher/Bedford benchmark dataset recover the canonical cluster-transition sites established by prior analyses. Moreover, after filtering the WIC dataset for confounding factors, our models recover the majority of positions from four major prior reference sets (Koel, Neher/Bedford, Harvey, and Shah) and improve concordance between rankings derived from the Neher/Bedford and WIC datasets. Rankings from our models also agree more strongly with models trained to predict sampling time or passage identity than with standard evolutionary metrics used to detect diversifying selection. Our results show that interpretable sequence-based models can provide a more integrative ranking of candidate antigenic positions across different data sources and modeling approaches. This work should aid efforts to prioritize H3N2 substitutions for epidemic surveillance.