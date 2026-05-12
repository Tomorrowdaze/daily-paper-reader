---
title: "Entropy Sorting Feature Selection: information-theoretic gene set identification improves single-cell RNA sequencing data interpretability"
title_zh: 熵排序特征选择：信息论驱动的基因集识别提升单细胞RNA测序数据的可解释性
authors: "Radley, A., Boezio, G., Shand, C., Perez-Carrasco, R., Briscoe, J."
date: 2026-05-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.26.701684v2.full.pdf"
tags: ["query:q6"]
score: 6.0
evidence: 通过信息论特征选择提高数据可解释性
tldr: 本研究针对单细胞RNA测序数据特征选择方法不足的问题，提出了熵排序特征选择（ESFS）框架。该方法通过信息论原理全面筛选关键基因，提高数据可解释性，在胚胎发育、肿瘤微环境及神经系统分析中均展现出优异效果。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有单细胞RNA测序数据分析在特征选择方面方法有限，难以充分提取生物学信号。
method: 研究提出了熵排序特征选择（ESFS）这一模块化、易用的信息论框架，用于筛选关键基因特征。
result: ESFS在多种数据集中显著提升了解释力，揭示了被传统方法忽略的复杂表达动态。
conclusion: ESFS确立了熵排序这一信息论框架，为单细胞数据的深入解析提供了新的思路。
---

## 摘要
单细胞RNA测序（scRNA-seq）极大地提升了我们解析细胞异质性的能力，但由于技术噪声和批次效应，提取有意义的信号仍然具有挑战性。多数用于去噪scRNA-seq数据的方法集中于使用主成分分析或深度学习等潜在表示来突出生物学信号。相比之下，尽管特征选择对后续分析具有显著影响，却较少受到关注，导致广泛依赖于相对简单的高变异基因选择策略。在此我们提出了熵排序特征选择（Entropy Sorting Feature Selection, ESFS），这是一个模块化且用户友好的框架，可显著提高scRNA-seq数据的可解释性。值得注意的是，ESFS能够揭示在潜在表示中被掩盖的复杂表达动态。我们在多种数据中展示了ESFS的实用性：在无需批次整合的情况下识别八个独立人类胚胎数据集中的一致发育程序；解析传统分析未能检测到的小鼠结肠空间基因表达；区分胶质母细胞瘤中的共享和肿瘤特异性微环境；以及分离小鼠发育中神经管的空间、时间和神经发生程序。我们的研究不仅提供了一个强大且易用的软件，用于深入理解复杂生物系统，还确立了熵排序作为一种新颖的信息论方法，可用于高级数据分析。

## Abstract
Single-cell RNA sequencing (scRNA-seq) has transformed our ability to resolve cellular heterogeneity, but extracting meaningful signals remains challenging due to technical noise and batch effects. Most methods for denoising scRNA-seq data have focused on using latent representations such as principal component analysis and deep learning to prioritise biological signals. By contrast, despite its influence on downstream analyses, feature selection has received relatively limited attention, leading to widespread reliance on the comparatively simplistic strategy of highly variable gene selection. Here we present Entropy Sorting Feature Selection (ESFS), a modular, user-friendly framework that substantially improves the interpretability of scRNA-seq data. Notably, ESFS reveals complex expression dynamics that are obscured in latent representations. We demonstrate the utility of ESFS in diverse data: identifying coherent developmental programs across eight independent human embryo datasets without batch integration; resolving spatial gene expression in mouse colon missed by conventional analyses; disambiguating shared and tumour-specific microenvironments in glioblastoma; and disentangling spatial, temporal, and neurogenic programs in the developing mouse neural tube. Beyond delivering a powerful and user-friendly software that deepens insight into complex biological systems, our work establishes Entropy Sorting as a novel information theoretic for advanced data analysis methods.