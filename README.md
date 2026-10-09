# Labour Market Statistics MCP Server

Unemployment, employment, wages and earnings, labour costs and social protection from Eurostat, OECD, the ILO, the World Bank and national statistics offices.

Remote MCP server (Streamable HTTP), read-only, hosted by [Monitly](https://monit.ly).

```
https://monit.ly/api/mcp/labour
```

## Tools

| Tool | What it does |
|---|---|
| `search_catalog` | Find labour market datasets by topic, country and source. |
| `inspect_dataset` | Check country coverage, dimensions and the latest values. |
| `get_dataset` | Dataset metadata and period range. |
| `get_series` | Time series for one country. |

## Example prompts

- What is the unemployment rate in Spain?
- How have average wages in Poland changed since 2010?
- Compare youth unemployment across the EU.

## Authentication

No account or key is needed. A fair-use daily limit applies; for higher volumes use the keyed Monitly MCP at https://monit.ly/mcp-docs.

## Setup

**Claude (claude.ai, Desktop):** Settings → Connectors → Add custom connector → paste the URL above.

**Cursor / VS Code / Windsurf** (`mcp.json`):

```json
{
  "mcpServers": {
    "labour-market-statistics": {
      "url": "https://monit.ly/api/mcp/labour"
    }
  }
}
```

**ChatGPT:** Settings → Apps → Developer mode → Create → paste the URL.

## About

Part of the [Monitly](https://monit.ly/mcp-docs) MCP family. Full Monitly catalog (100,000+ datasets, all topics): https://monit.ly/api/mcp/public.

Questions: info@monit.ly

## Gemini CLI

```bash
gemini extensions install https://github.com/ContentWriterco/Labour-Market-Statistics-MCP
```

No account or key needed.

## Setup guides

Step-by-step setup guides for Claude, ChatGPT, Gemini, Grok, Le Chat, Perplexity, Cursor, VS Code and Claude Code: https://monit.ly/mcp/connect
