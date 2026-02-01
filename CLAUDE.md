# CLAUDE.md

## Project Overview
This repository is a sandbox for learning and experimenting with **Claude Code extensions**. It contains examples of Plugins and MCP Servers to demonstrate how to extend Claude's capabilities.

## Codebase Map
- **`my-first-plugin/`**: A sample Claude Code Plugin.
    - `skills/`: Contains custom skills (Markdown instructions).
    - `.claude-plugin/`: Manifest file defining the plugin.
- **`hello-world-mcp/`**: A Type-Script based Model Context Protocol (MCP) server.
    - `src/index.ts`: The server logic exposing tools.

## Development Workflow

### Running the Plugin
To start Claude with the local plugin enabled:
```bash
claude --plugin-dir ./my-first-plugin
```

### Building the MCP Server
To build the TypeScript MCP server:
```bash
cd hello-world-mcp
npm run build
```

## Useful Commands
- **New Plugin Creation**: `mkdir -p new-plugin/.claude-plugin && mkdir -p new-plugin/skills`
- **Verify Plugin**: `claude --plugin-dir ./new-plugin` then run `/help`
