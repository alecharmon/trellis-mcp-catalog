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
- **Engineering Toolkit**: Sentry, Axiom, Vercel, PostHog, Linear.

Composite component entries intentionally use `toolOverrides: []`. In Obot, an
empty override list means all tools from that component server are enabled. Do
not replace this with an explicit `enabled: true` allowlist unless you want new
provider tools to be hidden until the catalog is updated.

Standalone/base servers do not define tool allowlists in the catalog, so their
server-provided tools are enabled by default. GitHub and BigQuery are intentionally
not published because this registry is OAuth-only and those integrations were
using PAT/service-account credentials.

## Secrets

Do not commit secrets. Configure OAuth or prompted tokens in Obot.
