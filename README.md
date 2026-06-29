# Ponytail · user-invoked

A user-invokable port of [DietrichGebert's ponytail](https://github.com/DietrichGebert/ponytail) — the lazy senior dev mode for AI agents.

## Why this exists

The original ponytail activates automatically on every coding task. That works great when you're writing code, but it also fires when you're planning, debugging, reviewing docs, or doing anything else — and the constant "write less code" nudges get in the way.

This version flips that: **the model never auto-invokes it**. You call it when you want it. Type `ponytail` in your agent when you're about to write code and need the lazy discipline. The rest of the time it stays out of your way.

No credit taken — all the credit goes to DietrichGebert for the original ladder, rules, and design. This is just a repackage with a different invocation model.

## Install

```bash
npx skills add pathanaawej0-dot/ponytail-skill
```

Then type `ponytail` (or `/ponytail`, `@ponytail`) in your agent whenever you're about to code and want the lazy ladder active.

## What it does

Stops the agent before writing code and climbs a 7-rung ladder:

1. Does this need to exist? (YAGNI)
2. Already in this codebase? Reuse it.
3. Stdlib does it? Use it.
4. Native platform feature covers it? Use it.
5. Already-installed dependency solves it? Use it.
6. Can it be one line? One line.
7. Only then: minimum code that works.

Lazy means efficient, not careless. Input validation, error handling, security, and accessibility are never simplified away.

## Levels

| Level | Invoke | What changes |
|-------|--------|-------------|
| **lite** | `ponytail lite` | Build what's asked, name the lazier alternative in one line. |
| **full** | `ponytail full` | Ladder enforced. Stdlib and native first. Shortest diff. **Default.** |
| **ultra** | `ponytail ultra` | YAGNI extremist. Deletion before addition. Challenge requirements. |

## Agent support

Any agent compatible with the [Agent Skills](https://agentskills.io) open standard — Claude Code, Codex CLI, Cursor, Windsurf, OpenCode, Gemini CLI, pi, Hermes, Cline, and more.

## Deactivate

Say "stop ponytail" or "normal mode" to revert to default behavior.

## License

MIT
