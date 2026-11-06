# GAMES.GG MCP

![GAMES.GG](assets/games-gg-icon-256.png)

Connect your AI assistant to [GAMES.GG](https://games.gg) for game guides,
reviews, news, deals and release dates. Save games and guides to your account,
and follow redeem-code alerts. Available tools can vary by app and account.

**Server URL:** `https://mcp.games.gg/mcp`

Sign in with a free GAMES.GG account through OAuth when your app asks you to
connect. You do not need an API key. Account tools act on your own saved items
and code follows. Deals are not available in ChatGPT.

See the [setup guide](https://help.games.gg/en/articles/2048414-use-gamesgg-with-your-ai-assistant)
for account limits.

## Claude

1. Open **Customize → Connectors** and add a custom connector.
2. Set the name to **GAMES.GG** and the server URL to `https://mcp.games.gg/mcp`.
3. Connect and complete the GAMES.GG sign-in.

Custom connectors depend on your Claude plan and workspace settings.

## ChatGPT

1. Open **Settings → Apps → Advanced settings** and enable developer mode,
   if your plan and workspace allow it.
2. Create a custom app named **GAMES.GG** with the server URL
   `https://mcp.games.gg/mcp` and OAuth authentication.
3. Connect, sign in to GAMES.GG, then select the app in a chat.

## Claude Code

```sh
claude mcp add --transport http games-gg https://mcp.games.gg/mcp
```

Run `/mcp` in Claude Code and authenticate **games-gg**.

## Cursor

[Add to Cursor](https://cursor.com/en/install-mcp?name=games-gg&config=eyJ1cmwiOiJodHRwczovL21jcC5nYW1lcy5nZy9tY3AifQ%3D%3D)

Or add this entry to `~/.cursor/mcp.json`. Keep any existing servers:

```json
{
  "mcpServers": {
    "games-gg": {
      "url": "https://mcp.games.gg/mcp"
    }
  }
}
```

Open Cursor's MCP settings and connect **games-gg** to sign in.

## VS Code

Run **MCP: Add Server** from the Command Palette. Select **HTTP**, enter
`https://mcp.games.gg/mcp`, and name the server **games-gg**. Choose where to
save the configuration, start the server, and complete sign-in when prompted.

## Gemini CLI

```sh
gemini extensions install https://github.com/GAM3Sgg/games-gg-mcp
```

Restart Gemini CLI. Run `/mcp auth games-gg` to complete sign-in if needed.

## Cline

Open **MCP Servers → Remote Servers**. Use the name **games-gg**, the URL
`https://mcp.games.gg/mcp`, and **Streamable HTTP** as the transport.
Add the server and complete OAuth sign-in. Confirm that the tool list appears.

Agents can follow [llms-install.md](llms-install.md).

## Try it

- “Find a beginner guide for Elden Ring.”
- “What did GAMES.GG say about this game?”
- “Which games release this week?”
- “Save this game to my list.”
- “Follow redeem-code alerts for this game.”

## Help and policies

- [Setup help](https://help.games.gg/en/articles/2048414-use-gamesgg-with-your-ai-assistant)
- [Privacy policy](https://games.gg/privacy-policy/)
- [Terms of service](https://games.gg/terms-of-service/)
- [Support](https://help.games.gg)
- [MIT license](LICENSE)
