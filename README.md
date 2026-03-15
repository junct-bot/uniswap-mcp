# Uniswap MCP Server

MCP server for Uniswap. Agent-ready API for Uniswap.

Hosted at [uniswap.mcp.junct.dev/mcp](https://uniswap.mcp.junct.dev/mcp). Free to use. No auth. No API key required.

Part of [Junct](https://junct.dev) — the agent-readiness layer for web3.

## Quick Start

Add to your MCP client config (Claude Desktop, Cursor, Windsurf):

```json
{
  "mcpServers": {
    "uniswap": {
      "url": "https://uniswap.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    }
  }
}
```

## About

This MCP server is **deterministically generated** from the Uniswap API specification. Every tool maps 1:1 to a real API endpoint — no hallucinated endpoints.

- **Protocol:** Uniswap
- **Endpoint:** `https://uniswap.mcp.junct.dev/mcp`
- **Transport:** Streamable HTTP
- **Auth:** None required
- **Documentation:** [uniswap.mcp.junct.dev/llms.txt](https://uniswap.mcp.junct.dev/llms.txt)

## Links

- [Junct Dashboard](https://junct.dev/servers/uniswap)
- [llms.txt](https://uniswap.mcp.junct.dev/llms.txt)
- [agents.md](https://uniswap.mcp.junct.dev/agents.md)
- [OpenAPI spec](https://uniswap.mcp.junct.dev/openapi.json)

Keywords: Uniswap, MCP server, DeFi, AI agent, agent-ready API, crypto tools, Model Context Protocol
