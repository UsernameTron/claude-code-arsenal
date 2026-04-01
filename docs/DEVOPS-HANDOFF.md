# DevOps Handoff — Claude Code Arsenal

## Project Summary

Claude Code Arsenal is a production-ready plugin for Claude Code providing battle-tested agents, skills, hooks, commands, rules, and MCP configurations for AI-assisted software development.

## Environment Requirements

- **Node.js**: >=18 (no transpilation required)
- **Platform**: macOS, Linux, Windows (cross-platform via Node.js scripts)
- **Claude Code**: Latest stable release

## How to Run

```bash
# Install the plugin
# Follow installation instructions in README.md

# Run tests
node tests/run-all.js

# Lint markdown files
npx markdownlint-cli '**/*.md' --ignore node_modules
```

## Configuration Reference

- `CLAUDE_PACKAGE_MANAGER` — Override package manager detection (npm, pnpm, yarn, bun)
- `ECC_HOOK_PROFILE` — Hook profile gating
- `ECC_DISABLED_HOOKS` — Comma-separated list of hooks to disable at runtime

## Security Notes

- No secrets or credentials are stored in this repository
- Hook scripts run with user-level permissions — review before enabling
- All hook scripts exit 0 on non-critical errors to avoid blocking tool execution

## Deployment Maturity

Production-ready. Used as a Claude Code plugin installation.

## Known Tech Debt

- None currently tracked
