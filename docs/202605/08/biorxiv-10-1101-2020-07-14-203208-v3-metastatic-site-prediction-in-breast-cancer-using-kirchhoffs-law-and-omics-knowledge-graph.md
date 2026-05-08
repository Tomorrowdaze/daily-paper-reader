---
title: "Metastatic Site Prediction in Breast Cancer using Kirchhoff's Law and Omics Knowledge Graph"
title_zh: 利用基尔霍夫定律与组学知识图预测乳腺癌的转移部位
authors: "Jha, A., Khan, Y., Sahay, R., d'Aquin, M."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.1101/2020.07.14.203208v3.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 使用知识图谱保留预测的机制结构
tldr: 本文提出Kirchhoff知识图谱（K-KG），将电路守恒定律融入图推理，构建多层次癌症决策网络，实现跨多组学层次的信息流守恒与拓扑特征挖掘。结合图卷积网络，该方法在乳腺癌转移部位预测中显著优于现有模型，为多组学机制解析提供新方向。
source: biorxiv
selection_source: fresh_fetch
motivation: 为解决现有乳腺癌转移预测模型忽视多部位、多组学和多模态生物复杂性的局限。
method: 提出Kirchhoff知识图谱框架，结合电路守恒定律、拓扑子结构挖掘及图卷积网络实现多组学数据融合预测。
result: 在多项独立数据集中K-KG模型在预测复发和特定位点转移上表现优异，AUC最高达0.87，显著优于传统模型。
conclusion: 该研究证明基于Kirchhoff定律的知识图谱方法能有效捕捉多组学信息流，显著提升乳腺癌转移部位预测的准确性。
---

## 摘要
从原发肿瘤预测乳腺癌（BRCA）及更广泛的转移性疾病的转移解剖部位仍然是一个未解决的问题。这一困难具有结构性：转移生物学涉及多部位（骨、肺、肝、脑）、多组学（基因组学、蛋白质组学、甲基组学、药物反应）以及多模态（CNV、基因表达、DNA甲基化、通路、临床关联）。现有分类器要么将这种异质性压缩为单个特征向量，要么仅依赖单一组学层，二者都丢弃了驱动转移趋向性的机制结构。我们提出了 Kirchhoff 知识图（K-KG），这是一个将电路理论中的守恒定律引入知识图推理的框架。我们的主要贡献包括：（1）一个分层的 RDF 癌症决策网络，整合了 36 个多组学数据集，涵盖突变、通路、药物、疾病及反应；（2）两个新的守恒定律——知识图电压定律（KGVL）和知识图电流定律（KGCL），用于调控遍历过程中的信息流动，并提供图完整性的原理性度量；（3）在守恒图上进行拓扑结构基序挖掘，以识别重新连线标志转移转变的三角子结构，从而替代基于表达的特征选择；（4）一个图卷积神经网络，其隐藏层即为组学层，用于将特定转移部位的预测表示为连续百分比而非二元标签。在 TCGA-BRCA 训练集以及一个验证集和来自 GEO 的四个独立测试队列中，K-KG 实现在复发预测中 83.8% 的 AUC，以及在脑部特异性预测中最高 0.87 AUC / 0.91 F1，较随机森林、神经网络和 SVM 基线模型提升 8–20 个 AUC 点。据我们所知，这是 Kirchhoff 定律（1845、1847）首次应用于基于图的机器学习，也是首个返回按转移部位贡献谱而非单一标签的转移预测模型。

## Abstract
Predicting the anatomical site of metastasis from a primary tumour remains an unsolved problem in breast cancer (BRCA) and metastatic disease more broadly. The difficulty is structural: metastatic biology is multi-site (bone, lung, liver, brain), multi-omics (genomics, proteomics, methylomics, drug response), and multi-modal (CNV, gene expression, DNA methylation, pathways, clinical associations). Existing classifiers either collapse this heterogeneity into a single feature vector or rely on a single omics layer, both of which discard the mechanistic structure that drives metastatic tropism. We introduce Kirchhoff Knowledge Graphs (K-KG), a framework that imports the conservation laws of electrical-circuit theory into knowledge graph reasoning. Our contributions are: (1) a layered RDF Cancer Decision Network integrating 36 polyomics datasets across mutations, pathways, drugs, diseases, and reactions; (2) two novel conservation laws - the Knowledge-Graph Voltage Law (KGVL) and Knowledge-Graph Current Law (KGCL) - that govern information flow during traversal and yield a principled measure of graph completeness; (3) topological motif mining on the conserved graph, replacing expression-based feature selection by identifying triangular sub-structures whose rewiring marks metastatic transition; (4) a Graph Convolutional Neural Network whose hidden layers are the omics layers themselves, predicting site-specific metastasis as a continuous percentage rather than a binary label. On TCGA-BRCA training plus one validation and four independent test cohorts from GEO, K-KG achieves 83.8% AUC for relapse prediction and up to 0.87 AUC / 0.91 F1 for brain-site-specific prediction, outperforming Random Forest, Neural Network, and SVM baselines by 8-20 AUC points. To our knowledge this is the first application of Kirchhoff's laws (1845, 1847) to graph-based machine learning, and the first metastasis predictor that returns a per-site contribution profile rather than a single label.