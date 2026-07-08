---
title: "Identifying intervention strategies from machine learning models with COALA: a counterfactual optimization framework"
title_zh: 利用 COALA 从机器学习模型中识别干预策略：一种反事实优化框架
authors: "Han, B., Duan, Q., Hu, T."
date: 2026-07-07
pdf: "https://www.biorxiv.org/content/10.1101/2025.07.18.664723v2.full.pdf"
tags: ["query:q6"]
score: 7.5
evidence: 用于机器学习中可操作解释性的反事实优化框架
tldr: 本文提出面向生物医学机器学习模型解释的COALA框架，通过反事实优化寻找可执行干预策略，并在用户定义的可变特征集合上分析不同特征约束对最优干预的影响。相比传统SHAP等方法只强调特征重要性，COALA更关注多特征组合形成的整体模式。实验表明，该方法在合成与真实数据上均能揭示复杂模型规律，并生成更直观、可操作的多特征干预建议。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有可解释AI方法多停留在特征重要性层面，难以解释复杂模式形成原因及提供可执行的健康干预建议。
method: 研究提出COALA框架，在用户定义的可变特征子集上搜索最优反事实，并通过约束其他特征分析干预策略与特征组合关系。
result: 在合成与真实数据实验中，COALA能够识别简单和复杂模型规律，并相比SHAP提供更直观、多特征联动的干预方案。
conclusion: COALA通过基于反事实的全局优化与特征约束分析，为复杂生物医学模型提供了更具可操作性和整体性的解释框架。
---

## 摘要
研究动机：生物医学中的机器学习模型日益复杂，常常如同“黑箱”一般。然而，要理解疾病的致病因素并制定可执行的健康干预措施，就需要具有可解释性的模型。常见的可解释人工智能方法（如 SHAP）侧重于特征重要性，但难以解释为何特征会以特定模式产生作用，以及应采取何种干预措施。反事实解释通过提出“如果……会怎样”的情景来解决这一问题，但现有工具主要关注个体预测，无法泛化复杂趋势。研究结果：我们提出了“面向可执行可解释性的反事实优化框架”（Counterfactual Optimization for Actionable interpretabiLity in AI，COALA）。COALA 通过在用户定义的可变特征子集上识别最优反事实，并对其余特征施加约束，从而揭示约束特征如何决定最优干预措施。通过分析特征的反事实画像而非单个特征，COALA 能够揭示整体性模式。基于合成数据集和真实数据集的实验表明，COALA 能揭示简单与复杂模型中的趋势，并提供比 SHAP 更直观的多特征干预方案。可获取性与实现：COALA 的实现代码、合成数据、基于合成数据训练的模型，以及复现实验结果和图表的代码可在 https://github.com/brt-solo/COALA 获取。

## Abstract
Motivation: Machine learning models in biomedicine have become increasingly complex, often functioning as black boxes. However, understanding contributors to disease and making actionable health interventions requires interpretable models. Common explainable AI methods like SHAP focus on feature importance but fall short in explaining why features contribute in certain patterns or what interventions to take. Counterfactual explanations address this by proposing "what if" scenarios but current tools focus on individual predictions and fail to generalize complex trends. Results: We introduce the framework Counterfactual Optimization for Actionable interpretabiLity in AI (COALA). COALA interprets models by identifying optimal counterfactuals across user-defined mutable feature subsets and constraining remaining features to reveal how constraint features determine what interventions are optimal. By analyzing counterfactual profiles of features rather than individual features, COALA reveals holistic patterns. Using synthetic and real datasets, COALA reveals simple and complex model trends and provides more intuitive, multi-feature interventions than SHAP. Availability and Implementation: Code for COALA implementation, synthetic data, models trained on synthetic data, and code to replicate results and figures are available at https://github.com/brt-solo/COALA.