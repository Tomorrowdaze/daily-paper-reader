---
title: Interpretable sequence-based machine learning consolidates candidate H3N2 hemagglutinin antigenic sites
title_zh: 可解释的基于序列的机器学习整合 H3N2 血凝素抗原位点候选
authors: "Meyer, A. G., Santillana, M."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721429v1.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 基于SHAP属性的可解释机器学习
tldr: 本研究通过可解释的序列基础机器学习模型，整合了H3N2血凝素潜在抗原位点的排名。利用梯度提升树和SHAP归因方法，研究在两种互补数据集上验证模型性能，既复现了已知关键抗原位点，又提升了不同分析之间的一致性，为流感疫苗株筛选提供数据驱动支持。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有流感H3N2血凝素抗原位点定义不一致，影响疫苗株选择，亟需整合性评估方法。
method: 使用可解释的梯度提升树模型结合SHAP分析，对两个H3N2血凝抑制数据集进行抗原位点重要性评估。
result: 模型在两套H3N2血凝抑制数据集上成功整合了抗原位点排名，既复现已知抗原簇转换位点，也提高了不同数据集间的一致性。
conclusion: 可解释的序列模型能在多数据源间生成更一致的抗原位点优先级，有助于流行病监测与疫苗设计。
---

## 摘要
季节性甲型流感病毒 A(H3N2) 的疫苗株选择依赖于识别哪些血凝素（HA）氨基酸替换最有可能削弱中和抗体识别。然而，已发表的抗原位点集合在关键位点的判定上存在显著分歧。我们采用可解释的基于序列的梯度提升树模型，并结合基于 SHAP 的位点归因方法，对两个互补的血凝抑制（HI）数据集进行分析，从而生成更为统一的候选抗原位点排序。基于 Neher/Bedford 基准数据集训练的模型成功复现了先前分析所揭示的经典簇转换位点。此外，在对 WIC 数据集进行混杂因素过滤后，我们的模型还复现了四个主要参考集合（Koel、Neher/Bedford、Harvey 和 Shah）中的大部分关键位点，并提升了从 Neher/Bedford 与 WIC 数据集得出的排名一致性。我们的模型所得排序与那些旨在预测取样时间或传代特征的模型更为一致，而与用于检测多样化选择的标准进化度量的相关性较低。结果表明，可解释的基于序列的模型能够在不同数据源与建模方法之间提供更整合的候选抗原位点排名。本研究有助于优先确定 H3N2 突变用于流行病监测。

## Abstract
Vaccine strain selection for seasonal influenza A(H3N2) depends on knowing which hemagglutinin (HA) substitutions are most likely to erode neutralizing antibody recognition, yet published antigenic site sets disagree substantially on which positions matter most. We applied interpretable gradient-boosted tree models with SHAP-based site attribution to two complementary hemagglutination inhibition (HI) datasets to produce a more consolidated ranking of candidate antigenic positions. Models trained on a Neher/Bedford benchmark dataset recover the canonical cluster-transition sites established by prior analyses. Moreover, after filtering the WIC dataset for confounding factors, our models recover the majority of positions from four major prior reference sets (Koel, Neher/Bedford, Harvey, and Shah) and improve concordance between rankings derived from the Neher/Bedford and WIC datasets. Rankings from our models also agree more strongly with models trained to predict sampling time or passage identity than with standard evolutionary metrics used to detect diversifying selection. Our results show that interpretable sequence-based models can provide a more integrative ranking of candidate antigenic positions across different data sources and modeling approaches. This work should aid efforts to prioritize H3N2 substitutions for epidemic surveillance.