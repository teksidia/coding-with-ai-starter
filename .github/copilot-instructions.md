# Copilot Instructions

## Agentic Workflow

### 1. Directory Structure

```text
/docs
 ├── vision.md              # High-level "Why" and product goals
 ├── architecture.md        # Technical "Blueprints" (Data flow, Stack, Patterns)
 └── /cycles
      └── /YYYYMMDD         # Specific development sprint/session
           ├── /feature-name
           │    ├── requirements.md     # User stories and "What" needs to be built
           │    └── specification.md   # Technical "How" (The AI's coding contract)
```

### 2. Documentation Roles

- [Vision](../docs/vision.md) Non-technical "North Star." Defines the problem statement and core project values.
- [Architecture](../docs/architecture.md) The bridge between vision and code. Defines the data model, API patterns, and system constraints.

#### [Cycles](../docs/cycles/)

See the [README](../docs/cycles/README.md) for the workflow and conventions around cycles, requirements, specs, and session logs.

## Architecture

Before writing any code, read [`docs/architecture.md`](../docs/architecture.md) to understand the data model and stack.

## Build & Run

### Tests

### Linting & Formatting

## MCP Servers

- **Playwright** (`@playwright/mcp`) — configured in [`.mcp.json`](../.mcp.json). Use it to navigate the app, interact with UI elements, take screenshots, and run end-to-end flows directly from Copilot Chat.

## Key Conventions

> Update this section as conventions emerge in the codebase.

- **API base URL**: e.g. configured via environment variable (e.g., `VITE_API_URL` or `REACT_APP_API_URL`) — do not hardcode
