# OpenClaw Superpowers

轻量级复杂任务执行技能集（OpenClaw 风格 Agent 系统）  
A lightweight skill family for complex-task execution in OpenClaw-style agent systems.

这个项目打包了一套可复用的工作流层，适用于多步骤、高风险、长耗时，或在对外汇报完成前需要明确验证的任务。  
This project packages a reusable workflow layer for tasks that are multi-step, high-risk, long-running, or require explicit verification before being reported as done.

## What it does / 它能做什么

It adds six reusable execution building blocks:  
它增加了 6 个可复用的执行构件：

- task-shaping
- plan-and-slice
- delegation-contract
- verify-before-done
- checkpoint-recap
- delivery-closeout

The goal is simple:  
目标很简单：

> Strengthen complex work without slowing simple work down.  
> 让复杂任务更稳，但不拖慢简单任务。

## Project structure / 项目结构

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

## Language versions / 语言版本

- Chinese version / 中文版本：`zh/openclaw-superpowers/`
- English version / 英文版本：`en/openclaw-superpowers/`

## Attribution / 致谢说明

This project is adapted with inspiration from:  
本项目参考并改编自：

- https://github.com/obra/superpowers

See `ATTRIBUTION.md` for details.  
更多说明见 `ATTRIBUTION.md`。

## Notes / 说明

- This repository keeps the skill body lean and puts details into `references/`.  
  本仓库保持技能主体简洁，把细节放进 `references/`。
- The public version removes host-specific references and private workflow bindings.  
  公开版本移除了宿主环境特定引用和私有工作流绑定。
- You can use it as-is, or adapt the wording and trigger thresholds to your own agent runtime.  
  你可以直接使用，也可以按自己的 Agent 运行环境调整文案和触发阈值。

## License / 许可证

MIT
