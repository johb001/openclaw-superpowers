# plan-and-slice

## Purpose

Break a complex task into manageable units so it can be executed, delegated, verified, and resumed without turning into a blob.

## When to Read

Read this when any of the following is true:

- The task has more than two steps
- Multiple roles or agents are involved
- The work cannot reasonably finish in a single reply
- There is clear parallelization value
- Resume cost would be high if the task is interrupted

Usually skip this for:

- Tasks that already have only one or two actions
- Cases where splitting would make the work slower or less clear
- Moments where only one minimal validation action is needed first

## Output Structure

Each sub-task should include:

- Task name
- Owner
- Deliverable
- Verification action
- Completion criteria

## Template

```md
### Sub-task 1
- Owner:
- Deliverable:
- Verification action:
- Completion criteria:
```

## Usage Principles

- Slice only to the level where each unit is independently executable and verifiable
- Slicing exists to improve execution, not to look sophisticated
- Prefer serial flow when parallelism adds noise
- The resulting structure should make sequence and responsibility obvious
- If only one minimal next action is needed, do that first instead of writing a large plan

## Common Mistakes

### Mistake 1: slicing too coarsely
Fix: make each unit concrete enough to execute and verify.

### Mistake 2: slicing too finely
Fix: keep only the layers that materially help execution, coordination, or validation.

### Mistake 3: listing steps without ownership or completion criteria
Fix: define who owns it and what counts as done.

## Result Standard

After slicing, each unit should be independently executable, independently verifiable, and easy to route back upstream.
