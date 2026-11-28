# NameIO — AI Visibility (GEO/AEO) & SEO Plugin + Hosted MCP

[![NameIO MCP connector](https://glama.ai/mcp/connectors/com.getnameio/nameio/badges/score.svg)](https://glama.ai/mcp/connectors/com.getnameio/nameio)

**Connect your Claude, ChatGPT, Codex, or Cursor directly to live AI visibility, Search Console, GA4, keyword, backlink, and technical audit data — and draft reviewable page fixes.**

Built for **Shopify / ecommerce stores**, **lead-generation sites** (local services, B2B/SaaS, publishers), and the **independent SEO consultants** who audit them.

- **Free starter tier:** Includes **$1 in live data credits** (no credit card required) — [sign up free](https://app.getnameio.com/sign-up)
- **Zero-login instant check:** See which brands ChatGPT recommends in your niche — [app.getnameio.com/check](https://app.getnameio.com/check)
- **Self-serve Pro:** **$54/month** (or $499/year) with $15/month in usage credits included — no enterprise sales calls
- **Hosted MCP endpoint (Streamable HTTP, OAuth 2.1):** `https://app.getnameio.com/mcp`
- **Official MCP Registry:** `com.getnameio/nameio` · **Docs:** [getnameio.com/docs/mcp](https://getnameio.com/docs/mcp)

---

## 30-Second Quickstart

### 1. Connect the hosted MCP server

**Claude Code**
```bash
claude mcp add --transport http nameio https://app.getnameio.com/mcp
```

**Install all 15 Agent Skills (Claude Code, Cursor, Codex, Windsurf, Antigravity)**
```bash
npx skills add ludditenoti-maker/nameio-plugin
```

**Gemini CLI**
```bash
gemini extensions install https://github.com/ludditenoti-maker/nameio-plugin
```

**Claude Web / Desktop, ChatGPT, and Cursor (1-click install)**
See step-by-step setup at [getnameio.com/docs/mcp](https://getnameio.com/docs/mcp).

### 2. Paste your first prompt

Once OAuth connects (supports **read-only** or **read + draft** scopes), paste this into your assistant:

> *"Run `whoami`, check my site's AI crawler & structured-data readiness, and read my AI funnel to show which buyer questions ChatGPT and Gemini answer with a competitor instead of me — then pull my top fix brief."*

---

## What Your Assistant Can Do (78+ Live MCP Tools)

- **Track AI shopping & buyer answers:** See which prompts ChatGPT, Gemini, Google AI Overviews, and Perplexity (Pro) answer with a competitor instead of your brand, and which external URLs get cited.
- **Read your 3-stage AI funnel:** Awareness, consideration, and conversion presence, share, and placement with sample-size-gated counts — plus a 3-tier citation funnel (retrieved vs. cited vs. converting) for lead-gen sites.
- **Measure brand framing & sentiment:** Inspect verbatim competitor answers and record structured sentiment reads with quotes (`answer-tone`).
- **Draft reviewable page fixes:** Pull a prioritized fix brief (`get_fix_brief`) and save a page diff + deterministic JSON-LD draft (`propose_page_fix`). **Agents only ever save drafts; publishing is always human.**
- **Check AI crawler & checkout readiness:** Verify plain-HTML readability, AI crawler rules, product feeds, and UCP checkout profiles (`/.well-known/ucp`).
- **Full SEO stack in the same MCP:** Keyword research, SERP competitors, backlinks, technical site audits, Google Search Console, and Google Analytics 4.

---

## Included Skills (15)

- `read-your-funnel` — read your awareness/consideration/conversion AI funnel (and 3-tier citation funnel for lead-gen) and pick the lowest step first
- `fix-what-ai-says` — pull a prioritized fix brief and draft page fixes for losing prompts or failing site checks
- `citation-to-lead-audit` — join AI citation gaps, deep-page conversion checks, and GA4 key events into a Citation-to-Lead Roadmap
- `answer-tone` — record structured sentiment reads with verbatim quotes from stored AI answers
- `ai-visibility-audit` — full AI visibility audit across buyer questions and cited sources
- `ai-prompt-research` — discover the real questions people ask AI in your market
- `seo-project-setup` — configure store or lead-gen scope, competitors, and Search Console intake
- `seo-audit` — full technical site and search audit
- `seo-report` — generate a self-contained HTML report from live data
- `seo-coach` — guided workflows across search and AI visibility
- `keyword-research` — keyword discovery, metrics, and SERP checks
- `keyword-clustering` — group keywords by intent and map to pages
- `competitive-landscape` — map market leaders, themes, and gaps
- `competitor-analysis` — deep dive on a single rival's organic footprint
- `link-prospecting` — find link prospects and cited third-party sites

---

## Live Benchmark Data

We measured **576 live ChatGPT shopping answers across 64 ecommerce categories** (373 brands, 2,033 external citations):
- [2026 Ecommerce ChatGPT Visibility Study](https://getnameio.com/study/chatgpt-ecommerce-2026)
- [Interactive 3D AI Shelf](https://getnameio.com/play) (zero login — test which DTC brands ChatGPT actually names)
- [2026 Lead Gen & Publisher Study](https://getnameio.com/study/chatgpt-lead-gen-2026)

## Security & Privacy

This plugin has **no executable scripts, hooks, or shell commands** — only 15 Markdown skills, editor manifests, and one HTTPS OAuth 2.1 MCP URL (`https://app.getnameio.com/mcp`) with an optional read-only consent toggle. See our [Privacy Policy](https://getnameio.com/privacy).

## Support

[Help and support](https://getnameio.com/docs/mcp#help-and-support) or email `chris@getnameio.com`.

## License

MIT — see [LICENSE](./LICENSE) and [NOTICE.md](./NOTICE.md).
