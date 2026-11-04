---
name: nmos-crawl-summary
description: Summarize NMOS.NET crawler activity, traffic, robots.txt, and SSL health. Use when the user mentions bot visits, AI crawlers, crawl stats, robots.txt, SSL expiry, or site health for their NMOS sites.
---

When the user asks about crawlers, bot visits, crawl budget, robots.txt, SSL, or site health on NMOS.NET:

1. Call the nmos connector's `list_sites` tool first if you do not already know the site id.
2. Prefer the site the user named; otherwise use the primary or first active site and say which one you used.
3. For recent activity, call `list_bot_visits` and/or `get_crawl_stats` with a sensible `days` window (default 7, max 90).
4. For traffic, call `get_traffic_overview`.
5. For policy and health, call `get_robots_status` and `get_site_health`.
6. Reply with a short summary: totals, top bots, any robots or SSL warnings. Do not dump raw JSON.
7. All tools are read-only. Do not claim you changed settings, tracking, or billing.

The remote MCP server is https://nmos.net/mcp. Users sign in with OAuth to their NMOS.NET account. Setup docs: https://nmos.net/setup. Privacy: https://nmos.net/privacy.
