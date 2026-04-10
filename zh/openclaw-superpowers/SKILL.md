---
name: openclaw-superpowers
description: Use when tasks are complex, multi-step, high-risk, require multiple agents, or need explicit validation before being reported as done. Adds a lightweight closed-loop workflow for shaping work, slicing plans, delegating clearly, verifying before completion, and checkpointing long tasks.
---

# OpenClaw Superpowers

为复杂任务提供一层轻量闭环增强：只增强复杂任务，不拖慢简单任务。

## 何时使用

只有当任务同时具备“复杂度”或“风险”时，才触发本 skill。常见触发情况：

- 明显是多步骤任务
- 涉及工程实现、配置修改、自动化落地，且不能只做一步就收口
- 任务周期较长，存在中途中断或续做风险
- 需要多智能体协作
- 属于高风险操作
- 需要显式验证，不能直接按“已完成”汇报

以下场景默认不触发，或只局部借用其中一个子能力：

- 简单问答
- 轻建议
- 一步能答完的小事
- 纯闲聊
- 单次低风险信息查询
- 已经非常清晰、可直接执行、且不需要额外验证的小改动

## 核心原则

- 先定型，再开干
- 先验证，再汇报
- 长任务要阶段收口
- 分派必须写清契约
- 流程服务结果，不制造额外摩擦

## 默认工作流

根据任务类型，从下列子能力中按需组合，不要求每次全用：

1. **task-shaping**：先把目标、完成标准、边界说清
2. **plan-and-slice**：把复杂任务拆成可控小块（增强项，后补）
3. **delegation-contract**：给子智能体写清目标、完成标准、验证要求、回流格式
4. **verify-before-done**：对外宣布完成前做最小验证
5. **checkpoint-recap**：长任务中途按阶段收口
6. **delivery-closeout**：把内部结果收成用户可直接消费的交付格式（增强项，后补）

当前 MVP 只落地 1 / 3 / 4 / 5，未落地的能力只作为后续扩展占位，不应假定已可直接调用。

## 第一阶段（MVP）

当前优先启用以下 4 个子能力：

- `task-shaping`
- `delegation-contract`
- `verify-before-done`
- `checkpoint-recap`

原因：这 4 个最直接解决高频问题：

- 任务没定型就开干
- 子任务分派模糊
- 没验证就报完成
- 长任务中途断层

## 如何选择要读的 reference

- 任务一开始目标不够清晰，读 `references/task-shaping.md`
- 任务需要拆成多个可执行块，读 `references/plan-and-slice.md`
- 需要把任务分派给 coder / reviewer / writer / learner，读 `references/delegation-contract.md`
- 任何涉及实现、配置、系统变更、自动化落地、文档高风险编辑的任务，在对外汇报前读 `references/verify-before-done.md`
- 任务明显变长、已开团队、已出现卡点、需要续做时，读 `references/checkpoint-recap.md`
- 任务即将结束、需要对外收口时，读 `references/delivery-closeout.md`

## 推荐编排

### 工程任务
`task-shaping → delegation-contract → implementer → verify-before-done → reviewer → checkpoint-recap（按需）`

### 调研任务
`task-shaping → researcher`

### 长任务
`task-shaping → 执行 → checkpoint-recap（循环）`

### 高风险任务
`task-shaping → 风险确认 → delegation-contract → verify-before-done → reviewer`

## 与现有体系的关系

本 skill 不替代宿主环境原有的角色分工、记忆系统、项目规则或领域技能。

它只做一件事：把已经稳定成立的执行原则，转成在复杂任务里更容易触发、组合、落地的工作流。

## 注意事项

- 不要对所有任务机械套完整流程
- 能直接做完的小任务，不要强行放大
- 默认先读取最相关的一个 reference；确有需要再继续补读下一份
- 没验证，不按完成处理
- checkpoint 只收关键状态，不堆过程噪音
- 对外输出优先给结论，不把内部过程原样外发