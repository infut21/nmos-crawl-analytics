# NMOS Crawl Analytics

Ask Claude or Cursor about crawler activity on your NMOS.NET sites without leaving the chat.

This plugin connects AI clients to the NMOS.NET remote MCP server so you can inspect AI and search bot visits, crawl volume, traffic overview, robots.txt scan status, and SSL health. Every tool is read-only: the plugin does not change site settings, tracking code, or billing.

## Clients

- **Claude** — `.claude-plugin/` + `.mcp.json` (directory plugin bundle)
- **Cursor** — `.cursor-plugin/` + `mcp.json` (marketplace / Agent Plugin)
- **Any MCP client** — `https://nmos.net/mcp` with OAuth

## Use it

1. Install from the Claude directory, Cursor marketplace, or load this folder locally.
2. Connect the bundled NMOS MCP server and sign in with your NMOS.NET account (OAuth).
3. Ask things like:
   - “List my NMOS sites and summarize crawls for the last 7 days.”
   - “Which AI crawlers hit my top site most this month?”
   - “Is robots.txt healthy, and when does SSL expire?”

### Cursor manual MCP

```json
{
  "mcpServers": {
    "nmos": {
      "url": "https://nmos.net/mcp"
    }
  }
}
```

## Data

Clients call tools on `https://nmos.net/mcp` using your signed-in NMOS.NET account. The plugin stores nothing itself. See the [privacy policy](https://nmos.net/privacy) and [setup guide](https://nmos.net/setup).

## Requirements

- An NMOS.NET account with at least one site set up for crawl tracking
- A Claude or Cursor plan that can install plugins / MCP servers

## Support

help@nmos.net
