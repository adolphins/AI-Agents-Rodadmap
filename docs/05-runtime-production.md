# 第 5 层：Runtime 与生产化【核心】⭐

> 学习目标：掌握 Agent 的生产部署、状态管理、可观测性

---

## 学习要点

### 会话与任务状态管理

- [ ] Agent 的会话状态设计
- [ ] 任务状态与生命周期
- [ ] Checkpoint 与断点续行
- [ ] 状态持久化与恢复

### 生产可靠性

- [ ] 重试机制与指数退避
- [ ] 超时管理与降级策略
- [ ] 异步任务与队列处理
- [ ] 并发控制与限流

### Sandbox 与权限管理

- [ ] 沙箱隔离的设计
- [ ] 权限传递与权限模型
- [ ] 工具调用的权限控制
- [ ] SQL 注入与命令注入防护

### API Gateway 与服务架构

- [ ] API 网关的设计
- [ ] 请求限流与熔断
- [ ] 缓存策略
- [ ] 模型降级与备选方案

### 部署与运维

- [ ] Agent 服务的部署架构
- [ ] 容器化与编排（Docker、Kubernetes）
- [ ] 日志收集与存储
- [ ] 监控与告警

---

## 推荐学习资源

| 资源 | 链接 | 说明 |
|------|------|------|
| **LangGraph Academy** | [文档](https://langchain-ai.github.io/langgraph/) | 状态管理与持久化 |
| **LangSmith** | [文档](https://smith.langchain.com/) | Agent 监控和调试工具 |
| **Langfuse** | [文档](https://langfuse.com/) | 开源 LLM 应用可观测性平台 |
| **roadmap.sh - AI Engineer** | [路线图](https://roadmap.sh/ai-engineer) | 完整的工程化路线 |

---

## 学习建议

1. **不要忽视可观测性**：生产环境中，日志和监控比代码本身更重要
2. **充分的测试**：在真实场景中测试各种边界情况和故障场景
3. **渐进式部署**：从小规模试点开始，逐步扩大规模
4. **成本意识**：时刻关注 API 调用的成本，设计成本控制机制

---

更详细的资源列表见：[reference/learning-resources.md](../reference/learning-resources.md)

---

**返回**：[知识体系总览](./README.md)
