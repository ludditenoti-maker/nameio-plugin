# NameIO — AI Visibility & Ecommerce SEO Plugin + MCP

[![NameIO MCP connector](https://glama.ai/mcp/connectors/com.getnameio/nameio/badges/score.svg)](https://glama.ai/mcp/connectors/com.getnameio/nameio)

NameIO shows which shopping questions ChatGPT, Gemini, Google AI Overviews, and Perplexity answer with a competitor instead of your store, which websites they cite, how they describe your brand, and what to change on your pages.

Your AI assistant does the reasoning. NameIO supplies the live data and saves reviewable drafts.

- **Try the free zero-login store check (no account needed):** [app.getnameio.com/check](https://app.getnameio.com/check)
- **Website & docs:** [getnameio.com/docs/mcp](https://getnameio.com/docs/mcp)
- **Hosted MCP endpoint (Streamable HTTP, OAuth 2.1):** `https://app.getnameio.com/mcp`
- **Official MCP Registry:** `com.getnameio/nameio`

## Install

### Claude Code
```bash
claude mcp add --transport http nameio https://app.getnameio.com/mcp
```

### Agent Skills (Claude Code, Cursor, Codex, Windsurf)
```bash
npx skills add ludditenoti-maker/nameio-plugin
```

### Gemini CLI
```bash
gemini extensions install https://github.com/ludditenoti-maker/nameio-plugin
```

### Claude Web / Desktop, ChatGPT, and Cursor
See step-by-step setup (including one-click Cursor install) at [getnameio.com/docs/mcp](https://getnameio.com/docs/mcp).

## What you can do

- See which shopping questions ChatGPT, Gemini, and Google AI Overviews answer with a competitor instead of your store (Perplexity on Pro), and which sites their answers link to
- Read your AI funnel (awareness, consideration, conversion): how often AI names your store, your share of named brands, and your place among them
- Compare how AI answers describe your brand next to your competitors, check by check
- Pull a prioritized fix brief and save a reviewable page diff plus deterministic JSON-LD draft (agents only ever save drafts; publishing is always human)
- Check what your site, crawlers, product feeds, and UCP checkout profile give AI assistants to work with
- Run keyword research, backlink analysis, site audits, and read Google Search Console and Google Analytics 4 data

## Included skills (14)

- `read-your-funnel` — read your awareness/consideration/conversion AI funnel and pick the lowest step to fix first
- `fix-what-ai-says` — pull a prioritized fix brief and draft page fixes for losing prompts or failing site checks
- `answer-tone` — record structured sentiment reads with verbatim quotes from stored AI answers
- `ai-visibility-audit` — full ecommerce AI visibility audit across buying questions and cited sources
- `ai-prompt-research` — discover the shopping questions people ask AI in your niche
- `seo-project-setup` — configure store scope, competitors, and Search Console intake
- `seo-audit` — full technical site and search audit
- `seo-report` — generate a self-contained HTML report from live data
- `seo-coach` — guided workflows across search and AI visibility
- `keyword-research` — keyword discovery, metrics, and SERP checks
- `keyword-clustering` — group keywords by intent and map to pages
- `competitive-landscape` — map market leaders, themes, and gaps
- `competitor-analysis` — deep dive on a single rival's footprint
- `link-prospecting` — find link prospects and cited third-party sites

## What the plugin runs and sends

This plugin has no executable scripts, hooks, or shell commands. It contains 14 Markdown skills, editor manifests, and one remote MCP server URL (`https://app.getnameio.com/mcp`). When your assistant calls a NameIO tool, inputs go over HTTPS to `app.getnameio.com/mcp` using OAuth 2.1 (with a read-only consent option if you do not want write tools enabled). See our [Privacy Policy](https://getnameio.com/privacy).

## Support

[Help and support](https://getnameio.com/docs/mcp#help-and-support) or email `chris@getnameio.com`.

## What's not done

NameIO does not publish fixes straight to your store yet (you paste approved fixes yourself), and it does not track Claude's answers.

## License

MIT — see [LICENSE](./LICENSE) and [NOTICE.md](./NOTICE.md).
