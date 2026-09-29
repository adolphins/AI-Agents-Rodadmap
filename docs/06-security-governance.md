# 第 6 层：安全、治理与评测【全程贯穿】

> 学习目标：掌握 Agent 系统的安全防护、治理方案、评测体系

---

## 学习要点

### Prompt Injection 与防护

- [ ] Prompt Injection 的原理与攻击方式
- [ ] 防护策略与输入验证
- [ ] Prompt 沙箱化设计
- [ ] 用户输入的安全处理

### Tool 安全

- [ ] Tool 调用的安全审查
- [ ] Tool 的权限控制与隔离
- [ ] Tool 调用的日志记录与审计
- [ ] 恶意 Tool 调用的检测与防止

### 可观测性与审计

- [ ] Trace 的设计与追踪
- [ ] 详细的操作审计日志
- [ ] Agent 决策过程的可解释性
- [ ] 用户行为的监控

### 成本与 Token 监控

- [ ] Token 使用量的准确计数
- [ ] 成本预算与警告机制
- [ ] 异常费用检测
- [ ] 模型成本优化

### 离线评测与回归测试

- [ ] RAG 的离线评测方法（Ragas、DeepEval）
- [ ] Agent 的评估框架
- [ ] 性能基准与回归测试
- [ ] 持续集成中的评测

### 治理与合规

- [ ] 数据隐私与 GDPR
- [ ] 模型偏差与公平性
- [ ] 使用政策与用户协议
- [ ] 风险评估与规避

---

## 推荐学习资源

| 资源 | 链接 | 说明 |
|------|------|------|
| **DeepEval** | [GitHub](https://github.com/confident-ai/deepeval) | Agent 离线评估框架 |
| **Ragas** | [GitHub](https://github.com/explodinggradients/ragas) | RAG/Agent 评估框架 |
| **roadmap.sh - AI Engineer** | [路线图](https://roadmap.sh/ai-engineer) | 安全与治理专区 |

---

## 学习建议

1. **从一开始就设计安全**：不要等问题出现再补救
2. **多层防护**：采用分层防护策略，单一防线容易被绕过
3. **充分记录**：详细的日志是事后分析的关键
4. **定期评测**：建立持续的评测和监控机制

---

更详细的资源列表见：[reference/learning-resources.md](../reference/learning-resources.md)

---

**返回**：[知识体系总览](./README.md)
