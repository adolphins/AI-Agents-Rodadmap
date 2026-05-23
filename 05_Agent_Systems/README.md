# Phase 5: Agent Systems & Multi-Agent Orchestration

> Stop typing, start delegating. Build AI that can plan, act, and collaborate.

## Goals

- Understand the **ReAct** paradigm (Thought → Action → Observation).
- Implement **Function Calling** and tool use (APIs, databases).
- Orchestrate complex workflows with **LangGraph** (state machines).
- Design **multi-agent** systems (router agent + specialized worker agents).

## Resources

- **Course:** [DeepLearning.AI - AI Agents in LangGraph](https://learn.deeplearning.ai/courses/ai-agents-in-langgraph) | [AutoGen vs CrewAI vs LangGraph](https://www.bilibili.com/video/BV1Jw411h7Z5)
- **Docs:** [LangGraph Docs](https://langchain-ai.github.io/langgraph/) | [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling)
- **Paper:** [ReAct](https://react-lm.github.io/)

## Project: Smart Voyage Agent

Build a multi-agent travel assistant using **LangGraph**.

Requirements:
- Parse complex user requests (e.g., "Check Beijing weather tomorrow, then book a morning train from Shanghai")
- Route intents to specialized agents: Weather Agent, Ticketing Agent
- Summarize and format final output for the user
