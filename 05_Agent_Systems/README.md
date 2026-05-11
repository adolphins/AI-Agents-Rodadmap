# 🤖 阶段五：高阶 Agent 与多智能体系统

> **"Stop typing, start delegating."** 
> 让模型不仅能“说”，还能“做”。通过赋予大模型使用工具（Tools）的能力，以及多智能体协同（Multi-Agent），构建真正的自动化 Agent 工作流。

## 🎯 核心目标
1. 深刻理解 **ReAct** (Reasoning and Acting) 范式。
2. 掌握 Function Calling 机制，让模型自主调用外部 API（如查天气、查数据库）。
3. 掌握 **LangGraph** 框架，将大模型的不确定性转化为确定性的状态机工作流。
4. 实现多智能体协作（如 Router Agent 路由给特定的 Worker Agent）。

---

## 📚 优质学习资源推荐

### 📺 视频教程
* [YouTube] [DeepLearning.AI: AI Agents in LangGraph](https://learn.deeplearning.ai/courses/ai-agents-in-langgraph) *(LangChain 官方出的神级教程)*
* [Bilibili] [多智能体系统开发：AutoGen vs CrewAI vs LangGraph](https://www.bilibili.com/video/BV1Jw411h7Z5)

### 📖 文章与指南
* [LangGraph 官方文档](https://langchain-ai.github.io/langgraph/)
* [OpenAI - Function Calling 指南](https://platform.openai.com/docs/guides/function-calling)
* [ReAct 论文原理解析](https://react-lm.github.io/)

---

## 💻 练习与代码记录

- [ ] **`01_react_agent/` - ReAct 范式**
  - [ ] 手写一个简易的 Prompt 实现 ReAct 循环
  - [ ] 使用大模型实现算数计算器的自主调用
- [ ] **`02_tools_and_mcp/` - 工具调用**
  - [ ] 定义自定义 Tool（Python 函数映射到 LLM 工具）
  - [ ] 结合 FastAPI 编写可供 Agent 调用的天气/股票 API
  - [ ] 了解并测试最新的 MCP (Model Context Protocol)
- [ ] **`03_langgraph_flows/` - LangGraph 实战**
  - [ ] 定义 State、Node 和 Edge，构建状态机图
  - [ ] 在节点中引入 Human-in-the-loop (人工审批环节)
- [ ] **`04_multi_agent/` - 多智能体协同**
  - [ ] 构建一个主控 Router 节点，负责分发任务给下游专门的 Agent

---

## 🏆 阶段实战项目：多意图旅行智能助手 (Smart Voyage Agent)

**项目说明:**
使用 LangGraph 构建多 Agent 协同系统。用户输入一段复杂需求（如：“我想去北京，查一下明天的天气，然后帮我定一张早上从上海出发的高铁票”），系统能将意图拆分，分发给“天气 Agent”和“票务 Agent”，最终通过“汇总 Agent”格式化输出结果。