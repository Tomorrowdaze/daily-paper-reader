---
title: Interpretable sequence-based machine learning consolidates candidate H3N2 hemagglutinin antigenic sites
title_zh: 可解释的基于序列的机器学习整合了H3N2血凝素候选抗原位点
authors: "Meyer, A. G., Santillana, M."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721429v1.full.pdf"
tags: ["query:q5"]
score: 6.5
evidence: 使用基于SHAP的可解释梯度提升树模型进行预测归因。
tldr: 本研究通过解释性序列机器学习模型分析两项血凝抑制数据集，整合不同文献中对H3N2血凝素抗原位点的差异性认知，以基于SHAP特征归因的方式生成一致的抗原位点排名，为流感疫苗毒株选择提供更可靠的参考。
source: biorxiv
selection_source: fresh_fetch
motivation: 为提高H3N2疫苗毒株选择中抗原位点识别的一致性和可靠性。
method: 采用可解释的梯度提升树模型及SHAP特征归因分析抗原位点重要性。
result: 模型成功整合不同数据集的抗原位点排名，提高了对H3N2血凝素抗原变异的理解。
conclusion: 解释性机器学习能增强不同数据源间抗原位点排名一致性，助力流感监测与疫苗设计。
---

## 摘要
季节性流感A(H3N2)的疫苗毒株选择依赖于识别那些最可能削弱中和抗体识别的血凝素（HA）替代位点，然而已发表的抗原位点集在关键位点的定义上存在显著分歧。我们采用具有可解释性的梯度提升树模型，并结合基于SHAP的位点归因分析，对两个互补的血凝抑制（HI）数据集进行研究，从而获得更为统一的候选抗原位点排序。基于Neher/Bedford基准数据集训练的模型能够再现先前分析所建立的典型簇转变位点。此外，在对WIC数据集过滤掉混杂因素后，我们的模型成功恢复了来自四个主要参考集（Koel、Neher/Bedford、Harvey和Shah）的大部分位点，并提高了从Neher/Bedford和WIC数据集导出的排序之间的一致性。我们的模型所得排名与那些用于预测采样时间或传代身份的模型相比，一致性更高，而与标准的用于检测多样化选择的进化度量的相关性则较低。结果表明，可解释的基于序列的模型能够在不同的数据来源和建模方法间提供更具整合性的候选抗原位点排序。本研究有助于改进H3N2替代位点的优先级评估，以支持流行病监测工作。

## Abstract
Vaccine strain selection for seasonal influenza A(H3N2) depends on knowing which hemagglutinin (HA) substitutions are most likely to erode neutralizing antibody recognition, yet published antigenic site sets disagree substantially on which positions matter most. We applied interpretable gradient-boosted tree models with SHAP-based site attribution to two complementary hemagglutination inhibition (HI) datasets to produce a more consolidated ranking of candidate antigenic positions. Models trained on a Neher/Bedford benchmark dataset recover the canonical cluster-transition sites established by prior analyses. Moreover, after filtering the WIC dataset for confounding factors, our models recover the majority of positions from four major prior reference sets (Koel, Neher/Bedford, Harvey, and Shah) and improve concordance between rankings derived from the Neher/Bedford and WIC datasets. Rankings from our models also agree more strongly with models trained to predict sampling time or passage identity than with standard evolutionary metrics used to detect diversifying selection. Our results show that interpretable sequence-based models can provide a more integrative ranking of candidate antigenic positions across different data sources and modeling approaches. This work should aid efforts to prioritize H3N2 substitutions for epidemic surveillance.