# task-shaping

## Purpose

Compress a complex task into a clear, executable, and verifiable definition before work starts.

## When to Read

Read this when any of the following is true:

- The user's goal is still fuzzy
- The task is clearly multi-step
- The task involves implementation, configuration, automation, or project work and the scope is not yet tight
- Rework risk is high
- The user explicitly asks to plan, clarify, or think first

Usually skip this for:

- Tasks that are already fully clear
- One-step tasks
- Small edits with an obvious done-state

## Output Structure

Default structure:

- Goal
- Done-state
- Boundaries
- Risks / uncertainties
- Success criteria

## Minimum Requirement

Before execution starts, you should be able to answer:

1. What exactly are we doing?
2. What counts as done?
3. What is out of scope?
4. What still needs confirmation or carries risk?

## Template

```md
- Goal:
- Done-state:
- Boundaries:
- Risks / uncertainties:
- Success criteria:
```

## Usage Principles

- Do not force the full template onto tiny tasks
- If the task is already clear, only fill the missing parts
- You do not need all five fields every time; fill what matters
- The higher the complexity, the more explicit the done-state should be
- If boundaries are unclear, do not rush into heavy execution

## Common Mistakes

### Mistake 1: repeating the user's words without sharpening them
Fix: compress the request into an executable definition.

### Mistake 2: defining the action but not the done-state
Fix: make completion criteria explicit.

### Mistake 3: thinking while executing and letting scope drift
Fix: define boundaries first.

## Result Standard

After task-shaping, the agent should be able to move into execution cleanly instead of circling around scope confusion.
