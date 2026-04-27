# Stage 2 Supply

## 一、机制理解：Attention & Transformer

### 1.1 核心论文精读补充

**The Illustrated Transformer（最直观的图解）**

- 🔗 文章地址：https://jalammar.github.io/illustrated-transformer/
- 💡 推荐理由：全程配图讲解 Attention 的计算过程，是理解 Transformer 最友好的入门材料，建议与论文配合阅读

## 二、预训练（Pre-training）

**LLaMA 技术报告（工程实践参考）**

- 🔗 论文地址：https://arxiv.org/abs/2302.13971
- 💡 推荐理由：Meta 开源模型的技术细节，展示了完整的预训练工程实践，包括数据配比、训练稳定性等问题的解决方案

## 三、后训练（Post-training）

**DPO 论文（更简洁的对齐方法）**

- 🔗 论文地址：https://arxiv.org/abs/2305.18290
- 💡 推荐理由：绕过奖励模型，直接从偏好数据优化策略，是目前工业界最常用的对齐方案之一

## 四、推理（Reasoning）

**Chain-of-Thought Prompting（思维链提示）**

- 🔗 论文地址：https://arxiv.org/abs/2201.11903
- 💡 推荐理由：推理模型的理论基础，展示了“让模型一步步思考”如何显著提升复杂推理任务的表现

**OpenR（开源推理模型训练框架）**

- 🔗 仓库地址：https://github.com/openreasoner/openr
- ⭐ GitHub Stars: 3k+
- 💡 推荐理由：提供完整的推理模型训练 pipeline，包括推理数据生成、RL 训练等，是动手实践推理模型的最佳起点

## 五、轻量小项目：从零实现一个 LLM

**minimind（中文小模型全流程实现）**

- 🔗 仓库地址：https://github.com/jingyaogong/minimind
- 🔗 多模态版本：https://github.com/jingyaogong/minimind-v
- ⭐ GitHub Stars: 20k+
- 💡 推荐理由：完整实现了预训练 → SFT → RLHF 全流程，代码注释详细，中文社区友好，适合跟着走完整个训练 pipeline

**LLM-from-scratch（从零实现大模型功能拆解讲述）**

- 🔗 中文翻译版本仓库地址：https://github.com/MLNLP-World/LLMs-from-scratch-CN
- ⭐ GitHub Stars: 2k+
- 🔗 原仓库地址：https://github.com/rasbt/LLMs-from-scratch
- ⭐ GitHub Stars: 91k+
- 💡 推荐理由：不仅关注 LLM 的基础构建，如 Transformer 架构、序列建模，还深入探索了 GPT、BERT 等模型的底层实现，适合系统拆解学习

## 六、大模型实战：微调与部署

### 5.1 高效微调（PEFT）补充

**LLaMA-Factory（一站式微调框架）**

- 🔗 仓库地址：https://github.com/hiyouga/LLaMA-Factory
- ⭐ GitHub Stars: 40k+
- 💡 推荐理由：支持主流开源模型（LLaMA、Qwen、Mistral 等）的 SFT / DPO / LoRA 微调，提供 WebUI，降低工程门槛

**veRL（大规模 RLHF 训练框架）**

- 🔗 仓库地址：https://github.com/volcengine/verl
- ⭐ GitHub Stars: 8k+
- 💡 推荐理由：字节跳动开源的分布式 RLHF 训练框架，支持 PPO / GRPO 等算法，与 HuggingFace 生态无缝集成，是目前在真实大模型上做 RLHF 实验的最佳选择之一

### 5.2 推理与部署补充

**vLLM（高性能推理框架）**

- 🔗 仓库地址：https://github.com/vllm-project/vllm
- ⭐ GitHub Stars: 45k+
- 💡 推荐理由：基于 PagedAttention 技术，大幅提升推理吞吐量，是目前生产环境部署 LLM 的主流选择

## 七、多模态 LLM（Multimodal LLM）

### 6.1 核心论文补充

**LLaVA（最具影响力的开源多模态模型）**

- 🔗 论文地址：https://arxiv.org/abs/2304.08485
- 🔗 李沐精读视频：https://www.bilibili.com/video/BV1iN411r7ma
- 💡 推荐理由：结构简洁（CLIP + Projector + LLaMA），用指令微调实现视觉问答，是理解多模态 LLM 架构的最佳入门论文

**Qwen-VL 技术报告（工程实践参考）**

- 🔗 论文地址：https://arxiv.org/abs/2308.12966
- 💡 推荐理由：详细描述了一个完整的多模态模型训练流程，包括多阶段训练策略和数据配比，适合工程落地参考
