# Stage 3 Supply

## 3.1 什么是多智能体系统：任务驱动协作、自治群体交互

### 推荐课程补充

**HuggingFace Agents Course（系统入门首选）**

- 🔗 课程地址：https://huggingface.co/learn/agents-course/
- 💡 推荐理由：HuggingFace 官方出品，从单 Agent 基础到多 Agent 协作循序渐进，配有可直接运行的代码实践，是目前最完整的开源 Agent 入门课程

### 代表系统精读补充

**Generative Agents：斯坦福小镇（自治群体交互）**

- 🔗 论文地址：https://arxiv.org/abs/2304.03442
- 💡 重点理解：25 个 Agent 在模拟小镇中自主生活、社交、形成记忆，展示了 LLM 驱动的群体涌现行为。核心机制：记忆流（Memory Stream）+ 反思（Reflection）+ 行动规划（Planning）

### 延伸阅读

**A Survey on LLM-based Autonomous Agents（全景综述）**

- 🔗 论文地址：https://arxiv.org/abs/2308.11432
- 💡 推荐理由：全面梳理 LLM Agent 的记忆、规划、工具使用与多 Agent 协作四大模块，适合在深入某个方向前建立完整的认知框架

**Large Language Model based Multi-Agents: A Survey of Progress and Challenges（多智能体专项综述）**

- 🔗 论文地址：https://arxiv.org/abs/2402.01680
- 💡 推荐理由：专注于多 Agent 系统本身，系统梳理 LLM 驱动的多 Agent 在通信、组织、环境与应用上的最新进展与挑战

## 3.2 智能体之间如何「说话」？——交互协议

### 推荐阅读补充

**CAMEL（角色扮演的多 Agent 通信范式）**

- 🔗 论文地址：https://arxiv.org/abs/2303.17760
- 🔗 仓库地址：https://github.com/camel-ai/camel
- ⭐ GitHub Stars: 16k+
- 💡 推荐理由：最早系统研究 LLM Agent 间角色扮演通信的论文，提出用"任务指定 Agent"驱动"执行 Agent"的双 Agent 通信范式，是理解 Agent 对话如何被设计的经典入门文献

## 3.3 智能体团队如何「组织」？——组织结构

### 推荐阅读补充

**LangGraph（基于图结构的 Agent 编排）**

- 🔗 仓库地址：https://github.com/langchain-ai/langgraph
- ⭐ GitHub Stars: 30k+
- 💡 推荐理由：将 Agent 协作流程建模为有向图（节点 = Agent/工具，边 = 消息流），支持条件分支、循环、并行执行，适合需要精确控制流程的复杂 MAS 场景

**MetaGPT（将公司 SOP 编码为 Agent 协作规范）**

- 🔗 论文地址：https://arxiv.org/abs/2308.00352
- 🔗 仓库地址：https://github.com/geekan/MetaGPT
- ⭐ GitHub Stars: 67k+
- 💡 推荐理由：将软件公司的标准操作流程（SOP）嵌入 Agent 角色定义，产品经理 → 架构师 → 工程师 → QA 的流水线协作，是“流水线式组织结构”最典型的实现，也是 GitHub 上最受关注的多 Agent 框架之一

## 3.4 智能体在什么「世界」里活动？——协作环境

### 推荐阅读补充

**MultiAgentBench**

- 🔗 论文地址：https://arxiv.org/abs/2503.01935
- 🔗 仓库地址：https://github.com/ulab-uiuc/MARBLE
- 💡 推荐理由：MultiAgentBench 是一个模块化且可扩展的架构，支持开发者快速构建、测试和评估多智能体系统。它通过统一的 API 管理智能体间的通讯、共享内存和环境交互。
