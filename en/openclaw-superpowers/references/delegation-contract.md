# delegation-contract

## Purpose

When work is delegated, provide the four critical pieces of information that turn a vague handoff into an executable contract.

## When to Read

Read this when the main agent delegates work to another role and the task is more than a tiny one-off assist.

Typical roles include:

- `implementer`
- `reviewer`
- `writer`
- `researcher`

If the host runtime uses different role names, apply the same logic anyway.

This can be relaxed for:

- Tiny supplemental lookups
- Extremely narrow one-action delegations
- Cases where the main agent has already made the boundaries extremely explicit

## The Four-Part Contract

Always make these clear:

- Goal
- Done-state
- Verification requirement
- Return format

## Template

```md
Goal:
Done-state:
Verification requirement:
Return format:
```

## Recommended Return Format

```md
- Completed:
- Verification evidence:
- Remaining risks / gaps:
- Recommended next step:
```

## Usage Principles

- You do not need to literally write four separate lines every time, but all four pieces must be present
- The implementer owns implementation, not final quality sign-off
- The reviewer owns validation, not the main implementation
- Writer and researcher roles also need explicit outputs and return format

## Common Mistakes

### Mistake 1: saying only “go do this”
Fix: at minimum, define the goal and done-state.

### Mistake 2: making the reviewer both implement and review
Fix: keep implementation and review separate.

### Mistake 3: forcing the main agent to re-interrogate the result afterward
Fix: define the return format before delegating.

## Result Standard

A good delegation contract lets the delegated agent start immediately without asking what to do, how to prove it, or how to report back.
