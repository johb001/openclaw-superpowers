# OpenClaw Superpowers

一个面向复杂任务的轻量工作流 skill family，适用于 OpenClaw 风格的 Agent 运行环境。

它解决的不是“不会做”，而是复杂任务里常见的几类问题：

- 没定型就开干
- 大任务糊成一坨
- 分派不清，回流混乱
- 没验证就报完成
- 长任务中途断层
- 对外汇报过程噪音太重

## 它提供什么

- `task-shaping`
- `plan-and-slice`
- `delegation-contract`
- `verify-before-done`
- `checkpoint-recap`
- `delivery-closeout`

一句话目标：

> 只增强复杂任务，不拖慢简单任务。

## 仓库结构

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

## 语言版本

- 中文版：`zh/openclaw-superpowers/`
- 英文版：`en/openclaw-superpowers/`

## 归因

本项目参考并改造自：

- https://github.com/obra/superpowers

详细说明见：`ATTRIBUTION.md`

## 说明

- skill 主体保持精简，细节放在 `references/` 里
- 公开版已去掉宿主私有路径和本地绑定表述
- 可以直接用，也可以按你自己的 Agent 运行环境继续改

## License

MIT
