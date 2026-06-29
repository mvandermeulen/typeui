# TypeUI for Hermes Agent

TypeUI connects Hermes Agent to the hosted TypeUI MCP server so it can use project design skills, brand kits, UI prompts, and layout variations while building interfaces.

## Configure TypeUI MCP

Merge this server into your Hermes configuration at `~/.hermes/config.yaml`:

```yaml
mcp_servers:
  typeui:
    url: "https://mcp.typeui.sh"
    auth: oauth
```

This folder includes the same snippet in `config.yaml`.

After updating the file, start or reload Hermes Agent:

```bash
hermes chat
```

Then run this command inside Hermes Agent:

```text
/reload-mcp
```

If Hermes does not start the OAuth flow automatically, run:

```bash
hermes mcp login typeui
```

Sign in with TypeUI when Hermes asks you to authorize the connection.

## Links

- Website: https://www.typeui.sh
- Documentation: https://www.typeui.sh/docs
- Hermes setup guide: https://www.typeui.sh/docs/guides/hermes
- TypeUI MCP server: https://mcp.typeui.sh
- Privacy policy: https://www.typeui.sh/privacy
- Terms of service: https://www.typeui.sh/terms
