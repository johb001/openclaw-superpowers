# verify-before-done

## Purpose

Require a minimum real validation step before reporting work as complete.

## When to Read

Read this when the task involves any of the following:

- Code implementation
- Configuration changes
- Bug fixes
- High-risk document edits
- Automation delivery
- System operations
- External state changes

## Output Structure

- What changed
- How it was verified
- Verification result
- What remains unverified
- Whether it is safe to report as done

## Minimum Verification Requirement

At least one real validation step should happen. Depending on context, that may include:

- build / lint / test
- actual runtime behavior
- visible page output
- a real configuration call succeeding
- re-reading document structure after edits
- logs / return values / status checks

If the environment prevents full verification, you must still say:

- what layer has been verified
- what layer remains unverified
- why further verification is currently blocked

## Guardrail

Without verification, do not directly say:

- done
- fixed
- ready
- no problem
- shipped

Instead say something like:

- changed, but not yet verified
- minimally handled, pending verification
- confirmed only at the code/config layer, not yet in live effect

## Template

```md
- What changed:
- Verification method:
- Verification result:
- Unverified items:
- Safe to report as done:
```

## Usage Principles

- Prefer real-path verification over static inspection
- If full verification is impossible, be explicit about the verified layer
- Separate verified / likely / unverified in external reporting
- Do not present “theoretically correct” as “already complete”
- If there is no evidence, downgrade the claim

## Common Mistakes

### Mistake 1: treating code completion as task completion
Fix: add at least one runtime-level verification.

### Mistake 2: relying on intuition
Fix: speak from evidence, not confidence.

### Mistake 3: not checking the post-change state in high-risk edits
Fix: read back the resulting state.

## Result Standard

Before saying the work is done, there should be at least one minimal evidence chain supporting that claim.
