# Amazon Ads MCP Starter Kit — Manage Amazon Advertising with AI

> **This is a recipe repo.** The Synter MCP server itself lives at [Synter-Media-AI/mcp-server](https://github.com/Synter-Media-AI/mcp-server): create, launch, and optimize campaigns across 16 ad platforms, with one-click install in Cursor, Claude, ChatGPT, and VS Code. Issues, releases, and ⭐ go there.


[![MCP Compatible](https://img.shields.io/badge/MCP-compatible-blue)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform: Amazon Ads](https://img.shields.io/badge/Platform-Amazon%20Ads-FF9900)](https://advertising.amazon.com)

**Turn your AI agent into an Amazon advertising expert.** Open this repo in Amp, Cursor, or VS Code and manage Sponsored Products, Sponsored Brands, and Sponsored Display campaigns — optimize ACOS, discover high-converting keywords, and scale your Amazon business.

---

## Install

[![Add to Cursor](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.com/en/install-mcp?name=synter-ads&config=eyJ1cmwiOiJodHRwczovL21jcC5zeW50ZXJhaS5jb20ifQ==)
[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_Synter-0098FF?logo=visualstudiocode&logoColor=white)](https://insiders.vscode.dev/redirect/mcp/install?name=synter-ads&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fmcp.synterai.com%22%7D)

- **Cursor / VS Code:** click a button above, or open this repo — it ships `.cursor/mcp.json` and `.vscode/mcp.json`.
- **Claude Code:** this repo ships `.mcp.json`; or run:
  ```bash
  claude mcp add --transport http synter-ads https://mcp.synterai.com
  ```
- **Codex:**
  ```bash
  codex mcp add synter-ads --url https://mcp.synterai.com
  codex mcp login synter-ads
  ```
- **Claude Desktop:** copy `claude_desktop_config.json` into your Claude config directory (macOS: `~/Library/Application Support/Claude/`, Windows: `%APPDATA%\Claude\`) and replace the placeholder API key.

Your client opens Synter sign-in in the browser (OAuth). New here? Create an account at https://synterai.com/sign-up. Headless/CI fallback: send `X-Synter-Key` with a key from https://synterai.com/developer.

The MCP server itself: https://github.com/Synter-Media-AI/mcp-server

---

## Why Amazon Ads + AI?

Amazon is the world's largest product search engine. 63% of online product searches start on Amazon, not Google. When someone searches on Amazon, they're not researching — they're ready to buy. This makes Amazon Ads the highest-converting advertising platform for product sellers.

But Amazon's advertising platform is complex. Sponsored Products has auto, manual broad, manual phrase, and manual exact targeting — each with different bid strategies. ACOS (Advertising Cost of Sale) is the North Star metric, not ROAS. Negative keywords work differently than Google. And the Amazon algorithm rewards sales velocity, meaning advertising directly improves your organic ranking.

An AI agent makes managing this complexity manageable. It understands Amazon's bid mechanics, discovers profitable keywords from search term reports, and optimizes ACOS across hundreds of products.

**Best for:** Amazon sellers (FBA and FBM), ecommerce brands, private label products, agencies managing Amazon accounts.

---

## What You Can Do

| Capability | Example |
|-----------|---------|
| **Sponsored Products** | "Create an auto-targeting Sponsored Products campaign for my new kitchen blender" |
| **Keyword Discovery** | "Which search terms from auto campaigns should I move to manual exact?" |
| **ACOS Optimization** | "My ACOS is 35%. Help me get it under 25%" |
| **Sponsored Brands** | "Create a Sponsored Brand campaign with our headline and 3 top products" |
| **Sponsored Display** | "Set up product targeting to show ads on competitor product pages" |
| **Negative Keywords** | "Add irrelevant search terms as negatives across all campaigns" |
| **Bid Optimization** | "Lower bids on keywords with ACOS above 40%, raise on profitable keywords" |
| **Budget Allocation** | "I have $1,000/month. How should I distribute across my 5 products?" |
| **Performance Reports** | "Show me ACOS by product for the last 30 days" |
| **Competitor Targeting** | "Target my ads on competitor product detail pages" |
| **Dayparting** | "When do my products convert best? Should I adjust bid schedules?" |
| **Product Launch Ads** | "I'm launching a new product — what's the ad strategy for week 1?" |

---

## Example Conversations

### 1. The Auto-to-Manual Keyword Workflow

> **You:** I've been running auto-targeting Sponsored Products for 3 weeks. What's next?
>
> **Agent:** Perfect timing. Let me harvest your search term report...
>
> Found 847 search terms. Here's the breakdown:
>
> **Top 15 performers (move to manual exact):**
> | Search Term | Clicks | Sales | ACOS | Recommended Bid |
> |---|---|---|---|---|
> | stainless steel water bottle 32oz | 89 | $1,240 | 12.3% | $1.45 |
> | insulated water bottle with straw | 67 | $890 | 14.1% | $1.20 |
> | bpa free water bottle large | 54 | $720 | 15.8% | $1.10 |
> | thermos water bottle adult | 42 | $580 | 16.2% | $0.95 |
> | ... (11 more) |
>
> **127 terms to add as negatives:**
> - "cheap water bottle" (87 clicks, $0 sales — price shoppers)
> - "water bottle for kids" (43 clicks, $0 sales — wrong audience)
> - "water bottle holder" (31 clicks, $0 sales — accessory seekers)
>
> **Recommended structure:**
> 1. Create manual exact campaign with the 15 profitable terms
> 2. Create manual phrase campaign with the top 30 terms (catches long-tail variations)
> 3. Add the 127 waste terms as negatives on the auto campaign
> 4. Keep auto campaign running at lower budget ($15/day → $10/day) to discover new terms
>
> **You:** Do it. And lower auto campaign bids by 20%.
>
> **Agent:** Done. Created 2 new campaigns with 45 keywords. Added 127 negative keywords to auto campaign. Reduced auto bids by 20%. Expected impact: ACOS should drop from 22% to ~16% within 2 weeks.

### 2. ACOS Deep Dive and Optimization

> **You:** My ACOS is 35% but my profit margin is only 30%. I'm losing money on ads. Help.
>
> **Agent:** Let me pull the full picture. ACOS of 35% on a 30% margin means you're spending $1.17 in ads for every $1.00 in profit. We need to get below 25% ACOS to be profitable.
>
> **Immediate actions:**
>
> **1. Kill the money pits (saves ~$800/month):**
> | Keyword | Spend | Sales | ACOS |
> |---|---|---|---|
> | "water bottle amazon" | $340 | $120 | 283% |
> | "best water bottle 2026" | $210 | $90 | 233% |
> | "water bottles bulk" | $180 | $0 | ∞ |
>
> These 3 keywords alone burned $730 last month with terrible returns. Pausing immediately.
>
> **2. Double down on winners (redirects $500/month):**
> | Keyword | Spend | Sales | ACOS |
> |---|---|---|---|
> | "32 oz insulated bottle" | $120 | $890 | 13.5% |
> | "leak proof water bottle" | $95 | $640 | 14.8% |
>
> These are printing money. Increase bids by 25% to win more impressions.
>
> **3. The hidden metric — TACoS (Total Advertising Cost of Sale):**
> Your ACOS is 35%, but your TACoS (ad spend ÷ total revenue including organic) is only 11%. This means Amazon ads are boosting your organic ranking. Even "unprofitable" ads drive organic sales.
>
> Want me to recalculate with organic halo effect included?

### 3. Product Launch Strategy

> **You:** I'm launching a new product next week. What's the Amazon Ads strategy?
>
> **Agent:** Product launches on Amazon follow a specific playbook. The goal: maximize sales velocity in weeks 1-3 to build organic ranking.
>
> **Week 1: Maximum aggression ($50/day)**
> - Auto campaign at 2x normal bids (you're buying data and ranking)
> - Sponsored Brands headline ad with "NEW" messaging
> - Sponsored Display product targeting on top 5 competitors
> - Accept high ACOS (50-70%) — this is an investment in ranking
>
> **Week 2: Harvest and optimize ($40/day)**
> - Pull search term report from auto campaign
> - Create manual campaigns with winning terms
> - Add negative keywords for irrelevant terms
> - Reduce auto bids by 15%
>
> **Weeks 3-4: Optimize for profitability ($30/day)**
> - Pause keywords with ACOS > 50% and no organic ranking improvement
> - Scale keywords with ACOS < 25%
> - Introduce Sponsored Display retargeting for viewed-but-not-purchased
> - Target ACOS: 30% (still above breakeven, but building ranking)
>
> **Month 2+: Steady state ($20-25/day)**
> - Focus on profitable keywords only
> - Target ACOS: 20-25%
> - Your organic ranking should be carrying 60-70% of sales by now
>
> **Key principle:** Early spend is an investment in organic ranking. Amazon's A10 algorithm rewards sales velocity heavily. $500 in "unprofitable" ads in week 1 can earn $5,000/month in organic sales.

### 4. Sponsored Brands vs Sponsored Products

> **You:** Should I use Sponsored Brands or Sponsored Products?
>
> **Agent:** Both, but for different purposes. Let me compare your current performance:
>
> | Metric | Sponsored Products | Sponsored Brands |
> |---|---|---|
> | ACOS | 22% | 31% |
> | Click-through rate | 0.8% | 1.4% |
> | Conversion rate | 14% | 8% |
> | New-to-brand % | 42% | 71% |
>
> **Sponsored Products** are your profit driver — lower ACOS, higher conversion rate. People see your product ad, click, and buy. Use for proven keywords with high purchase intent.
>
> **Sponsored Brands** are your growth driver — they appear at the top of search results with your brand logo, headline, and 3 products. Higher CPC, lower conversion, but 71% of customers are *new to your brand*. This is how you acquire customers who've never heard of you.
>
> **My recommendation:** Run both. Allocate 70% of budget to Sponsored Products (profit), 30% to Sponsored Brands (growth). Review monthly — if Sponsored Brands brings in high-LTV repeat buyers, the higher initial ACOS is worth it.

### 5. Competitor Product Targeting

> **You:** Can I show my ads on competitor product pages?
>
> **Agent:** Yes — this is Sponsored Display product targeting, and it's one of Amazon's most powerful features.
>
> When someone is looking at your competitor's product page, your ad appears below the buy box with a message like "Compare similar items." The customer is already in buying mode — they're just deciding *which* product.
>
> **Strategy:**
> 1. Identify your top 10 competitors by searching your main keywords
> 2. Create a Sponsored Display campaign targeting their ASINs
> 3. Use competitive ad copy: highlight what makes your product different (not cheaper — better)
>
> **Current competitive targeting results:**
> | Competitor ASIN | Their Price | Your Price | Your ACOS | Steal Rate |
> |---|---|---|---|---|
> | B08XYZ1234 | $34.99 | $29.99 | 18% | 8.2% |
> | B09ABC5678 | $39.99 | $29.99 | 14% | 11.4% |
> | B07DEF9012 | $24.99 | $29.99 | 42% | 2.1% |
>
> You're winning customers from higher-priced competitors (8-11% steal rate) but losing against the cheaper option. Consider targeting only competitors priced higher than you.

---

## Amazon Ads Tips from the Pros

1. **Track ACOS, not ROAS.** Amazon uses ACOS (ad spend ÷ ad revenue). 20% ACOS = 5x ROAS. Your target ACOS should be below your profit margin.
2. **Auto campaigns are keyword research tools.** Run auto for 2-3 weeks, harvest the search term report, move winners to manual campaigns, negative out losers. Rinse and repeat.
3. **Organic ranking is the real prize.** Amazon's algorithm rewards sales velocity. Even ads with high ACOS boost your organic ranking, which drives free sales. Track TACoS (Total ACOS) alongside ACOS.
4. **Negative keywords work differently.** On Amazon, add specific ASINs as negative product targets, not just keyword phrases. Prevents your ads from showing on irrelevant product pages.
5. **Product pages convert, not ads.** Your ads can only do so much — if your product listing has poor images, no A+ content, or bad reviews, no amount of ad spend will fix it. Optimize your listing first.
6. **Sponsored Display retargeting is underused.** Target people who viewed your product but didn't buy. These shoppers are warm — a retargeting ad with a coupon closes 15-20% more sales.
7. **Budget minimum: $10/day per campaign.** Amazon needs enough daily budget to gather meaningful data. For competitive categories, $25-50/day per campaign is more realistic.

---

## FAQ

### Is there an MCP for Amazon Ads?
Yes — this repo. It pre-configures the Synter MCP server for Amazon Advertising management. Works with Amp, Cursor, VS Code, and Claude Desktop.

### Can AI optimize my Amazon ACOS?
Yes. The agent analyzes search term reports, identifies profitable and wasteful keywords, adjusts bids, and adds negative keywords — all aimed at reducing your ACOS to your target level.

### What's the difference between ACOS and ROAS?
ACOS = Ad Spend ÷ Ad Revenue (expressed as %). ROAS = Revenue ÷ Ad Spend (expressed as Nx). They're inverses: 20% ACOS = 5x ROAS, 25% ACOS = 4x ROAS. Amazon sellers traditionally use ACOS.

### Should I use auto or manual targeting?
Both. Start with auto-targeting to discover keywords, then create manual campaigns with proven winners. Keep auto running at lower budgets to continuously discover new terms.

### Can the agent manage Sponsored Brands and Sponsored Display?
Yes. The agent supports all three Amazon ad types: Sponsored Products, Sponsored Brands (including video), and Sponsored Display (including product and audience targeting).

### Does this work for Amazon international marketplaces?
Yes, if your Amazon Advertising account has access to international marketplaces (UK, DE, JP, etc.). Specify the marketplace when making requests.

---

## Related Repos

- [amazon-dsp-agent](https://github.com/Synter-Media-AI/amazon-dsp-agent) — Programmatic display beyond Amazon
- [shopify-agent](https://github.com/Synter-Media-AI/shopify-agent) — Sync Shopify products
- [google-ads-agent](https://github.com/Synter-Media-AI/google-ads-agent) — Drive external traffic to Amazon listings
- [cross-platform-ads-agent](https://github.com/Synter-Media-AI/cross-platform-ads-agent) — Multi-channel management
- [conversion-tracking-agent](https://github.com/Synter-Media-AI/conversion-tracking-agent) — Attribution setup
- [audience-sync-agent](https://github.com/Synter-Media-AI/audience-sync-agent) — Sync audiences across platforms

---

## License

MIT — see [LICENSE](LICENSE) for details.

Built by [Synter](https://synterai.com) · [Get API Key](https://synterai.com/developer) · [Documentation](https://synterai.com/docs)
