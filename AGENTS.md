# AGENTS.md

这个仓库是《高性价比人生指南》的正文。

- **改这本书**（增删条目、改正文、动工具脚本）：规则全在 [CLAUDE.md](CLAUDE.md) 里，全部适用，先读完再动手。文件名叫 CLAUDE.md 只是历史原因，内容与工具无关。
- **用这本书回答问题**（有人问该不该做、值不值、怎么选、出事了先做什么、能领哪笔钱、犯不犯法）：按 [skills/life-decision-guide/SKILL.md](skills/life-decision-guide/SKILL.md) 执行，先查条目再答，答复里注明出自第几节第几条。装到别的目录去用的办法见 [skills/life-decision-guide/README.md](skills/life-decision-guide/README.md)。

- **做个人决策**（职业、学习、消费、迁移、长期规划等）：优先按 [skills/personal-decision-guide/SKILL.md](skills/personal-decision-guide/SKILL.md) 执行。需要《高性价比人生指南》的证据时，再调用 [skills/life-decision-guide/SKILL.md](skills/life-decision-guide/SKILL.md) 作为证据检索层。不要把个人敏感信息写进公开仓库。

- **所有 Skill 的成长机制**：无论调用哪个 Skill，完成主任务后都按 [skills/_shared/GROWTH_PROTOCOL.md](skills/_shared/GROWTH_PROTOCOL.md) 执行经验捕获、分级、验证和升级。单次案例不得直接改写通用规则；正式升级通过分支 + PR，并做最小回归测试。上游 Fork 保留的 Skill 默认用 overlay，不直接改原文件。

- **复杂系统理解**：当任务涉及架构、模块关系、能量/信息/控制链或局部问题的系统定位时，使用 [skills/system-modeling/SKILL.md](skills/system-modeling/SKILL.md)。
- **反馈与控制分析**：当任务涉及测量→判断→动作→反馈、延迟、阈值、振荡、反复异常或闭环失效时，使用 [skills/feedback-loop-analysis/SKILL.md](skills/feedback-loop-analysis/SKILL.md)。
- **任务闭环**：当任务需要把模糊要求变成可执行、可验收、可追踪的工作项时，使用 [skills/closed-loop-task-control/SKILL.md](skills/closed-loop-task-control/SKILL.md)。
- **证据核验**：当结论依赖规格书、标准、供应商回复、测试报告、论文或 AI 输出时，使用 [skills/evidence-verification/SKILL.md](skills/evidence-verification/SKILL.md) 区分事实、推断、假设与未知。

- **知识型回答统一规范**：历史、文学、哲学、电影、科学、工程、比较、翻译等知识型任务统一遵循 [skills/_shared/KNOWLEDGE_ANSWER_PROTOCOL.md](skills/_shared/KNOWLEDGE_ANSWER_PROTOCOL.md)。优先权威与一手信源，先给明确判断，区分事实/争议/接受史/推论，比较问题要说明结构差异、历史原因和实际后果；“继续”优先延续上一轮最相关未展开方向。若与安全、隐私、医疗法律边界或政治中立规则冲突，以更高优先级规则为准。
