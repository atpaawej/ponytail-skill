# Ponytail

Makes your AI agent think like a lazy senior dev. The best code is the code you never wrote.

## Install

```bash
npx skills add atpaawej/ponytail-skill
```

Then type `ponytail` (or `/ponytail`, `@ponytail`) in your agent to activate lazy mode.

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
