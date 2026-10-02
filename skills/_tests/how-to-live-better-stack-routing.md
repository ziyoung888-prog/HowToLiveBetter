# HowToLiveBetter Skill Stack — Routing Regression

## 三层职责

| 层 | Skill | 负责 | 不负责 |
|---|---|---|---|
| Knowledge | how-to-live-better-knowledge | 找章节、条目、原文、证据、来源、适用条件 | 不单独做个性化决策 |
| Decision | life-decision-guide | 基于书的成本/收益/证据方法回答“该不该、值不值” | 不把用户长期目标当作已知事实 |
| Personal | personal-decision-guide | 加入用户目标、约束、机会成本、风险、长期复利 | 不把个人偏好伪装成书中证据 |

## Routing Cases

### A. “书里有没有说通勤？”
→ how-to-live-better-knowledge

### B. “每天通勤两小时值不值？”
→ life-decision-guide；知识层提供第 4 节原文

### C. “结合我现在的工作，我要不要为了缩短通勤搬家？”
→ personal-decision-guide；必要时调用 knowledge + life-decision

### D. “低钠盐这条的研究出处是什么？”
→ how-to-live-better-knowledge

### E. “我适不适合换低钠盐？”
→ 涉及个人健康条件，不由 knowledge skill 直接判断；读取书中适用条件后进入相应高风险专业流程

## 冲突判据

以下情况视为职责漂移：
- knowledge skill 在没有个人上下文分析的情况下直接替用户做重大决策；
- personal skill 把自身推断写成书中结论；
- life-decision skill 不读取原文就凭记忆补条目；
- 三个 skill 同时维护正文数字副本，造成来源漂移。

## 当前结论

三层可以共存。新 Skill 应被视为底层“检索/证据接口”，不是 life-decision-guide 的替代品。
