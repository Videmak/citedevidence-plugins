# CitedEvidence plugins

The official [CitedEvidence](https://citedevidence.com) plugin for ChatGPT, Codex
and Claude. It connects your assistant to CitedEvidence Scholar (over 250 million
scholarly works) and to your CitedEvidence account. It also adds skills for
finding evidence, checking references, formatting citations, Deep Research and
manuscript review.

The plugin uses the CitedEvidence MCP server at `https://citedevidence.com/mcp`.
You sign in with your CitedEvidence account the first time it connects.

## Install

- **Claude (web, desktop, Cowork):** Customize → Plugins → Add marketplace → `Videmak/citedevidence-plugins`, then install CitedEvidence and connect it on the plugin's Connectors tab.
- **Claude Code:** `/plugin marketplace add Videmak/citedevidence-plugins`, then `/plugin install citedevidence@citedevidence`, then `/mcp` to sign in.
- **Codex CLI:** `codex plugin marketplace add Videmak/citedevidence-plugins`, then install CitedEvidence from the Plugins Directory.
- **ChatGPT desktop / Codex app:** Plugins → Add → Add a marketplace → `Videmak/citedevidence-plugins`, then install CitedEvidence.

Any other MCP client can connect directly to `https://citedevidence.com/mcp`
(Streamable HTTP, OAuth). No API key is needed.

## What's inside

```text
.agents/plugins/marketplace.json   ChatGPT / Codex marketplace
.claude-plugin/marketplace.json    Claude marketplace
plugins/citedevidence/             the plugin: manifests, MCP server, six skills, icons
listing/                           screenshots of the interactive results
```

## Privacy and support

- The plugin sends CitedEvidence only what each request needs: search terms, the references or text you ask it to check, format, research or review, and the papers you save.
- Disconnect at any time in CitedEvidence under Profile → Connected apps.
- Privacy policy: https://citedevidence.com/privacy · Terms: https://citedevidence.com/terms · Help: https://citedevidence.com/help · Setup guide: https://citedevidence.com/integrations/ai-assistants

Licensed under MIT (see `plugins/citedevidence/LICENSE`).
