---
title: "RulePep: Interpretable ESM-Guided Neural-Symbolic Peptide Classification"
title_zh: RulePep：可解释的 ESM 引导神经符号肽分类方法
authors: "Midjani, F., Ghelich, R., Keshtkar, F. Z., Malekpour, M., Lee, H."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.03.736448v1.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 用于风险预测的可解释神经符号分类
tldr: RulePep是一种结合ESM-2蛋白语言模型与神经符号推理的可解释肽分类框架，针对肽功能预测中“高性能但黑盒化”的问题，引入潜在谓词、极性约束规则与可加符号logit，实现对预测依据的规则级解释与审计。该方法在血脑屏障穿透、溶血性和抗癌肽分类任务上均取得具有竞争力的AUROC和MCC表现，同时兼顾预测准确性与透明性。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有基于蛋白语言模型的肽分类方法虽然准确率高，但预测过程缺乏可解释性，难以明确哪些序列特征支持或反对分类结果。
method: 该方法以冻结的ESM-2序列表征为输入，通过潜在谓词、极性约束可微规则和可加符号logit构建神经符号分类器，实现可解释预测。
result: 在血脑屏障穿透、溶血性和抗癌肽三个数据集上，RulePep分别取得0.8869、0.9155和0.9765的AUROC，并在MCC指标上表现优异，消融实验验证了各模块有效性。
conclusion: RulePep在保持高分类性能的同时提供可解释的规则级证据与审计能力，为透明化肽功能预测和候选筛选提供了有效框架。
---

## 摘要
肽类正日益被探索为治疗候选物、递送载体和功能性生物分子，但由于序列空间巨大且微小的序列变化即可改变功能性，对肽活性与安全性的实验筛选仍然成本高昂。因此，计算肽分类方法能够帮助优先筛选候选物。然而，许多基于蛋白质语言模型的分类器虽然具有较强性能，却依赖不透明的预测头，使得难以确定哪些学习到的证据支持或反对某一预测。我们提出了 RulePep，一种由 ESM-2 引导的神经符号肽功能预测分类器。RulePep 将冻结的 ESM-2 序列表征映射为学习得到的潜在谓词、受极性约束的可微规则，以及可在个案层面进行检视的加性符号 logit 组件。我们在三个生物学性质不同的肽分类任务上评估了 RulePep：血脑屏障穿透能力、溶血效力以及抗癌活性。在 BBPpredict、HemoPI3 和 AntiCP 2.0 的替代基准数据集上，RulePep 分别取得了 0.8869/0.6850、0.9155/0.6820 和 0.9765/0.8633 的 AUROC/MCC 值。消融实验支持了多层表示池化、规则极性、挖掘规则初始化、符号容量以及基于规则的聚合机制的贡献。RulePep 将具有竞争力的预测性能与加性 logit 重构、规则级证据报告以及谓词抑制审计相结合，为肽候选物优先筛选提供了一个透明的基于序列的框架。

## Abstract
Peptides are increasingly explored as therapeutic candidates, delivery vectors, and functional biomolecules, but experimental screening of peptide activity and safety remains costly because the sequence space is vast and small sequence changes can alter functionality. Computational peptide classification can therefore help prioritize candidates. However, many protein-language-model-based classifiers achieve strong performance using opaque prediction heads, making it difficult to determine which learned evidence supports or opposes a prediction. We present RulePep, an ESM-2-guided neural-symbolic classifier for peptide-function prediction. RulePep maps frozen ESM-2 sequence representation to learned latent predicates, polarity-constrained differentiable rules, and an additive symbolic logit whose components can be inspected at the case level. We evaluate RulePep on three biologically distinct peptide classification tasks: blood-brain barrier penetration, hemolytic potency, and anticancer activity. On the BBPpredict, HemoPI3, and AntiCP 2.0 alternate benchmark datasets, RulePep achieved AUROC/MCC values of 0.8869/0.6850, 0.9155/0.6820, and 0.9765/0.8633, respectively. Ablation experiments supported the contributions of multi-layer representation pooling, rule polarity, mined-rule initialization, symbolic capacity, and rule-derived aggregation. RulePep combines competitive predictive performance with additive logit reconstruction, rule-level evidence reporting, and predicate-suppression auditing, providing a transparent sequence-based framework for peptide candidate prioritization.