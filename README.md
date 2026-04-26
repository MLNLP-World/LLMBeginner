<div align="center">

<img src="asset/image.png" alt="Slay the LLM Maze" width="320" />

# 零基础通关 LLM 的项目式学习路线
![GitHub stars](https://img.shields.io/github/stars/chenyuanTKCY/Slay-the-LLM-Maze?style=social)
![GitHub forks](https://img.shields.io/github/forks/chenyuanTKCY/Slay-the-LLM-Maze?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/chenyuanTKCY/Slay-the-LLM-Maze?style=social)
![License](https://img.shields.io/github/license/chenyuanTKCY/Slay-the-LLM-Maze)
![Last Commit](https://img.shields.io/github/last-commit/chenyuanTKCY/Slay-the-LLM-Maze)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![Awesome](https://awesome.re/badge.svg)
> 该项目旨在为初学者提供一条清晰的大模型学习路径，从零基础出发，循序渐进地理解 LLM 的核心原理、训练机制与应用范式，并逐步过渡到智能体（Agent）的构建与基础实践。我们希望在“会用”的基础上，进一步帮助学习者实现“看懂、做出、跑通”。整体内容采用分阶段设计，从 Big Picture 到底层机制，再到项目实践与系统搭建，力求路径清晰、节奏可控，帮助学习者逐步建立较为完整的认知与动手能力 🚀

由于我们能力与经验有限，内容难免存在不足或疏漏，敬请大家谅解，欢迎大家交流与指正。



</div>

---

## 📰 News

- **2026-04** - 项目启动，建立学习路线框架

---

## 📋 路线总览

本仓库采用阶段式学习路径（Staged Learning Path），旨在帮助你从零基础逐步成长为具备 LLM 研究能力的开发者。每个阶段都有明确的学习目标和可交付成果。

| 阶段 | 学习重点 | 核心目标 | 
|:---:|:---|:---|
| **Stage 0** | Big Picture | 理解整体路径与最终目标 |
| **Stage 1** | DL + RL | 建立深度学习与强化学习基础 |
| **Stage 2** | LLM | 构建大语言模型并掌握后训练方法 |
| **Stage 3** | Agent | 构建智能体框架与应用 |


---

## 🗺️ Stage 0: Big Picture

在开始学习任何技术细节之前，先建立对整个 LLM 领域的全局认知至关重要。很多初学者容易陷入"学了很多，但不知道自己在哪里"的困境——Stage 0 就是为了避免这种迷失。

**本阶段目标：** 理解 LLM 的来龙去脉、主流技术路线、以及你自己的学习路径，产出一份个人学习计划。

### 🧭 0.1 理解 LLM 的全貌

**① LLM 是什么？能做什么？**

在深入学习之前，先从宏观视角理解大语言模型：

- LLM 的核心能力来自海量数据上的预训练（Pre-training）
- 通过指令微调（Instruction Tuning）和人类反馈强化学习（RLHF）使模型变得"有用"
- 当前主流模型：GPT-4、Claude、Gemini、LLaMA、Qwen 等

**② LLM 的技术演进脉络**

理解历史脉络有助于理解为何现在的技术是这样的：

```
词向量时代（Word2Vec）
    → RNN / LSTM 序列模型
        → Transformer 架构（2017, Attention is All You Need）
            → BERT（理解型）/ GPT（生成型）
                → 大规模预训练（GPT-3, 175B 参数）
                    → 指令对齐（InstructGPT, RLHF）
                        → 当代 LLM（ChatGPT, Claude, Gemini...）
```

### 📖 0.2 推荐阅读

**① 李沐精读论文系列（必看）**

- 🔗 视频地址：https://space.bilibili.com/1567748478/lists?sid=32139
- 💡 推荐理由：逐行精读 Transformer、BERT、GPT 等奠基论文，帮助你建立"读论文"的能力，这是 LLM 研究者的核心技能

**② Andrej Karpathy：Neural Networks: Zero to Hero**

- 🔗 视频地址：https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ
- 💡 推荐理由：从最基础的神经网络一路讲到 GPT，是目前最好的 LLM 入门叙事线，强烈建议作为 Stage 0 的压轴内容

### 🎯 0.3 制定你的个人学习计划

在完成上述内容后，请根据自身情况回答以下问题，写出你的学习计划：

| 问题 | 思考方向 |
|:---|:---|
| 我的目标是什么？ | 做应用开发 / 研究模型 / 理解原理 |
| 我的时间预算？ | 每周可投入多少小时 |
| 我的已有基础？ | Python 熟练度 / 数学基础（线代、概率） |
| 我计划跳过哪些内容？ | 结合目标裁剪路径，避免无效学习 |


> 💬 建议：把你的学习计划写成一个 Markdown 文件放在本地仓库的专用文件夹，定期回顾和更新。


## 📚 Stage 1: DL + RL 基础

### 🟦 一、Deep Learning（深度学习）

深度学习是理解 LLM 的基石。本部分帮助你掌握神经网络、反向传播、优化算法等核心概念，为后续学习 Transformer 架构打下坚实基础。

#### 🎬 1.1 视频课程

**① 吴恩达：深度学习专项课程**

- 🔗 课程链接：https://www.bilibili.com/video/BV1FT4y1E74V/
- 📒 配套笔记：https://github.com/MLNLP-World/Deep_Learning_Notes
- 💡 推荐理由：系统性强，适合建立完整的深度学习知识体系

**② 李沐：动手学深度学习**

- 🔗 课程链接：https://space.bilibili.com/1567748478/lists?sid=358497
- 📒 配套笔记：https://github.com/MLNLP-World/Deep_Learning_Notes
- 💡 推荐理由：理论与代码结合紧密，注重动手实践

#### 💻 1.2 代码学习

**① 经典论文代码实现（强烈推荐）**

- 🔗 仓库地址：https://github.com/labmlai/annotated_deep_learning_paper_implementations
- ⭐ GitHub Stars: 66k+
- 💡 特点：论文逐行注释讲解，适合深入理解 Transformer、GPT 等模型实现细节

**② 可视化学习网站**

- 🔗 网站地址：https://nn.labml.ai/
- 💡 推荐理由：代码与解释同步展示，交互式体验，非常适合初学者直观理解模型结构

---

### 🟩 二、Reinforcement Learning（强化学习）

强化学习是 LLM 后训练（RLHF）的核心技术。掌握 RL 基础将帮助你理解如何通过人类反馈优化模型行为。

#### 🎬 2.1 视频课程

**① 动画中学强化学习（最容易理解）**

- 🔗 课程链接：https://space.bilibili.com/399855081/lists/4452634?type=series
- 📒 配套笔记：https://github.com/MLNLP-World/Reinforcement-Learning-Comic-Notes/
- 💡 推荐理由：以漫画形式讲解 RL 核心概念，零基础友好，大幅降低入门门槛

**② 李宏毅：强化学习课程**

- 🔗 课程链接：https://www.bilibili.com/video/BV1XP4y1d7Bk
- 💡 推荐理由：中文讲解清晰，善用直观类比，适合快速建立 RL 整体认知

**③ 王树森：深度强化学习（DRL）**

- 🔗 课程链接：https://www.bilibili.com/video/BV12o4y197US
- 💡 推荐理由：史蒂文斯理工学院王树森博士主讲，语言简洁有力，抛弃繁琐的数学推导，直接给出直观易懂的结论，初学者能在短时间内快速建立 DRL 整体体系认知

#### 💻 2.2 代码学习

**① Hands-on-RL（动手学强化学习）**

- 🔗 仓库地址：https://github.com/boyu-ai/Hands-on-RL
- 💡 推荐理由：配套教材《动手学强化学习》，从基础算法（Q-Learning）到 PPO 逐步实现，代码简洁，适合边学理论边写代码

**② easy-rl（强化学习中文教程）**

- 🔗 仓库地址：https://github.com/datawhalechina/easy-rl
- 💡 推荐理由：Datawhale 出品，中文注释详细，覆盖主流 RL 算法实现，社区活跃，适合中文学习者系统入门

---

## 🤖 Stage 2: LLM

完成 Stage 1 后，你已具备深度学习与强化学习的基础。Stage 2 的目标是真正理解 LLM 的内部机制，并亲手构建和训练一个语言模型。

**本阶段目标：** 掌握 Transformer 架构原理 → 理解预训练与后训练方法 → 掌握推理模型 → 从零实现小型 LLM → 在真实大模型上做微调实战 → 拓展到多模态。

---

### 🔩 一、机制理解：Attention & Transformer

在动手写代码之前，必须真正理解 Transformer 的每一个组件——注意力机制不是魔法，它是有数学直觉的。

#### 📖 1.1 核心论文精读

**① Attention is All You Need（2017，必读）**

- 🔗 论文地址：https://arxiv.org/abs/1706.03762
- 🔗 李沐精读视频：https://www.bilibili.com/video/BV1pu411o7BE
- 💡 重点理解：Multi-Head Self-Attention、位置编码（Positional Encoding）、Encoder-Decoder 结构

**② The Illustrated Transformer（最直观的图解）**

- 🔗 文章地址：https://jalammar.github.io/illustrated-transformer/
- 💡 推荐理由：全程配图讲解 Attention 的计算过程，是理解 Transformer 最友好的入门材料，建议与论文配合阅读

#### 🎬 1.2 视频讲解

**Andrej Karpathy：Let's build GPT from scratch**

- 🔗 视频地址：https://www.youtube.com/watch?v=kCc8FmEb1nY
- 🔗 配套代码：https://github.com/karpathy/nanoGPT
- 💡 推荐理由：2 小时内从零手写一个 GPT，边写边讲原理，是目前最好的 Transformer 实践教程

---

### 🏋️ 二、预训练（Pre-training）

预训练是 LLM 能力的来源。理解预训练的目标函数、数据处理和训练技巧，是研究 LLM 的必要基础。

**核心概念：**

- **Next Token Prediction**：自回归语言模型的训练目标，模型通过预测下一个词来学习语言规律
- **Scaling Law**：模型参数量、数据量、计算量三者的幂律关系，指导如何高效扩大模型规模
- **训练技巧**：混合精度训练（FP16/BF16）、梯度累积、学习率调度（Warmup + Cosine Decay）

**① Scaling Laws for Neural Language Models（必读论文）**

- 🔗 论文地址：https://arxiv.org/abs/2001.08361
- 💡 重点理解：为什么更大的模型 + 更多数据 = 更好的效果，以及如何用有限算力做出最优决策

**② LLaMA 技术报告（工程实践参考）**

- 🔗 论文地址：https://arxiv.org/abs/2302.13971
- 💡 推荐理由：Meta 开源模型的技术细节，展示了完整的预训练工程实践，包括数据配比、训练稳定性等问题的解决方案

---

### 🎯 三、后训练（Post-training）

预训练后的模型只会"续写文本"，后训练让模型变得"听话"且"有用"。这是当前 LLM 研究最活跃的方向之一。

**后训练技术路线：**

```
预训练模型（Base Model）
    → SFT 监督微调：用高质量对话数据教模型"怎么回答"
        → RM 奖励模型训练：学习人类对回答质量的偏好
            → RLHF / PPO：用 RL 让模型最大化奖励，对齐人类期望
                → DPO：更简洁的对齐方案，无需显式 RM
```

**① InstructGPT 论文（RLHF 的奠基之作）**

- 🔗 论文地址：https://arxiv.org/abs/2203.02155
- 🔗 李沐精读视频：https://www.bilibili.com/video/BV1hd4y187CR
- 💡 重点理解：三阶段训练流程（SFT → RM → PPO），以及为什么 RLHF 能显著提升模型有用性

**② DPO 论文（更简洁的对齐方法）**

- 🔗 论文地址：https://arxiv.org/abs/2305.18290
- 💡 推荐理由：绕过奖励模型，直接从偏好数据优化策略，是目前工业界最常用的对齐方案之一



---

### 🧠 四、推理（Reasoning）

传统 LLM 是"快思考"模型，直接输出答案。推理模型引入"慢思考"机制，通过显式的推理过程（如思维链、自我反思）来提升复杂问题的求解能力。

#### 4.1 System 2 Thinking（慢思考 / 推理模型）

**核心思想：** 让模型在回答前先"思考"——生成中间推理步骤，而不是直接给出答案。这类似人类的 System 2 思维（深思熟虑），而非 System 1（直觉反应）。

**代表模型：**

- **OpenAI o1 系列**：通过强化学习训练模型生成长推理链，在数学、编程等任务上显著超越 GPT-4
- **DeepSeek-R1**：开源的推理模型，公开了训练方法和推理过程，是目前最具影响力的开源推理模型

**① DeepSeek-R1 技术报告（必读）**

- 🔗 论文地址：https://arxiv.org/abs/2501.12948
- 💡 重点理解：如何用 RL 训练模型生成高质量推理链，以及推理模型与传统 LLM 的训练差异

**② Chain-of-Thought Prompting（思维链提示）**

- 🔗 论文地址：https://arxiv.org/abs/2201.11903
- 💡 推荐理由：推理模型的理论基础，展示了"让模型一步步思考"如何显著提升复杂推理任务的表现

**③ 代码实践：OpenR（开源推理模型训练框架）**

- 🔗 仓库地址：https://github.com/openreasoner/openr
- ⭐ GitHub Stars: 3k+
- 💡 推荐理由：提供完整的推理模型训练 pipeline，包括推理数据生成、RL 训练等，是动手实践推理模型的最佳起点

---

### 🛠️ 五、轻量小项目：从零实现一个 LLM

理论学完，动手是关键。这一部分帮助你把前面所学串联起来，亲手训练一个完整的小型语言模型。

**① nanoGPT（最推荐的起点）**

- 🔗 仓库地址：https://github.com/karpathy/nanoGPT
- ⭐ GitHub Stars: 40k+
- 💡 推荐理由：Karpathy 出品，约 300 行核心代码实现完整 GPT 训练，可在单张 GPU 上跑通，是从零实现 LLM 的最佳模板

**② minimind（中文小模型全流程实现）**

- 🔗 仓库地址：https://github.com/jingyaogong/minimind 
https://github.com/jingyaogong/minimind-v (多模态版本)
- ⭐ GitHub Stars: 20k+
- 💡 推荐理由：完整实现了预训练 → SFT → RLHF 全流程，代码注释详细，中文社区友好，适合跟着走完整个训练 pipeline

**③ LLM-from-scratch （从零实现大模型功能拆解讲述）**

- 🔗 中文翻译版本仓库地址：https://github.com/MLNLP-World/LLMs-from-scratch-CN
- ⭐ GitHub Stars: 2k+
- 🔗 原仓库地址：https://github.com/rasbt/LLMs-from-scratch
- ⭐ GitHub Stars: 91k+
- 💡 推荐理由：不仅关注 LLMs 的基础构建，如 Transformer 架构、序列建模 等，还深入探索了 GPT、BERT 等深度学习模型 的底层实现。项目中的每一部分均配备详细的代码实现和学习资源，帮助学习者从零开始构建 LLMs，全面掌握其核心技术。

**推荐学习顺序：**

1. 跑通 nanoGPT，理解训练循环的每一行代码
2. 在 minimind 上走完 预训练 → SFT → DPO 全流程
3. 尝试修改超参数（层数、头数、学习率），观察训练曲线变化

---

### 🚀 六、大模型实战：微调与部署

在真实大模型上做实验，是从"理解原理"到"工程落地"的关键一步。

#### 5.1 高效微调（PEFT）

全量微调大模型成本极高，PEFT 方法只训练少量参数，即可达到接近全量微调的效果。

**① LoRA（最主流的高效微调方法）**

- 🔗 论文地址：https://arxiv.org/abs/2106.09685
- 💡 核心思想：将权重更新分解为两个低秩矩阵的乘积，只训练约 0.1% 的参数量即可达到不错效果

**② LLaMA-Factory（一站式微调框架）**

- 🔗 仓库地址：https://github.com/hiyouga/LLaMA-Factory
- ⭐ GitHub Stars: 40k+
- 💡 推荐理由：支持主流开源模型（LLaMA、Qwen、Mistral 等）的 SFT / DPO / LoRA 微调，提供 WebUI，降低工程门槛


**③ veRL（大规模 RLHF 训练框架）**

- 🔗 仓库地址：https://github.com/volcengine/verl
- ⭐ GitHub Stars: 8k+
- 💡 推荐理由：字节跳动开源的分布式 RLHF 训练框架，支持 PPO / GRPO 等算法，与 HuggingFace 生态无缝集成，是目前在真实大模型上做 RLHF 实验的最佳选择之一

#### 5.2 推理与部署

**① Ollama（本地运行大模型最简单的方式）**

- 🔗 官网地址：https://ollama.com/
- 💡 推荐理由：一行命令在本地运行 LLaMA、Qwen 等模型，适合快速体验和调试

**② vLLM（高性能推理框架）**

- 🔗 仓库地址：https://github.com/vllm-project/vllm
- ⭐ GitHub Stars: 45k+
- 💡 推荐理由：基于 PagedAttention 技术，大幅提升推理吞吐量，是目前生产环境部署 LLM 的主流选择

---

### 🖼️ 七、多模态 LLM（Multimodal LLM）

纯文本 LLM 之外，多模态模型能够同时理解图像、视频、音频等信息。这是当前前沿研究和产品落地最活跃的方向之一。

**多模态的核心问题：** 如何把不同模态的信息"对齐"到同一个语义空间，让语言模型能够理解图像？

**模态融合的主流架构：**

```
图像编码器（Vision Encoder，如 ViT / CLIP）
    → 将图像切成 Patch，编码为向量序列
        → 投影层（Projector）：把视觉 token 映射到语言模型的词向量空间
            → 语言模型（LLM）：统一处理文字 + 图像 token，生成回答
```

#### 📖 6.1 核心论文

**① CLIP（视觉-语言对齐的奠基之作）**

- 🔗 论文地址：https://arxiv.org/abs/2103.00020
- 💡 重点理解：对比学习如何让图像和文本在同一空间对齐，这是多模态模型的底层基础

**② LLaVA（最具影响力的开源多模态模型）**

- 🔗 论文地址：https://arxiv.org/abs/2304.08485
- 🔗 李沐精读视频：https://www.bilibili.com/video/BV1iN411r7ma
- 💡 推荐理由：结构简洁（CLIP + Projector + LLaMA），用指令微调实现视觉问答，是理解多模态 LLM 架构的最佳入门论文

**③ Qwen-VL 技术报告（工程实践参考）**

- 🔗 论文地址：https://arxiv.org/abs/2308.12966
- 💡 推荐理由：详细描述了一个完整的多模态模型训练流程，包括多阶段训练策略和数据配比，适合工程落地参考

#### 💻 6.2 代码实践

**LLaVA 官方仓库**

- 🔗 仓库地址：https://github.com/haotian-liu/LLaVA
- ⭐ GitHub Stars: 22k+
- 💡 推荐理由：代码结构清晰，支持自定义数据集微调，是动手实践多模态模型的最佳起点

---

## 🤖 Stage 3: Agent

完成 Stage 2 后，你已掌握 LLM 的训练、推理与部署。Stage 3 关注如何把模型放进**闭环**：感知 → 决策 → 行动 → 观察 → 更新状态，直至任务完成。

**本阶段目标：** 从范式上区分「聊天模型」与「行动者」→ 掌握工具调用与记忆/RAG 的工程化组合 → 理解多智能体的协议、组织与环境 → 跟跑至少一个开源项目，并自选垂直场景深入。

---

### 一、理解 Agent：从 LLM 到行动者

#### 1.1 Agent 的核心定义与能力边界

**定义：**

Agent = LLM（大脑） + 记忆 + 规划 + 工具使用。它能自主感知环境、做出决策并执行动作。

**能力边界：**

✅ 能：多步推理、调用外部工具、与用户/环境交互、利用长期记忆

❌ 不能：完全自主的目标设定（仍需人类引导）、真正的理解与意识

与普通 Chatbot 的区别：Chatbot 是被动响应，Agent 是主动规划与行动。

**① 李宏毅：一堂课搞懂 AI Agent 的原理**

- 🔗 视频地址：https://www.youtube.com/watch?v=M2Yg1kwPpts
- 💡 推荐理由：建立 Agent 概念与问题设定，适合作为 agent 入门课程。

**② Lilian Weng：LLM Powered Autonomous Agents（博文）**

- 🔗 文章地址：https://lilianweng.github.io/posts/2023-06-23-agent/
- 💡 推荐理由：从自主智能体、规划与工具等角度做系统梳理。

**③ Agent 领域综述**

- 🔗 论文地址：https://arxiv.org/pdf/2601.14192
- 💡 推荐理由：长文综述类材料，可按目录选读，用于扩展视野。

#### 1.2 Agent 的经典架构模式

**① ReAct**

- 🔗 论文地址：https://arxiv.org/abs/2210.03629  
- 💡 重点理解：核心在于将**思维链（CoT）与动作（Action）**交替结合，形成“思考-行动-观察”的闭环。模型在每一步行动前先写出推理过程，这不仅提高了决策的透明度，还允许模型根据环境的实时观察动态修正后续的推理。

**② Plan-and-Solve Prompting**

- 🔗 论文地址：https://arxiv.org/abs/2305.04091  
- 💡 重点理解：提出了“先全局规划，后分步执行”的策略。模型首先将复杂任务拆解为子任务列表，然后再逐一解决，显著提升了处理多步骤逻辑问题的稳定性与准确率。

**③ Reflexion**

- 🔗 论文地址：https://arxiv.org/abs/2303.11366  
- 💡 重点理解：引入了自我反思机制，通过在外部环境中试错来获取语言反馈。模型将失败的尝试存储在短期记忆中，并在下一次迭代时根据这些“教训”修正策略，这种“自省”能力让 Agent 具备了在不更新参数的情况下进行自我优化的能力。
---

### 二、Agent 核心能力

Agent 的本质是“系统”而非单一“模型”。 除了模型本身的推理能力外，系统侧的架构设计决定了 Agent 能否从“对话框”走向“生产力工具”。这主要涉及两个核心维度的工程闭环：一是工具调用，解决 Agent 权限受控、安全、稳态地操作外部环境的问题；二是记忆与上下文管理，解决信息在有限窗口内的流动策略，以及长短期知识的存储与检索。

#### 2.1 工具调用

**工具是什么：把外部能力封装成可调用的函数 / API**

工具是 Agent 的“手脚”：搜索、计算器、访问数据库、发消息等。除了名字和说明要清楚，还要约定入参/出参、超时、重试、是否改数据、给多大权限。

**① Anthropic：Writing Effective Tools for Agents**

- 🔗 文档地址：https://www.anthropic.com/engineering/writing-effective-tools-for-agents
- 💡 推荐理由：讲清工具名、说明与错误回传怎么写，模型才容易稳定、可恢复地调用。

**② OpenAI：Function Calling 指南**

- 🔗 文档地址：https://platform.openai.com/docs/guides/function-calling
- 💡 推荐理由：结构化调用的行业常用约定，对应「自然语言如何变成 JSON 参数、运行时如何执行与回写」的闭环。

**③ Model Context Protocol（MCP）**

- 🔗 文档地址：https://modelcontextprotocol.io/introduction
- 🔗 参考实现（官方 servers 仓库）：https://github.com/modelcontextprotocol/servers
- 💡 推荐理由：用统一方式暴露工具与数据，多客户端可复用同一套 MCP 服务；协议与参考实现可对照阅读。


**代码示例（LangChain `tool`）**

```python
from langchain.tools import tool

@tool
def search(query: str) -> str:
    """搜索实时信息"""
    return f"搜索结果: {query}"
```

#### 2.2 记忆与上下文管理

本节说明对话与外部知识如何进入模型、如何驻留：在系统提示、历史、工具返回与检索片段共同占用 token 的前提下，如何配置与裁剪上下文。随后讨论短期（工作）记忆、长期记忆与RAG技术。

**短期（工作）记忆：**

- 对话缓冲 / 滑动窗口：仅保留最近 k 轮对话或固定长度的 Token。实现最简单、延迟最低，但存在断层式遗忘，一旦信息超出窗口，Agent 将彻底丧失对早期指令的感知。
- 摘要压缩：周期性把历史压成摘要再续聊，需注意摘要漂移与事实丢失，需警惕“摘要漂移”（多次摘要后细节走样）与核心事实丢失；通常建议采用“摘要 + 最近 n 轮原话”的混合方案。

**长期记忆：**

- 向量数据库 + 混合检索： 结合语义检索理解意图与关键词检索锁定专有名词。必须引入重排序步骤。初次检索保证“召回率”，重排序保证“准确率”，防止 Agent 被海量但不相关的知识片段干扰。
- 结构化记忆： 用户偏好、任务状态机、会话级元数据存放在 DB / KV，而非全部塞进 prompt。 

**RAG 技术（把外部知识“接进”推理）**

**RAG**（Retrieval-Augmented Generation，检索增强生成）指：在回答前，先从文档、知识库、网页等语料里检索出与问题相关的若干片段，再与当前对话一起拼进提示，让模型在“有据可依”的上下文中生成。

**推荐阅读：**

**① Anthropic：Effective Context Engineering for AI Agents**

- 🔗 文档地址：https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- 💡 推荐理由：介绍系统提示、工具、历史、MCP 等如何共同占满窗口，将「上下文」视为可组合、可取舍的配置。

**② Claude-Mem**

- 🔗 文档地址：https://docs.claude-mem.ai/introduction
- 🔗 仓库地址：https://github.com/thedotmack/claude-mem
- 💡 推荐理由：工程向的长期记忆/持久化参考，适合本地或自建部署时阅读。

**③ Mem0（The Memory Layer for AI Agents）**

- 🔗 仓库地址：https://github.com/mem0ai/mem0
- ⭐ GitHub Stars: 以仓库页为准
- 🔗 论文地址：https://arxiv.org/abs/2504.19413
- 🔗 博客地址：https://get.mem.ai/blog
- 💡 推荐理由：较常用的记忆层实现参考之一；可先读论文与博客了解动机与能力边界，再决定是否接入。


**④ Agent Memory 综述（长文 PDF，选读）**

- 🔗 论文地址：https://arxiv.org/pdf/2512.13564
- 💡 推荐理由：可作为 agent memory 研究进展的补充阅读；具体以 arXiv 页面信息为准。


**⑤ LangChain 文档：RAG**

- 🔗 文档地址：https://docs.langchain.com/oss/python/langchain/rag
- 💡 推荐理由：官方文档里从加载、切分、向量库到检索接模型的主线，适合动手搭第一条 RAG 链路。

**⑥ LlamaIndex：生产环境 RAG 与优化**

- 🔗 文档地址：https://developers.llamaindex.ai/python/framework/optimizing/production_rag/
- 💡 推荐理由：索引、多路召回、重排等工程侧优化，适合在 baseline RAG 效果不足时对照排查。

---

### 三、多智能体系统原理

#### 3.1 什么是多智能体系统：任务驱动协作、自治群体交互

#### 3.2 智能体之间如何「说话」？——交互协议

#### 3.3 智能体团队如何「组织」？——组织结构

#### 3.4 智能体在什么「世界」里活动？——协作环境

### 四、实战项目

#### GUI Agent

**Awesome-GUI-Agent**

- 🔗 仓库地址：https://github.com/showlab/Awesome-GUI-Agent  
- 🔗 论文地址：无单一项目论文；列表内按主题链接 GUI Agent 相关论文、数据集、基准与开源实现，可按图索骥阅读。  
- ⭐ GitHub Stars: 1.2k+  
- 💡 推荐理由：桌面/移动端多模态 GUI 导航、屏幕理解与操作类资源的**总索引**，适合建立领域地图、对比感知方案（纯视觉、DOM/可访问性树、混合）与典型评测；学习路径上建议作为「选方向 + 找论文/代码」的入口，而非单一代码库。  

**MobileRun**

- 🔗 仓库地址：https://github.com/droidrun/mobilerun  
- ⭐ GitHub Stars: 8k+ 
- 💡 推荐理由：面向 **Android 等真机/模拟器** 的自然语言操作框架，多模型后端、多步规划与截屏/可访问性等感知组合较完整，适合和 Awesome 里「手机 GUI」类线索对照，从**一条可复现的移动端指令**跑通到自定义流程。  

**UI-TARS**

- 🔗 仓库地址：https://github.com/bytedance/UI-TARS  
- ⭐ GitHub Stars: 10k+ 
- 💡 推荐理由：字节开源的**原生 GUI 交互 / 多模态智能体**主线仓库（含或指向 UI-TARS 系列模型与推理、强化学习后训练等说明），和「纯脚本点击」对读能看清 **VLM + 坐标签图 + 多环境任务** 的建模范式。若要做桌面/浏览器，可再关注同组织下的 *UI-TARS-desktop* 等派生项目。  

**AgentCPM-GUI（OpenBMB，端侧 Android GUI Agent）**

- 🔗 仓库地址：https://github.com/OpenBMB/AgentCPM-GUI  
- ⭐ GitHub Stars: 1.3k+（以仓库页为准）  
- 💡 推荐理由：**端上**操作 Android 应用的 GUI 智能体路线，强调用**强化学习微调**等后训练提升推理与执行效率，与 OpenBMB 生态（如已有接触 ToolBench/ChatDev）衔接自然；适合和 MobileRun 对读「同一 Android 场景下不同训练与部署取舍」。  
- 🎯 实战建议：先按 README 跑通官方任务或最小 demo，记录设备分辨率、无障碍与动作空间配置；再对照论文/技术报告中的**奖励设计与轨迹数据**是否可迁移到你自己的评测集。  

#### Computer Use Agent

**Browser Use**

- 🔗 仓库地址：https://github.com/browser-use/browser-use   
- ⭐ GitHub Stars: 90k+  
- 💡 推荐理由：社区热度高、迭代快的**浏览器侧**自动化 Agent 框架，强调让模型在真实网页上规划与执行；适合与 Playwright/浏览器能力结合，做「多步打开网页、填表、采数」等落地形态。  

**Anthropic Computer Use**

- 🔗 仓库地址：https://github.com/anthropics/anthropic-quickstarts    
- ⭐ GitHub Stars: 16k+  
- 💡 推荐理由：Anthropic 附带的**快速示例与脚手架**，便于在官方 Computer Use/视觉+键鼠范式下做最小可运行 demo；和「自己做浏览器环境」对读，能分清模型能力与客户端截图/控制协议分工。    

#### DeepResearch Agent（多轮搜索 + 交叉验证 + 报告）

**langchain-ai/open_deep_research**

- 🔗 仓库地址：https://github.com/langchain-ai/open_deep_research   
- ⭐ GitHub Stars: 11k+  
- 💡 推荐理由：适合作为**全流程主线**的多轮检索、压缩与成稿 pipeline，和 LangChain 生态、Provider/MCP 组合较好接；想一次性看清「子研究 → 综合 → 报告」的模块切分时优先选它。  

**dzhng/deep-research**

- 🔗 仓库地址：https://github.com/dzhng/deep-research   
- ⭐ GitHub Stars: 18k+  
- 💡 推荐理由：单仓库体量相对克制，**代码路径短**，适合读清「多轮 query 生成、并发抓取、再汇总成 Markdown 报告」的主干逻辑，再迁移到自己的栈或做教学拆解。  


#### 基于 OpenClaw 部署小红书自动运营

#### 法律智能体

#### 金融智能体

#### 医疗健康助手


