---
title: Autoresearch Discovery of Interpretable Filter Rules for Antibody Binder Classification
title_zh: 用于抗体结合物分类的可解释过滤规则的自动研究发现
authors: "Landajuela, M."
date: 2026-05-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.05.723069v1.full.pdf"
tags: ["query:q5"]
score: 6.5
evidence: 使用自动化研究循环发现用于分类的可解释过滤规则
tldr: 该研究针对抗体设计中筛选瓶颈问题，提出一个自我研究循环系统，迭代生成和评估无训练的筛选规则。在七个抗体-抗原系统上取得显著性能提升，最终RMSD调优三联规则在保持可解释性的同时接近最强LLM性能，展示了自动化自研究发现可解释筛选规则的潜力。
source: biorxiv
selection_source: fresh_fetch
motivation: 抗体设计中候选数量庞大但实验验证稀少，使得如何无训练地高效筛选成为关键问题。
method: 研究采用一个自我研究循环，迭代提出并评估抗体筛选规则变体，通过版本控制记录结果并指导改进。
result: 最终发现的RMSD调优三联规则在七个系统上平均ROC-AUC提升至0.8060，优于多种机器学习和LLM基线。
conclusion: 该研究证明了系统化的自我研究可从简单结构置信度信号中发现紧凑且可解释的抗体筛选规则，在有限数据条件下也具有较强性能。
---

## 摘要
抗体设计过程通常在能够进行实验验证之前生成大量候选分子，因此候选筛选成为关键瓶颈。我们研究了一个“自动研究（autoresearch）”循环是否能够无需训练地发现更优的抗体结合物分类过滤规则。该循环通过迭代提出规则变体，在固定的“Leave-One-System-Out”协议下进行评估，在版本控制系统中记录每次实验，并利用结果指导下一次迭代。在七个抗体-抗原系统上记录的 75 个唯一过滤规则变体中，该循环将平均 ROC-AUC 从初始基线的 0.6371 提升至精炼后的“RMSD 调谐三元组（RMSD-Tuned Triad）”规则的 0.8060，取得了 0.1689 的绝对提升和 26.5% 的相对改善。所发现的过滤规则在性能上可与监督式机器学习基线及提示式大型语言模型（LLM）基线竞争：它优于逻辑回归（0.7144）、特征选择后的平衡逻辑回归（0.7536）以及 GPT-4o 表格少样本提示（0.7640），并且与最强的 GPT-5 表格少样本结果（0.8104）仅差 0.0044 ROC-AUC。与 LLM 基线不同的是，最终规则在获得数值结构导出的特征后，不需要提示样例，也不需要进行 LLM 推理。这些结果表明，系统化的自动研究可以将简单的结构置信度信号转化为紧凑、可解释的过滤规则，在目标特异性训练数据稀缺时具有实际价值。

## Abstract
Antibody design campaigns increasingly generate many candidates before only a small subset can be tested experimentally, making candidate filtering a central bottleneck. We study whether an autoresearch loop can discover better training-free filters for antibody binder classification by iteratively proposing rule variants, evaluating them under a fixed Leave-One-System-Out protocol, recording each experiment in version control, and using the results to guide the next iteration. Across 75 unique logged filter variants on seven antibody-antigen systems, the loop improves average ROC-AUC from 0.6371 for the initial baseline to 0.8060 for a compact final rule that we call the RMSD-Tuned Triad rule, an absolute gain of 0.1689 and a relative improvement of 26.5%. The discovered filter is competitive with supervised machine learning baselines and prompted LLM baselines evaluated on the same systems: it exceeds logistic regression (0.7144), feature-selected balanced logistic regression (0.7536), and GPT-4o tabular few-shot prompting (0.7640), and it comes within 0.0044 ROC-AUC of the strongest GPT-5 tabular few-shot result (0.8104). Unlike the LLM baseline, the final rule requires no prompted examples and no LLM inference once the numeric structure-derived features are available. These results show that systematic autoresearch can turn simple structural-confidence signals into compact, interpretable filters that are useful when target-specific training data are scarce.