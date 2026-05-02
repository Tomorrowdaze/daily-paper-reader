---
title: "NEURA: An agentic system for autonomous neuroimaging workflows"
title_zh: NEURA：一种用于自主神经影像工作流的智能系统
authors: "Xie, J., Wang, J., Wu, X., Liu, X., Mi, Y., Liu, Q., Xu, T., Liu, C., Chen, H., Guo, J."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.27.721217v1.full.pdf"
tags: ["query:profile-1"]
score: 6.0
evidence: 可追溯的推理和基于证据的分析计划
tldr: "本文提出NEURA，一个由大型语言模型驱动的智能系统，用于自动化处理神经影像学工作流程。它能从自然语言研究问题和多模态数据中生成分析计划、执行脚本和结果报告，并保持可追踪推理。实验显示其规划准确率达89.5%，在多项指标显著优于直接使用LLM查询，展示出在自动化、可扩展和可解释的脑影像研究中的潜力。"
source: biorxiv
selection_source: fresh_fetch
motivation: 神经影像分析需要跨学科深厚知识，造成学术与临床应用门槛过高。
method: 提出一个由大型语言模型驱动的智能代理系统NEURA，用于自动化设计和执行神经影像学工作流程。
result: "NEURA在规划准确率上达到89.5%，在工具选择和顺序等方面显著优于直接LLM查询，并在疾病案例中验证其可靠性。"
conclusion: NEURA实现了从研究管线自动化到可解释、可扩展的神经影像研究系统的重大进展。
---

## 摘要
神经影像学对于研究人类大脑至关重要；然而，其所需的深度跨学科研识使得入门门槛极高，从而限制了其更广泛的临床与科学应用。我们提出 NEURA，这是一种由大型语言模型（LLM）驱动的智能系统，用于自动化的神经影像工作流规划与分析。NEURA 能够处理自然语言研究问题及多模态神经影像数据集，生成基于证据的分析方案、可执行脚本、已验证的统计结果以及结构化报告，同时提供与中间产物及完整执行记录相连的可追踪推理路径。在经过精心构建的基准测试中，NEURA 的规划准确率达到 89.5%，显著优于直接基于 LLM 的查询，在规划准确率、工具选择及工具顺序方面分别平均提升了 30.5%、25.6% 和 36.7%。在脊髓小脑性共济失调 3 型（SCA3）的案例研究中，NEURA 能够自主识别出与既有病理和专家手动分析一致的小脑萎缩及异常弥散模式。总体而言，这些结果表明，我们的研究使神经影像学从传统的流程自动化迈向严谨、可扩展且可解释的研究系统。

## Abstract
Neuroimaging is essential for studying the human brain; however, the deep interdisciplinary expertise required imposes a very high threshold, limiting its broader clinical and scientific applications. We introduce NEURA, a large language model (LLM)-powered agentic system for automated neuroimaging workflow planning and analysis. NEURA processes free-text research questions and multimodal neuroimaging datasets to generate evidence-grounded analysis plans, executable scripts, validated statistical results and structured reports, with traceable reasoning linked to intermediate artefacts and full execution records. Through extensive evaluations on a curated benchmark, NEURA achieved an 89.5% planning accuracy and substantially outperformed direct LLM queries, with average gains of 30.5% in planning accuracy, 25.6% in tool selection and 36.7% in tool ordering. In case studies of spinocerebellar ataxia type 3, NEURA autonomously identified cerebellar atrophy and abnormal diffusivity patterns consistent with established pathologies and expert manual analyses. Collectively, these results demonstrate that our work advances from pipeline automation to rigorous, scalable and interpretable neuroimaging research systems.