# Trellis MCP Catalog

Public Obot MCP catalog for Trellis.

Add this Git source URL in Obot:

```text
https://github.com/alecharmon/trellis-mcp-catalog.git
```

`.obotcatalogs` restricts Obot sync to files named `*.mcp.yaml`.

## Layout

```text
mcp-catalog/base/        Individual MCP server catalog entries
mcp-catalog/composites/  Composite MCP server catalog entries
```

## Current composites

- **General**: Linear, Slack, Granola, Notion, Flora.
- **Engineering Toolkit**: Sentry, GitHub, Axiom, Vercel, PostHog, BigQuery, Linear.

## Secrets

Do not commit secrets. Configure OAuth or prompted tokens in Obot.
