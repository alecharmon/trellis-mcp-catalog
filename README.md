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

## Catalog contents

This registry currently publishes individual/base MCP server entries only.
Composite servers are intentionally not published because several OAuth-based
remote MCP providers behave better when connected standalone.

## Secrets

Do not commit secrets. Configure OAuth or prompted tokens in Obot.
