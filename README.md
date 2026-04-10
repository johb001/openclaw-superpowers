# OpenClaw Superpowers

A lightweight skill family for complex-task execution in OpenClaw-style agent systems.

This project packages a reusable workflow layer for tasks that are multi-step, high-risk, long-running, or require explicit verification before being reported as done.

## What it does

It adds six reusable execution building blocks:

- task-shaping
- plan-and-slice
- delegation-contract
- verify-before-done
- checkpoint-recap
- delivery-closeout

The goal is simple:

> Strengthen complex work without slowing simple work down.

## Project structure

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

## Language versions

- Chinese version: `zh/openclaw-superpowers/`
- English version: `en/openclaw-superpowers/`

## Attribution

This project is adapted with inspiration from:

- https://github.com/obra/superpowers

See `ATTRIBUTION.md` for details.

## Notes

- This repository keeps the skill body lean and puts details into `references/`.
- The public version removes host-specific references and private workflow bindings.
- You can use it as-is, or adapt the wording and trigger thresholds to your own agent runtime.

## License

MIT
