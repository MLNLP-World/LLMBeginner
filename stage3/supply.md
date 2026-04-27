# Stage 3 Supply

## 一、理解 Agent：从 LLM 到行动者

### 1.1 Agent 的核心定义与能力边界补充

**Lilian Weng：LLM Powered Autonomous Agents（博文）**

- 🔗 文章地址：https://lilianweng.github.io/posts/2023-06-23-agent/
- 💡 推荐理由：全面解析 LLM Agent 的设计范式与关键技术，配有丰富的案例分析，是理解 LLM Agent 架构设计的优质参考。

**Agent 领域综述**

- 🔗 论文地址：https://arxiv.org/pdf/2309.07864
- 💡 推荐理由：长文综述类材料，可按目录选读，用于扩展视野。

### 1.2 Agent 的经典架构模式补充

**Plan-and-Solve Prompting**

- 🔗 论文地址：https://arxiv.org/pdf/2305.04091
- 💡 重点理解：提出了“先全局规划，后分步执行”的策略。模型首先将复杂任务拆解为子任务列表，然后再逐一解决，显著提升了处理多步骤逻辑问题的稳定性与准确率。

**Reflexion**

- 🔗 论文地址：https://arxiv.org/pdf/2303.11366
- 💡 重点理解：引入了自我反思机制，通过在外部环境中试错来获取语言反馈。模型将失败的尝试存储在短期记忆中，并在下一次迭代时根据这些“教训”修正策略，这种“自省”能力让 Agent 具备了在不更新参数的情况下进行自我优化的能力。

## 二、Agent 核心能力

### 2.1 工具调用补充

**Anthropic：Tool Use 概览**

- 🔗 文档地址：https://docs.anthropic.com/claude/docs/tool-use
- 💡 推荐理由：介绍 Client/Server 工具的执行模式、Agent 循环的工作机制，以及工具调用的流程，适合理解工具集成的核心概念与实现路径。

**Model Context Protocol（MCP）**

- 🔗 文档地址：https://modelcontextprotocol.io/introduction
- 🔗 参考实现：https://github.com/modelcontextprotocol/servers
- 💡 推荐理由：用统一方式暴露工具与数据，多客户端可复用同一套 MCP 服务；协议与参考实现可对照阅读。

**Agent Skills with Anthropic**

- 🔗 课程地址：https://learn.deeplearning.ai/courses/agent-skills-with-anthropic/information
- 💡 推荐理由：学习用开放标准构建可复用的智能体技能，掌握将技能、MCP 与子智能体组合的方法，搭建能访问外部数据、具备专业知识的强大的智能体系统。

### 2.2 记忆与上下文管理补充

**Claude-Mem**

- 🔗 文档地址：https://docs.claude-mem.ai/introduction
- 🔗 仓库地址：https://github.com/thedotmack/claude-mem
- 💡 推荐理由：工程向的长期记忆/持久化参考，适合自建部署时阅读。

**Mem0（The Memory Layer for AI Agents）**

- 🔗 仓库地址：https://github.com/mem0ai/mem0
- ⭐ GitHub Stars: 54k+
- 🔗 论文地址：https://arxiv.org/pdf/2504.19413
- 🔗 博客地址：https://get.mem.ai/blog
- 💡 推荐理由：较常用的记忆层实现参考之一；可先读论文与博客了解动机与能力边界，再决定是否接入。

**Agent Memory 综述（长文 PDF，选读）**

- 🔗 论文地址：https://arxiv.org/pdf/2512.13564
- 💡 推荐理由：可作为 agent memory 研究进展的补充阅读。

**LangChain 文档：RAG**

- 🔗 文档地址：https://docs.langchain.com/oss/python/langchain/rag
- 💡 推荐理由：官方文档里从加载、切分、向量库到检索接模型的主线，适合动手搭第一条 RAG 链路。

## 三、多智能体系统

### 3.1 什么是多智能体系统：任务驱动协作、自治群体交互补充

**HuggingFace Agents Course（系统入门首选）**

- 🔗 课程地址：https://huggingface.co/learn/agents-course/
- 💡 推荐理由：HuggingFace 官方出品，从单 Agent 基础到多 Agent 协作循序渐进，配有可直接运行的代码实践，是目前最完整的开源 Agent 入门课程

**Generative Agents：斯坦福小镇（自治群体交互）**

- 🔗 论文地址：https://arxiv.org/abs/2304.03442
- 💡 重点理解：25 个 Agent 在模拟小镇中自主生活、社交、形成记忆，展示了 LLM 驱动的群体涌现行为。核心机制：记忆流（Memory Stream）+ 反思（Reflection）+ 行动规划（Planning）

**A Survey on LLM-based Autonomous Agents（全景综述）**

- 🔗 论文地址：https://arxiv.org/abs/2308.11432
- 💡 推荐理由：全面梳理 LLM Agent 的记忆、规划、工具使用与多 Agent 协作四大模块，适合在深入某个方向前建立完整的认知框架

**Large Language Model based Multi-Agents: A Survey of Progress and Challenges（多智能体专项综述）**

- 🔗 论文地址：https://arxiv.org/abs/2402.01680
- 💡 推荐理由：专注于多 Agent 系统本身，系统梳理 LLM 驱动的多 Agent 在通信、组织、环境与应用上的最新进展与挑战

### 3.2 智能体之间如何「说话」？——交互协议补充

**CAMEL（角色扮演的多 Agent 通信范式）**

- 🔗 论文地址：https://arxiv.org/abs/2303.17760
- 🔗 仓库地址：https://github.com/camel-ai/camel
- ⭐ GitHub Stars: 16k+
- 💡 推荐理由：最早系统研究 LLM Agent 间角色扮演通信的论文，提出用"任务指定 Agent"驱动"执行 Agent"的双 Agent 通信范式，是理解 Agent 对话如何被设计的经典入门文献

### 3.3 智能体团队如何「组织」？——组织结构补充

**LangGraph（基于图结构的 Agent 编排）**

- 🔗 仓库地址：https://github.com/langchain-ai/langgraph
- ⭐ GitHub Stars: 30k+
- 💡 推荐理由：将 Agent 协作流程建模为有向图（节点 = Agent/工具，边 = 消息流），支持条件分支、循环、并行执行，适合需要精确控制流程的复杂 MAS 场景

**MetaGPT（将公司 SOP 编码为 Agent 协作规范）**

- 🔗 论文地址：https://arxiv.org/abs/2308.00352
- 🔗 仓库地址：https://github.com/geekan/MetaGPT
- ⭐ GitHub Stars: 67k+
- 💡 推荐理由：将软件公司的标准操作流程（SOP）嵌入 Agent 角色定义，产品经理 → 架构师 → 工程师 → QA 的流水线协作，是“流水线式组织结构”最典型的实现，也是 GitHub 上最受关注的多 Agent 框架之一

### 3.4 智能体在什么「世界」里活动？——协作环境补充

**MultiAgentBench**

- 🔗 论文地址：https://arxiv.org/abs/2503.01935
- 🔗 仓库地址：https://github.com/ulab-uiuc/MARBLE
- 💡 推荐理由：MultiAgentBench 是一个模块化且可扩展的架构，支持开发者快速构建、测试和评估多智能体系统。它通过统一的 API 管理智能体间的通讯、共享内存和环境交互。

## 四、实战项目补充

### 4.1 GUI Agent

**UI-TARS**

- 🔗 仓库地址：https://github.com/bytedance/UI-TARS
- ⭐ GitHub Stars: 10k+
- 💡 推荐理由：字节开源的原生 GUI 交互 / 多模态智能体，支持桌面与移动端，结合 VLM 视觉理解与精准动作预测。与 MobileRun 相比更侧重模型能力。

**AgentCPM-GUI**

- 🔗 仓库地址：https://github.com/OpenBMB/AgentCPM-GUI
- ⭐ GitHub Stars: 1.4k+
- 💡 推荐理由：OpenBMB 社区开源的 GUI-Agent 强调轻量模型 + 强化学习微调，更适合端上隐私敏感场景与低延迟需求。

### 4.2 Computer Use Agent

**Anthropic Computer Use**

- 🔗 仓库地址：https://github.com/anthropics/anthropic-quickstarts
- ⭐ GitHub Stars: 16k+
- 💡 推荐理由：Anthropic 官方的 Computer Use 示例集合，提供操作系统级操作能力，适合跨应用、跨窗口的桌面自动化场景。

### 4.3 DeepResearch Agent

**dzhng/deep-research**

- 🔗 仓库地址：https://github.com/dzhng/deep-research
- ⭐ GitHub Stars: 18k+
- 💡 推荐理由：极简实现，适合快速理解 DeepResearch 原理、教学拆解或迁移到自己的技术栈。

### 4.6 金融智能体

**FinRobot（金融 Agent 平台，更推荐实战）**

- 🔗 仓库地址：https://github.com/AI4Finance-Foundation/FinRobot
- ⭐ GitHub Stars: 6k+
- 💡 推荐理由：FinGPT 的 Agent 进阶版，集成 LLM + 强化学习 + 量化分析三大能力，适合作为金融智能体实战的完整项目模板。
