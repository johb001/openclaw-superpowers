# OpenClaw Superpowers

轻量级复杂任务执行技能集，面向 OpenClaw 风格的 Agent 系统。

本项目提供一套可复用的复杂任务执行工作流，用于处理多步骤、高风险、长耗时，或在对外汇报完成前需要明确验证的任务。

## 核心能力

本项目提供 6 个可复用的执行构件：

- task-shaping
- plan-and-slice
- delegation-contract
- verify-before-done
- checkpoint-recap
- delivery-closeout

核心目标：

> 让复杂任务更稳，不因流程失控；让简单任务更快，不被额外流程拖慢。

## 项目结构

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

## 语言目录

- 中文目录：`zh/openclaw-superpowers/`

> 仓库中仍保留 `en/` 目录作为英文技能文件目录，但 README 介绍部分当前仅保留中文。

## 致谢说明

本项目参考并改编自：

- https://github.com/obra/superpowers

更多说明见 `ATTRIBUTION.md`。

## 说明

- 本仓库保持技能主体简洁，将扩展说明与细节放在 `references/` 中。
- 公开版本移除了宿主环境特定引用和私有工作流绑定。
- 你可以直接使用，也可以按自己的 Agent 运行环境调整文案、触发条件与执行阈值。

## License

MIT
