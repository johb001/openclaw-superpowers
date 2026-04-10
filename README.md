# OpenClaw Superpowers

[中文](#中文说明) | [English](#english)

---

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

---

## English

**A lightweight skill family for complex-task execution in OpenClaw-style agent systems.**

This project packages a reusable workflow layer for tasks that are multi-step, high-risk, long-running, or require explicit verification before being reported as done.

### What it does

It adds six reusable execution building blocks:

- task-shaping
- plan-and-slice
- delegation-contract
- verify-before-done
- checkpoint-recap
- delivery-closeout

The goal is simple:

> Strengthen complex work without slowing simple work down.

### Project structure

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

### Language versions

- Chinese version: `zh/openclaw-superpowers/`
- English version: `en/openclaw-superpowers/`

### Attribution

This project is adapted with inspiration from:

- https://github.com/obra/superpowers

See `ATTRIBUTION.md` for details.

### Notes

- This repository keeps the skill body lean and puts details into `references/`.
- The public version removes host-specific references and private workflow bindings.
- You can use it as-is, or adapt the wording and trigger thresholds to your own agent runtime.

## License

MIT
