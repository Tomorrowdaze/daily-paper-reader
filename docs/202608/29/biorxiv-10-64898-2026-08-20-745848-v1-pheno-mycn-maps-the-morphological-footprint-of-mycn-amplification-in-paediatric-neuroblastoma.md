---
title: Pheno-MYCN maps the morphological footprint of MYCN amplification in paediatric neuroblastoma
title_zh: Pheno-MYCN映射儿童神经母细胞瘤中MYCN扩增的形态学足迹
authors: "Chai, B., Fourkioti, O., Naidoo, R., De Vries, M., George, S., Chesler, L., Hutchinson, J. C., Bakal, C."
date: 2026-08-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.20.745848v1.full.pdf"
tags: ["query:q5"]
score: 6.5
evidence: 将预测与可解释的形态学子群体联系起来的弱监督框架
tldr: "本研究针对神经母细胞瘤MYCN扩增难以与形态定位结合的问题，提出弱监督框架Pheno-MYCN，将切片级MYCN预测与H&E形态子群关联；在189张切片中解析表型簇并揭示可解释的扩增足迹，凭形态即可高精度定位（AUC0.93–1.00），为低成本标记与映射提供可能。"
source: biorxiv
selection_source: fresh_fetch
motivation: MYCN扩增常以整体检测进行且难与组织形态异质性对应，单独的分子或形态信息均难以定位风险与相关生物学。
method: "提出弱监督框架Pheno-MYCN，将切片级MYCN预测与H&E上的可解释形态子群关联，并结合专家审阅与细胞级特征分析进行验证。"
result: 在189张切片上解析出与神经母细胞瘤形态相符的表型簇，发现MYCN扩增为各子群留下不同形态标记（如致密而紊乱的肿瘤、稀疏低多样网络、坏死/出血富集），可仅凭形态高精度识别（AUC0.93–1.00），并呈肿瘤内连续梯度。
conclusion: "MYCN扩增在常规H&E上具备具体且可解释的形态足迹，可被读取与定位，为分子检测受限环境提供低成本的标记与映射途径。"
---

## 摘要
MYCN扩增长期以来一直是儿童神经母细胞瘤的预后标志，但其检测通常以整体方式进行，与病理学家所评估的异质性组织结构并置，而非在其内部定位。这造成了空白：仅凭MYCN状态无法定位其相关生物学，单凭形态学也无法判定分子风险。基于我们发现二者结合可识别各自单独方法漏判的高风险病例，我们开发了Pheno-MYCN，这是一种弱监督框架，将切片级MYCN预测与常规H&E全切片图像上的可解释形态学亚群相连。我们的目标并非更强的分类器；该预测旨在探查MYCN扩增对组织的影响，其证据可供病理学审视。在189张切片中，Pheno-MYCN将每张切片划分为表型簇，经专家评审映射到神经母细胞瘤的形态学类型。细胞层面的分析显示，MYCN扩增通过不同特征“标记”每个亚群：例如，肿瘤区域呈细胞致密却结构紊乱、网络更稀疏且多样性较低；并且在坏死与出血区域主要表现为更高的丰度。仅凭这些特征即可在每张切片上识别出呈MYCN扩增样的组织（AUC 0.93–1.00，逐切片留一法），并可在肿瘤内部追踪其为一个连续梯度。因此，MYCN扩增在组织上留下了具体且可解释的足迹，可在常规H&E下读取并定位，在分子检测受限的环境中提供一种低成本的提示与空间映射手段。

## Abstract
MYCN amplification has long been a prognostic marker in paediatric neuroblastoma, yet is typically assayed in bulk, alongside rather than within the heterogeneous tissue architecture pathologists assess. This leaves a gap: MYCN status alone cannot localise MYCN-associated biology, while morphology alone cannot assign molecular risk. Motivated by our finding that the two together identify high-risk cases missed by either, we developed Pheno-MYCN, a weakly supervised framework linking slide-level MYCN prediction to interpretable morphological sub-populations on routine H&E whole-slide images. The aim is not a stronger classifier: prediction probes what MYCN amplification does to the tissue, its evidence open to pathological scrutiny. Across 189 slides, Pheno-MYCN resolved each into phenotypic clusters that expert review mapped to neuroblastoma morphologies. Cell-level profiling revealed MYCN amplification "marked" every sub-population, through a different feature in each: densely cellular yet disorganised tumour with sparser, less diverse networks; chiefly abundance in necrotic and haemorrhagic regions. MYCN-amplified-like tissue was identifiable per slide from these features alone (AUC 0.93-1.00, leave-one-slide-out) and traced as a continuous gradient within tumours. Thus MYCN amplification leaves a concrete, interpretable footprint that can be read and localised on routine H&E, offering a low-cost means to flag and map it where molecular testing is limited.