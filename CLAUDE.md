# CLAUDE.md

## Project Overview
This repository is a sandbox for learning and experimenting with **Claude Code extensions**. It contains examples of Plugins and MCP Servers to demonstrate how to extend Claude's capabilities.

## Codebase Map
- **`hello-claude-plugin/`**: A sample Claude Code Plugin.
    - `skills/`: Contains custom skills (Markdown instructions).
        - `hello/SKILL.md`: A greeting skill.
        - `joke/SKILL.md`: A joke-telling skill.
    - `.claude-plugin/plugin.json`: Manifest file defining the plugin.

## Development Workflow

### Running the Plugin
To start Claude with the local plugin enabled:
```bash
claude --plugin-dir ./hello-claude-plugin
```

## Useful Commands
- **New Plugin Creation**: `mkdir -p new-plugin/.claude-plugin && mkdir -p new-plugin/skills`
- **Verify Plugin**: `claude --plugin-dir ./hello-claude-plugin` then run `/help`
