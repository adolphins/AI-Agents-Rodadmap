# 第 4 层：Agent 与工具调用【核心】⭐

> 学习目标：理解 Agent 的本质、掌握 Function Calling、学会设计 Agent 架构

---

## 学习要点

### Agent 核心概念

- [ ] 什么是 Agent？定义与三个核心部分
- [ ] Agent 的 5 大核心特征（自主性、目标导向、适应性、推理能力、工具使用）
- [ ] Agent vs Workflow vs Assistant 的区别与适用场景
- [ ] Agent 的优势与限制

### Function Calling 与 Tool Use

- [ ] Function Calling 的本质与工作原理
- [ ] Tool 的三要素（名称、描述、参数定义）
- [ ] Tool 的设计最佳实践
- [ ] Function Calling vs ReAct Prompting vs Workflow 的对比

### Agent 设计模式

- [ ] **Reflection** 模式 - 反思与自我纠正
  - 工作流程、适用场景、优缺点
  
- [ ] **Tool Use** 模式 - 工具调用
  - 工作流程、适用场景、优缺点
  
- [ ] **Planning** 模式 - 计划制定
  - 工作流程、适用场景、优缺点
  
- [ ] **Multi-Agent Collaboration** 模式 - 多智能体协作
  - 工作流程、适用场景、协作模式、优缺点

### Agent 工作流设计

- [ ] **ReAct 模式**（Reasoning + Acting）
  - 核心循环、优缺点、何时使用
  
- [ ] **Plan-and-Execute 模式**
  - 流程、优缺点、何时使用
  
- [ ] **Router 模式**（路由模式）
  - 流程、优缺点、何时使用

### MCP 协议详解

- [ ] MCP 的定义与核心理念
- [ ] MCP 的三个关键概念
  - Server（服务器）- 常见类型
  - Client（客户端）- 常见类型
  - Tool（工具）- 标准定义
  
- [ ] MCP 的完整工作流程
- [ ] MCP vs Function Calling 对比
- [ ] MCP 的应用场景（数据访问、系统集成、工具标准化）
- [ ] MCP 与 eDC 的关系

### 工具集成

- [ ] API、数据库、SaaS 工具的集成
- [ ] 浏览器自动化工具
- [ ] Human-in-the-Loop 人工审批机制

---

## 推荐学习资源

| 资源 | 链接 | 说明 |
|------|------|------|
| **mlabonne/llm-course** | [GitHub](https://github.com/mlabonne/llm-course) | 完整 LLM 工程师课程，含 Agent 模块 |
| **DeepLearning.AI - Design Patterns** | [课程](https://learn.deeplearning.ai/courses/ai-agents-in-langgraph) | Agent 4 大设计模式深入讲解 |
| **DeepLearning.AI - LangGraph** | [课程](https://learn.deeplearning.ai/courses/langgraph) | 有状态 Agent 构建 |
| **Anthropic - Building Effective Agents** | [指南](https://www.anthropic.com/research/building-effective-agents) | 何时用 Agent，何时用 Workflow |
| **OpenAI Function Calling** | [文档](https://platform.openai.com/docs/guides/function-calling) | Function Calling 官方指南 |
| **MCP 官方文档** | [文档](https://modelcontextprotocol.io) | 标准化工具集成协议 |
| **ReAct 论文** | [论文](https://react-lm.github.io/) | ReAct 模式的原始论文 |
| **500+ AI Agents Projects** | [GitHub](https://github.com/ashishpatel26/500-AI-Agents-Projects) | 实战案例库 |

---

## 学习建议

1. **先理论后实践**：先理解 Agent 的本质，再看具体实现
2. **对标真实场景**：思考如何在自己的应用中使用 Agent（如 eDC）
3. **选择一个框架深入**：建议从 LangGraph 开始，学会了再看其他框架
4. **充分测试工具**：Tool 设计得好坏直接影响 Agent 的性能

---

更详细的框架对比见：[reference/framework-comparison.md](../reference/framework-comparison.md)

更详细的资源列表见：[reference/learning-resources.md](../reference/learning-resources.md)

---

**返回**：[知识体系总览](./README.md)
