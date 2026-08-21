---
title: "Mantpy: a framework for extracellular matrix analysis in spatial proteomics"
title_zh: Mantpy：空间蛋白质组学中的细胞外基质分析框架
authors: "Ghafoor, M., Parkinson, J. E., Pham, T., Georgaka, S., Hayley, M. J., Jokl, E., Hanley, K. P., Allen, J. E., Sutherland, T. E., Rattray, M."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.04.657781v4.full.pdf"
tags: ["query:q5"]
score: 6.0
evidence: 支持用于空间分析的可解释图深度学习
tldr: 空间蛋白组学已能原位同时观测细胞与细胞外基质，但现有分析偏向细胞；Mantpy将ECM及其与细胞的界面建模为空间图，从标记直接构建ECM图并与细胞图联通，支持图统计、可解释图学习与可视化；在肠、肝、肺数据中重建分层结构、解析感染相关基质变化并刻画细胞-基质关联，且与scverse互操作并发布配套数据。
source: biorxiv
selection_source: fresh_fetch
motivation: 空间蛋白组学同时捕获细胞与ECM，但现有工具偏向细胞，难以系统解析基质的组成、结构与细胞互作。
method: 提出Mantpy，将ECM及其与细胞的界面表示为空间图，从ECM标记直接构建ECM图并与细胞图相连，支持图统计、可解释图深度学习与可视化，兼容scverse。
result: 在人体肠道、感染小鼠肝脏与小鼠肺数据上，Mantpy重建分层组织结构，解析感染相关基质组成与组织学变化，并刻画细胞-基质关联。
conclusion: Mantpy把空间分析的基本单元从细胞扩展到包围它的基质，并随附ECM数据集以推动联合细胞-基质研究。
---

## 摘要
空间蛋白质组学技术现已能在原位同时解析细胞和细胞外基质（ECM）。然而，尽管ECM在健康与疾病中发挥着至关重要的作用，现有分析工具仍以细胞为中心。在此我们提出 Mantpy，这一框架将ECM及其与细胞的界面表示为空间图。Mantpy 直接基于基质标记物构建ECM图，并将其与细胞图相连以开展细胞-ECM联合分析，支持图统计、可解释的基于图的深度学习以及可视化。从单一ECM标记物到ECM与细胞标记物的多重面板，Mantpy 能在人类肠道中重建分层的组织架构，在感染小鼠肝脏中解析与疾病相关的基质组成与组织结构，并在小鼠肺中表征细胞-基质关联。伴随包含ECM的数据集发布并与 scverse 生态系统互操作，Mantpy 将空间分析的基本单元从细胞拓展至包围它的基质。

## Abstract
Spatial proteomics technologies now profile cells and the extracellular matrix (ECM) together in situ. Yet analysis tools remain cell-centric, despite the ECM playing an essential role in health and disease. Here we present Mantpy, a framework that represents the ECM, and its interface with cells, as spatial graphs. Mantpy builds ECM graphs directly from matrix markers and links them with cell graphs for joint cell-ECM analysis, supporting graph statistics, explainable graph deep learning and visualisation. From a single ECM marker to multiplexed panels of ECM and cellular markers, Mantpy recovers layered tissue architecture in human intestine, resolves disease-associated matrix composition and organisation in infected mouse liver, and characterises cell-matrix associations in mouse lung. Released with ECM-inclusive datasets and interoperating with the scverse ecosystem, Mantpy extends the unit of spatial analysis beyond the cell, to the matrix that surrounds it.