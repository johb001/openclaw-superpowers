---
name: openclaw-superpowers
description: Use when tasks are complex, multi-step, high-risk, require multiple agents, or need explicit validation before being reported as done. Adds a lightweight closed-loop workflow for shaping work, slicing plans, delegating clearly, verifying before completion, and checkpointing long tasks.
---

# OpenClaw Superpowers

A lightweight workflow layer for complex tasks: strengthen complex work without slowing simple work down.

## When to Use

Use this skill only when a task has real complexity or real risk. Common triggers:

- The task is clearly multi-step
- The task involves implementation, configuration, automation, or delivery work that cannot be safely treated as a one-step action
- The work is long-running and may need clean resumption later
- The task requires multiple agents or roles
- The task is high-risk
- The result must be explicitly verified before being reported as done

Usually do not trigger the full skill for:

- Simple Q&A
- Light suggestions
- One-step low-risk actions
- Casual chat
- Single low-risk information lookups
- Small edits that are already clear and need no extra verification

## Core Principles

- Shape before execution
- Verify before reporting completion
- Add checkpoints for long work
- Use explicit delegation contracts
- Process exists to protect outcomes, not to create friction

## Workflow Building Blocks

Use only the parts you need:

1. **task-shaping** — clarify goal, done-state, boundaries, and risks
2. **plan-and-slice** — break large work into manageable units
3. **delegation-contract** — delegate with explicit goal, done-state, verification, and return format
4. **verify-before-done** — validate before claiming completion
5. **checkpoint-recap** — summarize long-running work at meaningful stage boundaries
6. **delivery-closeout** — convert internal progress into a user-facing handoff

## How to choose a reference

- If the task is still fuzzy: read `references/task-shaping.md`
- If the task should be broken into executable chunks: read `references/plan-and-slice.md`
- If work is being delegated: read `references/delegation-contract.md`
- If the task changes external state or might be falsely reported as done: read `references/verify-before-done.md`
- If the task is getting long or needs a resumable state: read `references/checkpoint-recap.md`
- If the work is ready to be handed back to a user: read `references/delivery-closeout.md`

## Suggested compositions

### Engineering work
`task-shaping → delegation-contract → implementer → verify-before-done → reviewer → checkpoint-recap (as needed)`

### Research work
`task-shaping → researcher`

### Long-running work
`task-shaping → execution → checkpoint-recap (loop)`

### High-risk work
`task-shaping → risk check → delegation-contract → verify-before-done → reviewer`

## Relationship to host systems

This skill does not replace the host runtime's role system, memory layer, project rules, or domain-specific skills.

It only turns stable execution principles into a reusable workflow for complex work.

## Notes

- Do not force the full process onto simple tasks
- Do not over-read references; start with the single most relevant one
- Do not report unverified work as complete
- Keep checkpoints compact and useful
- Keep user-facing outputs cleaner than internal execution traces
