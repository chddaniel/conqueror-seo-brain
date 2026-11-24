# Conqueror SEO + AI Citations Brain

A free, read-only remote MCP server that gives AI agents step-by-step SEO and AI citation (AEO/GEO) playbooks, audit checklists, copy-paste templates and a weekly plan. Use it to rank on Google and get named by ChatGPT, Perplexity, Gemini, Claude, Grok Bot and Google AI Overviews.

- Landing page: https://brain.conquerorapp.com
- MCP endpoint (streamable HTTP): https://brain.conquerorapp.com/mcp
- Sign-in: OAuth 2.1 with PKCE. Enter your email and a 6 digit code. No API key.
- Price: free. Built by [Conqueror](https://conquerorapp.com).

## What you get

34 playbooks, 15 audit checklists (technical, on-page, local, product pages, AI citation readiness, plus WordPress, Shopify, Webflow, Framer, Wix and Squarespace), 17 templates (page outlines, schema JSON-LD, robots.txt for AI crawlers, llms.txt, outreach emails) and 7 read-only tools.

## Tools

| Tool | What it does |
| --- | --- |
| `situation_playbook` | Describe the business and the problem. Returns a diagnosis, the first 3 moves and the playbooks, checklists and templates to use, in order. |
| `weekly_plan` | Give a goal and the hours you have. Returns the tasks for this week with time estimates and steps, plus the next 3 weeks. |
| `search_brain` | Plain-words search across every playbook, checklist and template, with source links. |
| `get_playbook` | Full text of any playbook. |
| `get_checklist` | Audit checklists to run on your site. |
| `get_template` | Page outlines, schema snippets, robots.txt, llms.txt, outreach emails, agent prompts. |
| `list_sources` | Lists everything in the Brain. |

Prompts: `seo_ai_audit`, `this_week`, `ai_visibility_baseline`, `write_comparison_page`.

## Connect

Claude Code:

```
claude mcp add --transport http --scope user conqueror-brain https://brain.conquerorapp.com/mcp
```

Cursor, VS Code, Codex, Gemini CLI, Claude, ChatGPT and Grok Bot: add the URL https://brain.conquerorapp.com/mcp as a remote MCP server and sign in. Setup for each is on https://brain.conquerorapp.com.

Generic `mcp.json`:

```json
{
  "mcpServers": {
    "conqueror-brain": {
      "url": "https://brain.conquerorapp.com/mcp"
    }
  }
}
```

## Limits

60 calls a minute per account, 300 a minute per IP. Tokens last 1 hour and refresh on their own.

## Related

Conqueror's own MCP server (https://winwith.conquerorapp.com/mcp) does the work on your site: keyword data, AI visibility tracking and pages published after your approval.
