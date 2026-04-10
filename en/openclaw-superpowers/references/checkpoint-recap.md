# checkpoint-recap

## Purpose

Capture a compact stage summary during long-running work so the task can resume cleanly and avoid drift.

## When to Read

Read this when any of the following is true:

- The work is taking a while
- The task is clearly multi-stage
- A team or multiple agents are already involved
- The task is blocked midstream
- The user changed topics and may return later
- The context has become long enough that clean resumption matters

## Output Structure

- Current goal
- Completed so far
- Current blocker
- Next step

## Template

```md
- Current goal:
- Completed so far:
- Current blocker:
- Next step:
```

## Usage Principles

- Capture only key state, not the full play-by-play
- Do not write a checkpoint every round; write one when stage boundaries actually change
- Write it so a future you or a different agent can resume quickly
- State blockers as operational constraints, not emotions
- Make the next step concrete and executable

## When a Checkpoint is Especially Useful

1. A stage just ended and another is about to begin
2. The task is blocked and will not be resolved immediately
3. Work must continue across replies or sessions
4. Multiple delegated results need to be collapsed back into one state summary
5. The task may need to be resumed after topic switching

## Common Mistakes

### Mistake 1: writing a running diary
Fix: keep only goal / completed / blocker / next step.

### Mistake 2: listing activity but not the actual blocker
Fix: make the current constraint explicit.

### Mistake 3: writing a vague next step
Fix: make the next action directly executable.

## Result Standard

After interruption, the task should be resumable from the checkpoint without re-reading a large message history.
