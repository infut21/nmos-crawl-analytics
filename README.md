# NMOS Crawl Analytics

Ask Claude about crawler activity on your NMOS.NET sites without leaving the chat.

This plugin connects Claude to the NMOS.NET remote MCP server so you can inspect AI and search bot visits, crawl volume, traffic overview, robots.txt scan status, and SSL health. Every tool is read-only: the plugin does not change site settings, tracking code, or billing.

## Use it

1. Install the plugin from the Claude directory, or load this folder locally for testing.
2. Connect the bundled NMOS connector and sign in with your NMOS.NET account (OAuth).
3. Ask Claude things like:
   - “List my NMOS sites and summarize crawls for the last 7 days.”
   - “Which AI crawlers hit my top site most this month?”
   - “Is robots.txt healthy, and when does SSL expire?”

## Data

Claude calls tools on `https://nmos.net/mcp` using your signed-in NMOS.NET account. The plugin stores nothing itself. See the [privacy policy](https://nmos.net/privacy) and [setup guide](https://nmos.net/setup).

## Requirements

- An NMOS.NET account with at least one site set up for crawl tracking
- A Claude plan that can install directory plugins / connectors

## Support

help@nmos.net
