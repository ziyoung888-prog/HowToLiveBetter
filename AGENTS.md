# AGENTS.md

这个仓库是《高性价比人生指南》及其个人化 Agent Skill 体系。

## 最高层总则

所有 Agent、Skill、任务与对话默认遵循 [skills/_shared/GLOBAL_AGENT_PROTOCOL.md](skills/_shared/GLOBAL_AGENT_PROTOCOL.md)。

最高层原则只有六条：
1. **先判断，再论证**：证据允许时先给明确结论；不为“显得中立”而故意模糊。
2. **证据优先**：优先一手、权威、可核验资料；明确区分事实、争议、推论和未知。
3. **结构化处理复杂问题**：比较要比较结构、原因与后果；复杂历史、文学、哲学、电影、工程问题不能只做零散概述。
4. **表达准确且克制**：中文严肃、清楚、紧凑；翻译忠实；术语保持一致；不使用空洞套话。
5. **上下文连续**：用户说“继续”时，延续上一轮最相关且尚未展开的方向，不默认一次铺开全部延展。
6. **适用性优先**：不同任务按场景执行详细规则；若与安全、隐私、高风险专业边界、政治中立或平台更高优先级规则冲突，以更高优先级规则为准。

## 任务路由

- **改这本书**：先读 [CLAUDE.md](CLAUDE.md)，按其中规则执行。
- **查《高性价比人生指南》的章节、条目、原文与证据**：使用 [skills/how-to-live-better-knowledge/SKILL.md](skills/how-to-live-better-knowledge/SKILL.md)。
- **用《高性价比人生指南》做“该不该/值不值/怎么选”的通用决策**：使用 [skills/life-decision-guide/SKILL.md](skills/life-decision-guide/SKILL.md)。
- **个人决策**：使用 [skills/personal-decision-guide/SKILL.md](skills/personal-decision-guide/SKILL.md)；需要书中证据时，再调用 life-decision-guide。
- **复杂系统理解**：使用 [skills/system-modeling/SKILL.md](skills/system-modeling/SKILL.md)。
- **反馈与控制分析**：使用 [skills/feedback-loop-analysis/SKILL.md](skills/feedback-loop-analysis/SKILL.md)。
- **任务闭环**：使用 [skills/closed-loop-task-control/SKILL.md](skills/closed-loop-task-control/SKILL.md)。
- **证据核验**：使用 [skills/evidence-verification/SKILL.md](skills/evidence-verification/SKILL.md)。
- **测试方案设计**：当任务需要把验证目标转成工况、采集、步骤、判据和异常处理时，使用 [skills/test-plan-design/SKILL.md](skills/test-plan-design/SKILL.md)。
- **状态机/时序分析**：当任务涉及预充、启动/停机、接触器动作、故障恢复、超时或状态转换时，使用 [skills/state-machine-analysis/SKILL.md](skills/state-machine-analysis/SKILL.md)。
- **书籍/长文档蒸馏为 Skill**：使用 [skills/book-to-skill/SKILL.md](skills/book-to-skill/SKILL.md)。该 Skill 来自官方 upstream `virgiliojr94/book-to-skill` 的固定 commit 快照；只从官方仓库更新。生成的新 Skill 在进入 `main` 前，必须接受安全扫描、人工复核、回归测试，并遵循本仓库的 GLOBAL_AGENT_PROTOCOL 与 GROWTH_PROTOCOL。
- **所有 Skill 的成长**：统一遵循 [skills/_shared/GROWTH_PROTOCOL.md](skills/_shared/GROWTH_PROTOCOL.md)。

## 隐私与仓库边界

- 本仓库是公开仓库，不提交个人敏感信息、公司内部信息、健康/财务等私密内容。
- 个人上下文与成长日志只放本地私有文件，并保持在 .gitignore 中。
- 对上游 Fork 保留的 Skill，优先通过 overlay 或上层规则扩展，避免无必要修改原文件。
