# example-react

Example React plugin with a bundled skill and remote MCP access (DeepWiki).

## Layout
- One manifest per client in its dot-folder (`.claude-plugin`, `.cursor-plugin`, `.codex-plugin`, `.github/plugin`, `.plugin`, `.grok-plugin`, `.kimi-plugin`, `.antigravity-plugin`), plus `gemini-extension.json`.
- MCP configs in `agents/<client>/` (Antigravity: `mcp_config.json`; Kimi and Gemini: inline).
- Shared `skills/`.

## MCP
Remote HTTP: `https://mcp.deepwiki.com/mcp`.

stdio alternative (not used here):
```json
{ "mcpServers": { "example-react": { "command": "npx", "args": ["-y", "some-mcp-server"] } } }
```
