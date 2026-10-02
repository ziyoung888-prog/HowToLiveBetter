# how-to-live-better-knowledge

由 `book-to-skill 1.4.0` 的项目级思路生成的《高性价比人生指南》知识层。

## 为什么不是复制整本书

原始正文已经存在于仓库的 `book/`。再次复制会造成：
- 内容重复；
- 上游正文更新后两份内容漂移；
- Skill 体积膨胀；
- 难以确认哪一份才是权威来源。

因此本 Skill 采用“轻索引 + 原文按需加载”：
- `SKILL.md`：调用规则；
- `chapters/`：34 个章节路由；
- `cheatsheet.md`：主题快速映射；
- `patterns.md`：跨章节可复用模式；
- `glossary.md`：书内机器可读概念；
- 原始事实和数字：仍读 `book/*.md`。

## 与其他 Skill 的关系

```
how-to-live-better-knowledge
        ↓ 提供原文/证据/章节
life-decision-guide
        ↓ 通用决策
personal-decision-guide
        ↓ 个人目标与约束
行动建议
```

## 更新

正文新增/删除章节时：
1. 更新章节路由；
2. 更新 cheatsheet；
3. 运行回归测试；
4. 不需要复制正文。
