---
title: "BoYueGRN: Zero-shot causal discovery of directed gene regulatory networks from single-cell transcriptomes via amortized inference over synthetic structural causal models"
title_zh: BoYueGRN：通过在合成结构因果模型上的摊销推断，从单细胞转录组中零样本进行有向基因调控网络的因果发现
authors: "Wu, J., Shen, Y.-Q."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.15.745056v1.full.pdf"
tags: ["query:q6"]
score: 6.5
evidence: 该论文提出了一个使用结构因果模型进行机制分析的零样本因果发现框架。
tldr: BoYueGRN用合成因果模型的摊销推断，零样本从单细胞转录组推断定向GRN；一次前向输出边与方向，TF滑窗融合覆盖全转录组；在BEELINE与Perturb‑seq表现优异，支撑跨疾病图谱级调控动态重建。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-15-745056-v1/fig-001.webp\", \"caption\": \"Fig. 3 Zero-shot edge prediction on the BEELINE benchmark. 1080\", \"page\": 38, \"index\": 1, \"width\": 902, \"height\": 586}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-15-745056-v1/fig-002.webp\", \"caption\": \"Fig. 1 The BoYueGRN framework. 1042\", \"page\": 35, \"index\": 2, \"width\": 1009, \"height\": 1444}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-15-745056-v1/fig-003.webp\", \"caption\": \"Fig. 8 A reversible-to-irreversible regulatory state transition in 1164 periodontitis. 1165\", \"page\": 45, \"index\": 3, \"width\": 904, \"height\": 1215}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-15-745056-v1/fig-004.webp\", \"caption\": \"Fig. 2 Fidelity of the synthetic training distribution and task learnability. 1064\", \"page\": 37, \"index\": 4, \"width\": 904, \"height\": 544}]"
motivation: 现有单细胞GRN推断需逐数据集优化且难以判定因果方向，亟需可零样本、可泛化的定向推断方法。
method: BoYueGRN仅用1万合成结构因果模型进行摊销训练，单次前向输出边概率与方向，并以TF中心滑窗+非对称融合覆盖全转录组。
result: 在BEELINE基准零样本表现出色，两个全基因组CRISPRi Perturb‑seq上保留边的方向准确率达0.86和0.95，并重建五种疾病超27万细胞的细胞类型与阶段特异GRN动态。
conclusion: 该范式实现一次训练、跨数据集复用的定向GRN推断，摆脱逐数据集优化，为人类疾病图谱级调控动态系统化绘制与实验验证铺路。
---

## 摘要
传统上，基于单细胞RNA测序（RNA-seq）的基因调控网络（GRN）推断依赖于针对每个数据集的优化。现有工具必须为每个新数据集重新拟合，而且多数难以推断具有因果性的调控方向。我们在此提出 BoYueGRN，这是一种摊销的因果发现框架，仅在 10,000 个合成的结构因果模型上进行训练。对于任何未见过的数据集，一次前向传播即可返回边的概率与调控方向；同时，采用以转录因子（TF）为中心的滑动窗口结合不对称融合，将这一固定尺寸的模型扩展至覆盖整个转录组。BoYueGRN 在 BEELINE 基准测试中展现出强劲的零样本性能。在两个独立的全基因组 CRISPRi Perturb-seq 筛选实验中，所保留边的方向准确率分别达到 0.86 和 0.95。我们在五种疾病中重建了跨越超过 270,000 个细胞的细胞类型与阶段特异性的 GRN 动态，由此提出了可实验检验的生物学假设。BoYueGRN 将有向 GRN 推断重新表述为“一次训练、跨数据集复用”的范式。通过将网络重建与逐数据集优化解耦，这一范式为在人类疾病中系统化、图谱尺度地映射调控动态打开了大门。

## Abstract
Gene regulatory network (GRN) inference from single-cell RNA-seq conventionally relies on per-dataset optimization. Existing tools must be refit for every new dataset, and the majority fail to infer causal regulatory directions. Here we present BoYueGRN, an amortized causal discovery framework trained exclusively on 10,000 synthetic structural causal models. For any unseen dataset, a single forward pass returns edge probabilities and regulatory directions, while TF-centric sliding windows with asymmetric fusion extend this fixed-size model to full-transcriptome coverage. BoYueGRN demonstrates strong zero-shot performance across BEELINE benchmarks. On two independent genome-wide CRISPRi Perturb-seq screens, directional accuracy on retained edges reaches 0.86 and 0.95. Reconstructed cell-type- and stage-specific GRN dynamics across five diseases spanning more than 270,000 cells yield experimentally testable biological hypotheses. BoYueGRN reframes directed GRN inference as a train-once, reuse-across-datasets paradigm. By decoupling network reconstruction from per-dataset optimization, this paradigm opens the door to systematic, atlas-scale mapping of regulatory dynamics across human diseases.