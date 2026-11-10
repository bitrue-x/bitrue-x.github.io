---
title: "Disaggregated RAID Storage in Modern Datacenters"
collection: talks
type: "组会分享"
permalink: /talks/2026-10-24-disaggregated-raid
venue: "28th ACM International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS), 2023"
date: 2026-10-24
location: "演讲人，沈文溪"
---


**简介：**
随着大语言模型在各类任务中的广泛应用，模型的预测过程往往难以理解，形成了所谓的"黑箱"问题。可解释性研究的主流做法是训练稀疏自编码器（SAE），把模型激活拆成"特征"再追踪计算电路，但这需要额外的训练成本，且重建误差可能丢失信息。本文另辟蹊径，提出不训练 SAE、直接以 MLP 神经元为最小单元的电路追踪方法：作者首次实证表明 MLP 神经元基与 SAE 特征基一样稀疏——同一行为在神经元基上的电路比常用的 MLP 输出基小了约一百倍；并提出替换归因方法 RelP，仅用一次反向传播便达到积分梯度（IG）十次反向传播的效果，节点与连边都能归因。该方法具有零额外训练成本、即插即用的特点，证明了模型的电路在神经元坐标系里稀疏到可以直接读懂、直接干预，为提高模型透明度与可信度，以及神经元级的归因与干预研究，提供了重要思路。
