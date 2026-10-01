# personal-decision-guide

这是 `life-decision-guide` 上层的个人决策 skill。

## 两层架构

```
用户问题
  ↓
personal-decision-guide
  ├─ 校验前提
  ├─ 读取个人目标和约束
  ├─ 调用 life-decision-guide 查证据
  ├─ 比较风险 / 机会成本 / 可逆性 / 长期复利
  └─ 给建议、行动、复查点
        ↓
life-decision-guide
  └─ 从《高性价比人生指南》检索并引用相关条目
```

原版 `life-decision-guide` 不修改，继续作为证据检索层。

## 为什么不用总分

人生决策经常跨不同量纲：钱、时间、健康、职业资本、风险和选择权不能可靠地压成一个数字。这个 skill 默认做结构化比较，不输出伪精确的综合分数。

## 个人资料怎么放

这个 Fork 是公开仓库。不要把真实姓名、薪资、健康、公司内部信息、联系方式等敏感背景提交到 GitHub。

本地可复制：

```
personal/PERSONAL_CONTEXT.example.md
→
personal/PERSONAL_CONTEXT.md
```

`PERSONAL_CONTEXT.md` 已加入 `.gitignore`，只保存在本机。

也可以完全不建这个文件，让 agent 使用当前对话里已知的上下文。

## 调用方式

在支持 skill 的 agent 中可以显式调用 `personal-decision-guide`，也可以直接问：

- 我该不该跳槽？
- 这个证值得不值得考？
- A 和 B 哪个更适合我现在？
- 我要不要花三个月学这个技能？
- 这个选择的最大风险是什么？

对于指南能覆盖的问题，本 skill 应先调用 `life-decision-guide`，而不是重复维护证据。
