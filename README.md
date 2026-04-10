# OpenClaw Superpowers

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
  <img src="https://img.shields.io/badge/language-zh%20%2F%20en-brightgreen.svg" alt="Language">
  <img src="https://img.shields.io/badge/status-active-success.svg" alt="Status">
  <img src="https://img.shields.io/badge/openclaw-skill-purple.svg" alt="OpenClaw Skill">
</p>

面向 OpenClaw 风格 Agent 系统的复杂任务执行技能集。

本项目提供一套可复用的复杂任务执行工作流，用于处理多步骤、高风险、长耗时，或在对外汇报完成前需要明确验证的任务。它的目标不是增加流程负担，而是在复杂场景下补齐任务塑形、拆解、委派、校验、阶段收口与最终交付这些关键环节。

## 项目定位

OpenClaw Superpowers 适用于以下场景：

- 任务步骤多，容易在执行中失焦
- 任务风险高，不能“看起来做了”就算完成
- 任务耗时长，需要阶段性收口与续做能力
- 任务涉及协作、委派或跨角色回流
- 任务在对外汇报前，必须有明确验证证据

核心目标：

> 让复杂任务更稳，不因流程失控；让简单任务更快，不被额外流程拖慢。

## 核心能力

本项目提供 6 个可复用的执行构件：

- **task-shaping**：在开工前明确任务目标、边界、完成标准与风险点
- **plan-and-slice**：将复杂任务拆成可执行、可验证、可回流的小阶段
- **delegation-contract**：为委派任务补齐目标、验收标准、验证要求与回流格式
- **verify-before-done**：在汇报完成前先做最小但有效的结果验证
- **checkpoint-recap**：在长任务中定期整理当前目标、已完成、卡点与下一步
- **delivery-closeout**：交付前统一收口结果、状态、证据与后续动作

## 适用场景示例

你可以在以下类型的任务中使用本项目：

- **工程实现任务**：先定义完成标准，再拆解实现步骤，最后以验证结果作为完成依据
- **多 Agent 协作任务**：为委派补齐契约，要求每个子任务都能独立回流与验收
- **长耗时项目推进**：通过阶段性 checkpoint 防止任务失焦、断层或重复沟通
- **高风险改动任务**：在删除、覆盖、配置调整、权限变更等动作前后保留明确验证节点
- **对外交付任务**：在正式汇报前统一收口“结果 / 证据 / 风险 / 下一步”

## 快速开始

### 1. 选择语言目录

根据你的使用语言选择技能目录：

- 中文版本：`zh/openclaw-superpowers/`
- 英文版本：`en/openclaw-superpowers/`

### 2. 复制到你的技能目录

将对应目录复制到你的 AgentSkills / skills 工作区中。

### 3. 按需调整触发条件

建议优先根据你的运行环境调整以下内容：

- 何时触发复杂任务增强流程
- 什么情况下必须先验证再汇报完成
- 多 Agent 委派时的契约格式
- 长任务阶段收口的频率与模板

## 使用方式

你可以按以下方式使用本项目：

- 直接作为技能模板使用
- 按自己的 Agent 运行环境调整触发条件与执行阈值
- 仅保留部分执行构件，组合成更轻量的流程
- 结合自己的委派、验收、回流机制进行二次封装

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

## 目录说明

- `zh/openclaw-superpowers/`：中文版本技能内容
- `en/openclaw-superpowers/`：英文版本技能内容
- `references/`：补充说明、细节规则与扩展资料

> 当前 README 以中文介绍为主，便于中文用户快速理解项目定位；仓库中仍保留英文目录，便于后续维护多语言版本。

## 设计原则

- **复杂任务增强，简单任务不打扰**
- **先定义完成，再开始执行**
- **先验证结果，再对外汇报**
- **长任务要有阶段收口，避免失焦和断层**
- **委派要有契约，回流要有格式**

## 路线图

后续可继续完善的方向包括：

- 增加更多任务场景示例
- 补充不同 Agent 平台的适配说明
- 提供更标准化的委派与回流模板
- 补充验证清单、验收卡和阶段收口模板
- 增加更轻量或更严格的流程变体

## 致谢说明

本项目参考并改编自：

- https://github.com/obra/superpowers

更多说明见 `ATTRIBUTION.md`。

## 补充说明

- 本仓库保持技能主体简洁，将扩展说明与细节放在 `references/` 中。
- 公开版本移除了宿主环境特定引用和私有工作流绑定。
- 如需适配不同 Agent 平台，可按自身运行时能力调整触发逻辑、分工边界与交付规范。

## 许可证

MIT
