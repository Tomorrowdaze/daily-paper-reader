---
title: "NEURA: An agentic system for autonomous neuroimaging workflows"
title_zh: NEURA：一种用于自主神经影像学工作流程的智能代理系统
authors: "Xie, J., Wang, J., Wu, X., Liu, X., Mi, Y., Liu, Q., Xu, T., Liu, C., Chen, H., Guo, J."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.27.721217v1.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 可追溯的推理和基于证据的分析计划
tldr: 本文提出了一个名为NEURA的系统，它利用大型语言模型实现自主的神经影像学工作流程，从研究问题和多模态数据中生成分析方案、脚本和结果报告，并在准确率与性能上明显超越传统LLM查询。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统神经影像研究需要高度跨学科的专业知识，限制了其广泛应用，因此需要更智能的自动化系统来降低研究门槛。
method: 作者构建了一个由大型语言模型驱动的智能系统，用于自动生成并执行神经影像分析工作流程。
result: "NEURA在基准测试中达到89.5%的规划准确率，显著优于直接LLM查询，并在真实病例中成功识别相关病理特征。"
conclusion: NEURA展示了从流程自动化到可解释、可扩展的神经影像研究系统的重大进步。
---

## 摘要
神经影像学是研究人类大脑的重要手段；然而，它所需的深度跨学科专业知识设置了极高的门槛，限制了其在更广泛的临床和科学领域中的应用。我们介绍 NEURA——一个由大型语言模型（LLM）驱动的自主型系统，用于自动化神经影像学工作流程的规划与分析。NEURA 能够处理自由文本研究问题和多模态神经影像数据集，生成基于证据的分析方案、可执行脚本、经过验证的统计结果以及结构化报告，并提供与中间产物和完整执行记录相链接的可追溯推理过程。通过在一个精心整理的基准上进行广泛评估，NEURA 实现了 89.5% 的规划准确率，显著优于直接基于 LLM 的查询，规划准确率平均提升 30.5%，工具选择准确率提升 25.6%，工具顺序正确率提升 36.7%。在脊髓小脑性共济失调第 3 型（spinocerebellar ataxia type 3）的案例研究中，NEURA 能够自主识别与已知病理及专家人工分析一致的小脑萎缩和异常弥散模式。这些结果表明，我们的工作使神经影像研究系统从单纯的流程自动化迈向严格、可扩展且具有可解释性的全新阶段。

## Abstract
Neuroimaging is essential for studying the human brain; however, the deep interdisciplinary expertise required imposes a very high threshold, limiting its broader clinical and scientific applications. We introduce NEURA--a large language model (LLM)-powered agentic system for automated neuroimaging workflow planning and analysis. NEURA processes free-text research questions and multimodal neuroimaging datasets to generate evidence-grounded analysis plans, executable scripts, validated statistical results and structured reports, with traceable reasoning linked to intermediate artefacts and full execution records. Through extensive evaluations on a curated benchmark, NEURA achieved an 89.5% planning accuracy and substantially outperformed direct LLM queries, with average gains of 30.5% in planning accuracy, 25.6% in tool selection and 36.7% in tool ordering. In case studies of spinocerebellar ataxia type 3, NEURA autonomously identified cerebellar atrophy and abnormal diffusivity patterns consistent with established pathologies and expert manual analyses. Collectively, these results demonstrate that our work advances from pipeline automation to rigorous, scalable and interpretable neuroimaging research systems.