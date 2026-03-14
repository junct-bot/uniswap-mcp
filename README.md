# Uniswap MCP Server

Hosted MCP server for **Uniswap** — giving AI agents direct access to Uniswap dex data and operations.

> Powered by [Junct](https://junct.dev) — the agent-readiness layer for DeFi.

## Quick Connect

Add to your MCP client config (Claude Desktop, Cursor, Windsurf, etc.):

```json
{
  "mcpServers": {
    "uniswap": {
      "url": "https://uniswap.mcp.junct.dev/mcp"
    }
  }
}
```

**No setup required** — the server is hosted and maintained by Junct.

## Endpoint

| | |
|---|---|
| MCP URL | `https://uniswap.mcp.junct.dev/mcp` |
| Transport | Streamable HTTP |
| Domain | dex |
| Tools | 17 |
| Docs | [llms.txt](https://uniswap.mcp.junct.dev/llms.txt) |
| OpenAPI | [openapi.json](https://uniswap.mcp.junct.dev/openapi.json) |

## Tools (17)

| Tool | Description |
|---|---|
| `WETH9` | Calls WETH9(). Read-only — does not modify contract state. Unrestricted — any address can call this read function. Retur |
| `exactInput` | Calls exactInput(params: { path: string, recipient: string, deadline: string, amountIn: string, amountOutMinimum: string |
| `exactInputSingle` | Calls exactInputSingle(params: { tokenIn: string, tokenOut: string, fee: string, recipient: string, deadline: string, am |
| `exactOutput` | Calls exactOutput(params: { path: string, recipient: string, deadline: string, amountOut: string, amountInMaximum: strin |
| `exactOutputSingle` | Calls exactOutputSingle(params: { tokenIn: string, tokenOut: string, fee: string, recipient: string, deadline: string, a |
| `factory` | Calls factory(). Read-only — does not modify contract state. Unrestricted — any address can call this read function. Ret |
| `multicall` | Calls multicall(data: string[]). Requires ETH value to be sent with the transaction. Write function — may have access co |
| `refundETH` | Calls refundETH(). Requires ETH value to be sent with the transaction. Write function — may have access control restrict |
| `selfPermit` | Calls selfPermit(token: string, value: string, deadline: string, v: string, r: string, s: string). Requires ETH value to |
| `selfPermitAllowed` | Calls selfPermitAllowed(token: string, nonce: string, expiry: string, v: string, r: string, s: string). Requires ETH val |
| `selfPermitAllowedIfNecessary` | Calls selfPermitAllowedIfNecessary(token: string, nonce: string, expiry: string, v: string, r: string, s: string). Requi |
| `selfPermitIfNecessary` | Calls selfPermitIfNecessary(token: string, value: string, deadline: string, v: string, r: string, s: string). Requires E |
| `sweepToken` | Calls sweepToken(token: string, amountMinimum: string, recipient: string). Requires ETH value to be sent with the transa |
| `sweepTokenWithFee` | Calls sweepTokenWithFee(token: string, amountMinimum: string, recipient: string, feeBips: string, feeRecipient: string). |
| `uniswapV3SwapCallback` | Calls uniswapV3SwapCallback(amount0Delta: string, amount1Delta: string, _data: string). Write function — may have access |
| `unwrapWETH9` | Calls unwrapWETH9(amountMinimum: string, recipient: string). Requires ETH value to be sent with the transaction. Write f |
| `unwrapWETH9WithFee` | Calls unwrapWETH9WithFee(amountMinimum: string, recipient: string, feeBips: string, feeRecipient: string). Requires ETH  |

## Links

- [Junct Dashboard](https://junct.dev/servers/uniswap)
- [Server Info](https://uniswap.mcp.junct.dev/)
- [llms.txt](https://uniswap.mcp.junct.dev/llms.txt)
- [agents.md](https://uniswap.mcp.junct.dev/agents.md)
- [MCP Discovery](https://uniswap.mcp.junct.dev/.well-known/mcp/server.json)

---

*This server is automatically generated, hosted, and maintained by [Junct](https://junct.dev).*
