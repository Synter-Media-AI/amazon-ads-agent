# 🛒 Amazon Ads Agent

Manage Amazon Sponsored Products, Brands, and Display with AI agents via MCP.

 `amazon-ads` `sponsored-products` `ecommerce` `mcp` `ai-agents`

---

## What is this?

Open this repo in **Amp**, **Cursor**, or **VS Code** and your AI agent can immediately manage Amazon Ads — no SDK to install, no dependencies. The [Synter MCP server](https://github.com/Synter-Media-AI/mcp-server) is already configured.

## Setup (30 seconds)

1. **Get a free API key** at [syntermedia.ai/developer](https://syntermedia.ai/developer)
2. **Set the key:**
   ```bash
   export SYNTER_API_KEY=syn_your_key_here
   ```
3. **Open this repo** in Amp, Cursor, or VS Code
4. **Start chatting** — the MCP tools are already available

### Claude Desktop

Copy `claude_desktop_config.json` into `~/Library/Application Support/Claude/claude_desktop_config.json` and replace the API key.

---

## Example Prompts


> List Sponsored Products campaigns

> Create a Sponsored Brands campaign

> Pull ACOS metrics for the last 7 days

> Add product targeting to an ad group

> Optimize bids for keywords with high ACOS


See the `prompts/` folder for more ready-to-use prompt templates.

---

## How it works

This repo contains MCP configuration files that connect your AI agent to [Synter](https://syntermedia.ai) — a platform that manages ad accounts across Google, Meta, LinkedIn, Reddit, TikTok, X, Microsoft, Amazon, and more.

Your agent gets access to 140+ tools for campaign management, performance analytics, creative generation, audience sync, and conversion tracking.

| File | Editor |
|------|--------|
| `.agents/mcp.json` | Amp |
| `.cursor/mcp.json` | Cursor |
| `.vscode/mcp.json` | VS Code |
| `claude_desktop_config.json` | Claude Desktop |

---

## Connect Your Ad Accounts

1. Go to [syntermedia.ai/credentials](https://syntermedia.ai/credentials)
2. Click "Connect" next to Amazon Ads
3. Complete the OAuth flow
4. Your agent can now manage your campaigns

---

## Resources

- [Synter MCP Server](https://github.com/Synter-Media-AI/mcp-server) — Open source
- [Documentation](https://syntermedia.ai/manual)
- [Get API Key](https://syntermedia.ai/developer)

---

---

## Other Starter Kits

| Platform | Repo |
|----------|------|
| Google Ads | [google-ads-agent](https://github.com/Synter-Media-AI/google-ads-agent) |
| Meta Ads | [meta-ads-agent](https://github.com/Synter-Media-AI/meta-ads-agent) |
| LinkedIn Ads | [linkedin-ads-agent](https://github.com/Synter-Media-AI/linkedin-ads-agent) |
| All Platforms | [cross-platform-ads-agent](https://github.com/Synter-Media-AI/cross-platform-ads-agent) |

[View all starter kits →](https://github.com/orgs/Synter-Media-AI/repositories)

## License

MIT
