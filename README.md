# OpenClaw Superpowers

## 中文说明

**轻量级复杂任务执行技能集（OpenClaw 风格 Agent 系统）**

这个项目打包了一套可复用的工作流层，适用于多步骤、高风险、长耗时，或在对外汇报完成前需要明确验证的任务。

### 它能做什么

它增加了 6 个可复用的执行构件：

- task-shaping
- plan-and-slice
- delegation-contract
- verify-before-done
- checkpoint-recap
- delivery-closeout

目标很简单：

> 让复杂任务更稳，但不拖慢简单任务。

### 项目结构

```text
.
├── zh/
│   └── openclaw-superpowers/
│       ├── SKILL.md
│       └── references/
└── en/
    └── openclaw-superpowers/
        ├── SKILL.md
        └── references/
```

### 语言版本

- 中文版本：`zh/openclaw-superpowers/`
- 英文版本：`en/openclaw-superpowers/`

### 致谢说明

本项目参考并改编自：

- https://github.com/obra/superpowers

更多说明见 `ATTRIBUTION.md`。

### 说明

- 本仓库保持技能主体简洁，把细节放进 `references/`。
- 公开版本移除了宿主环境特定引用和私有工作流绑定。
- 你可以直接使用，也可以按自己的 Agent 运行环境调整文案和触发阈值。

## License

MIT
