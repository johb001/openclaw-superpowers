# delivery-closeout

## Purpose

Turn internal execution results into a user-facing summary that can be consumed without digging through process noise.

## When to Read

Read this when work is ending or a meaningful stage conclusion already exists.

Common cases:

- an engineering task finished a round
- research produced a usable conclusion
- long-running work needs a stage-level wrap-up
- multiple-agent outputs have returned and need to be collapsed into one answer

## Output Structure

- Current status
- Result
- Verified / unverified
- Whether a user decision is needed

## Template

```md
- Current status:
- Result:
- Verified / unverified:
- User decision needed:
```

## Usage Principles

- Give the conclusion first, then only the supporting detail the user needs
- Keep only process details that affect understanding or next decisions
- Separate verified and unverified clearly
- If a decision is needed, state it explicitly
- Do not paste internal notes, raw failure logs, or tool noise into the final user reply

## Common Mistakes

### Mistake 1: burying the conclusion in the middle
Fix: lead with the result.

### Mistake 2: mixing “done” with “verified”
Fix: separate execution from validation.

### Mistake 3: reporting as if finished when a user decision is still pending
Fix: state the exact decision point.

## Result Standard

After reading the closeout, the user should know the current state, the result, what is actually verified, and whether they need to decide anything next.
