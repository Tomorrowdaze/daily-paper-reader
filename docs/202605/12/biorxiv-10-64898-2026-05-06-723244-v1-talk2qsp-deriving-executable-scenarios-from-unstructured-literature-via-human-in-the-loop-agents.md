---
title: "Talk2QSP: Deriving Executable Scenarios from Unstructured Literature via Human-in-the-Loop Agents"
title_zh: Talk2QSP：通过人机交互智能体从非结构化文献中导出可执行场景
authors: "Kazemeini, A., Prieto, J., Balaji Kuttae, S., Siokis, A., Singh, G., Passban, P., Andreani, T."
date: 2026-05-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.06.723244v1.full.pdf"
tags: ["query:q6"]
score: 6.5
evidence: 用于模拟就绪模型干预的可执行因果系统
tldr: 本文提出Talk2QSP框架，用多智能体和人机交互机制自动从文献中提取并执行QSP场景，将非结构化描述转为可验证的模拟参数，在多模型和多场景测试中均取得可靠效果，显著增强QSP模型在药物研发中的可用性。
source: biorxiv
selection_source: fresh_fetch
motivation: 由于难以将文献中的非结构化场景准确转化为可重复、可模拟的QSP实验配置，限制了QSP模型的实际应用。
method: 采用基于大语言模型的场景提取器和双智能体场景映射器，并结合人机交互策略，将文本信息转化为参数变更。
result: 框架在四个ODE/QSP模型和七个专家标注场景中准确生成了全部可执行参数变更，涵盖复杂实验设计与不确定性处理。
conclusion: 通过人机协作和多智能体框架，成功将文献中的实验场景转化为可执行的QSP模型干预配置，提升了QSP在药物研发中的可操作性。
---

## 摘要
定量系统药理学（Quantitative Systems Pharmacology，QSP）模型在医药研究与开发中本质上发挥着干预性作用，作为可执行的因果系统，用于设计、评估和替代临床试验。然而，将 QSP 作为实验规划引擎进行部署仍受到限制，主要原因在于难以将非结构化文献中对临床或临床前场景的描述转化为可复现、可模拟的模型干预。针对这一问题，我们提出了一种基于智能体的框架，使 QSP 模型能够作为可干预实验系统运行，通过自动提取并执行源自文献的实验场景实现这一目的。该框架结合了模型实体的语义对齐、由大型语言模型（LLM）驱动的场景提取器（Scenario Extractor）以及双智能体场景映射器（Scenario Mapper）。与依赖不透明的一次性推理不同，我们的流程通过离散、可验证的工作指令将自由文本中的干预转换为精确的参数配置。此外，我们的动态人机交互（Human-in-the-Loop, HITL）策略使建模者能够以交互方式解决生物学歧义。在四种不同的动力学常微分方程（ODE）／QSP模型及七个由领域专家（SME）策划的文献场景上，我们的模型将所有选定场景正确转换为可执行的参数变动，其中包括多剂量干预、单位转换、空操作场景以及触发 HITL 的歧义情景。结果表明，专家与智能体系统之间的结构化协作能够成功解决单独依赖原始系统生物学标记语言（SBML）推理的 LLM 调用所无法可靠处理的场景。

## Abstract
Quantitative Systems Pharmacology (QSP) models play an inherently interventional role in pharmaceutical research and development, functioning as executable causal systems for designing, evaluating, and replacing clinical trials. However, deploying QSP as an experimental planning engine remains constrained by the difficulty of translating unstructured literature descriptions of clinical or preclinical scenarios into reproducible, simulation-ready model interventions. Motivated by this issue, we propose an agent-based framework that operationalizes QSP models as intervention-ready experimental systems by automatically extracting and executing literature-derived scenarios. The framework combines semantic grounding of model entities with a large language model (LLM)-driven Scenario Extractor and a dual-agent Scenario Mapper. Rather than relying on opaque, single-shot reasoning, our pipeline converts free-text interventions into precise parameter configurations through discrete, verifiable work orders. Moreover, our dynamic Human-in-the-Loop (HITL) strategy empowers modelers to resolve biological ambiguities interactively. Across four diverse kinetic ordinary differential equation (ODE)/QSP models and seven Subject Matter Expert (SME)-curated literature scenarios, our model resolved all selected scenarios into correct executable parameter changes, including multi-dose interventions, unit conversions, no-op scenarios, and ambiguity-triggered HITL cases, demonstrating that structured collaboration between experts and agentic systems can resolve scenarios that standalone raw Systems Biology Markup Language (SBML) reasoning LLM calls handle unreliably.