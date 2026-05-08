# STFU-m

Project documentation for humans.

Mandatory agent instructions are in [AGENTS.md](./AGENTS.md).

## Agent Instruction Protocol

Enforces minimal-token, high-density reasoning across AI coding agents (GitHub Copilot, Claude Code) in VSCode projects.

### What It Does

- Forces agents to read mandatory behavioral rules before every task
- Suppresses default verbose output patterns (greetings, recaps, unsolicited suggestions)
- Standardizes compressed reasoning format (`[LOGIC]`) for multi-step tasks
- Separates user-facing language (match input) from internal logic summaries (English only)

### Files

| File | Purpose |
| -- | -- |
| `AGENTS.md` | Master protocol — mandatory rules, priority order, reasoning style |
| `CLAUDE.md` | Claude Code entry point → references `AGENTS.md` + memory section |
| `.github/copilot-instructions.md` | Copilot entry point → references `AGENTS.md` |
