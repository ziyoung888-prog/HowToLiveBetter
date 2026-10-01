# AGENTS.md

这个仓库是《高性价比人生指南》的正文。

- **改这本书**（增删条目、改正文、动工具脚本）：规则全在 [CLAUDE.md](CLAUDE.md) 里，全部适用，先读完再动手。文件名叫 CLAUDE.md 只是历史原因，内容与工具无关。
- **用这本书回答问题**（有人问该不该做、值不值、怎么选、出事了先做什么、能领哪笔钱、犯不犯法）：按 [skills/life-decision-guide/SKILL.md](skills/life-decision-guide/SKILL.md) 执行，先查条目再答，答复里注明出自第几节第几条。装到别的目录去用的办法见 [skills/life-decision-guide/README.md](skills/life-decision-guide/README.md)。

- **做个人决策**（职业、学习、消费、迁移、长期规划等）：优先按 [skills/personal-decision-guide/SKILL.md](skills/personal-decision-guide/SKILL.md) 执行。需要《高性价比人生指南》的证据时，再调用 [skills/life-decision-guide/SKILL.md](skills/life-decision-guide/SKILL.md) 作为证据检索层。不要把个人敏感信息写进公开仓库。

- **所有 Skill 的成长机制**：无论调用哪个 Skill，完成主任务后都按 [skills/_shared/GROWTH_PROTOCOL.md](skills/_shared/GROWTH_PROTOCOL.md) 执行经验捕获、分级、验证和升级。单次案例不得直接改写通用规则；正式升级通过分支 + PR，并做最小回归测试。上游 Fork 保留的 Skill 默认用 overlay，不直接改原文件。
