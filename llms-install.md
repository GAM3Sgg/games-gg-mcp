# Connect to GAMES.GG MCP

Use the remote server at `https://mcp.games.gg/mcp` with Streamable HTTP.
No local server, build, package install or API key is needed.

## Cline

1. Open Cline's MCP Servers panel, then Remote Servers.
2. Set Server Name to `games-gg`, Server URL to
   `https://mcp.games.gg/mcp`, and Transport Type to Streamable HTTP.
3. Add the server. Let the user complete OAuth sign-in with their free
   GAMES.GG account in the app's authorization flow. Do not request their
   password or copy access tokens into configuration files.
4. Confirm that Cline shows the server's tools. Call `find_game` with
   `{"query":"Elden Ring"}` and check that it returns game results.

Do not enable automatic approval for account changes. Ask the user before
saving or removing games or guides, or changing redeem-code follows.

## Other apps

Follow [README.md](README.md) for Claude, ChatGPT, Claude Code, Cursor,
VS Code and Gemini CLI. Use the same remote URL and the app's OAuth flow.

If authentication fails, use the app's reconnect or authorize action.
For help, use https://help.games.gg/en/articles/2048414-use-gamesgg-with-your-ai-assistant
or https://help.games.gg.
