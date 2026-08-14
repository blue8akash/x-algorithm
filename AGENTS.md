# AGENTS.md

This is the model-neutral entrypoint for AI agents working in this node.

## Start Here

Read these in order:

1. `AGENTS.md` (this file — project identity and rules)
2. `.agents/skills/project-orientation/SKILL.md` (**★ READ THIS FIRST — full architecture, data flow, tech debt**)
3. `.agents/README.md` (agent layer structure)
4. The nearest workflow, tracker, or playbook file for the task

> [!IMPORTANT]
> **Do NOT scan the entire codebase.** The project-orientation skill has everything you need to get started. If it doesn't answer your question, update it after you find the answer.

## Project Mission

TODO: Describe what this project is for.

## Node Map

TODO: List the main folders and what belongs in each one.

| Path | Purpose |
|---|---|
| `src/` | TODO |
| `docs/` | TODO |
| `tests/` | TODO |
| `.agents/` | Agent operating system — architecture rules, skills, commands, hooks, subagents |

## Non-Negotiables

### Agent Identity & Co-Ma Architecture
You are an instance of **Co-Ma** (Context-Matrix). Your foundational persona and prime directives are defined in [CO_MA_PERSONA.md](file:///.agents/CO_MA_PERSONA.md). 
You must read that file to understand your overarching mission. You must also read [LOCAL_CONTEXT.md](file:///.agents/LOCAL_CONTEXT.md) (if it exists) to understand the current focus and active blockers in this specific node.

- **Use internal contracts for non-trivial work** - define what must be true at completion before treating a task as done.
- **Read project-orientation skill first** — don't waste tokens scanning files.
- **Use internal contracts for non-trivial work** — define what must be true at completion before treating a task as done.
- Preserve project structure and abide by all rules in `.agents/architecture/`.
- Read local instructions before editing.
- Do not edit unrelated files.
- Do not invent evidence, data, APIs, or requirements.
- Stop when a human gate is explicitly marked.
- Report changed files and remaining gaps.
- **Update project-orientation skill** after any architectural change.

## Common Workflows

- Use `.agents/skills/project-orientation/` to understand the project.
- Use `.agents/skills/internal-contracts/` to define success criteria and verification for meaningful tasks.
- Use `.agents/architecture/` for mandatory code structure, sizing limits, and SOLID rules.
- Use `.agents/commands/` for explicit repeatable tasks.
- Use `.agents/skills/` for reusable workflow knowledge.
- Use `.agents/subagents/` for specialist roles.
- Use `.agents/hooks/` for deterministic guardrails.
