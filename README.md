# Memory Graph Visualizer

A browser-based visualizer for [MCP Memory Server](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) knowledge graph files (`.jsonl`).

## Features

- **JSONL View** — Syntax-highlighted raw data with color-coded keys, types, and values
- **Tree View** — Collapsible tree structure showing entities, their observations, and outgoing relations
- **Graph View** — Interactive D3.js force-directed graph with drag, zoom, and hover tooltips

Zero dependencies. Single HTML file. Just open in a browser.

## Usage

### Option 1: Just open the file

```bash
open index.html
```

Then click **"Open JSONL"** and select your `.memory.jsonl` file.

### Option 2: Local server (for auto-loading)

```bash
npm start
# Opens at http://localhost:3000
```

### Finding your memory file

The MCP Memory Server stores data in a `.jsonl` file. Its location depends on your setup:

- **Project-scoped** (recommended): Check your `.mcp.json` for the `MEMORY_FILE_PATH` env var
- **Global default**: `~/.npm/_npx/<hash>/node_modules/@modelcontextprotocol/server-memory/dist/memory.jsonl`

## Screenshot

Load a `.jsonl` file to see:
- Left panel: JSONL source (syntax highlighted) or Tree structure (collapsible)
- Right panel: Interactive knowledge graph (drag nodes, zoom, hover for details)
