# MachinaOs Documentation

Official documentation for [MachinaOS](https://github.com/trohitg/MachinaOS) - an open-source workflow automation platform with AI agents, React Flow, and n8n-inspired architecture.

**60 nodes** | **6 AI providers** | **Dracula theme**

## Live Docs

https://docs.zeenie.xyz/

## Local Development

```bash
# Install Mintlify CLI
npm install -g mintlify

# Run local dev server
mintlify dev
```

The docs will be available at http://localhost:3000

## Documentation Coverage

### Node Catalog (60 nodes)

| Category | Count | Page |
|----------|-------|------|
| AI Models | 6 | [ai-models.mdx](nodes/ai-models.mdx) |
| AI Agents | 3 | [ai-agent.mdx](nodes/ai-agent.mdx) |
| AI Skills | 10 | [skills.mdx](nodes/skills.mdx) |
| AI Tools | 4 | [tools.mdx](nodes/tools.mdx) |
| WhatsApp | 3 | [whatsapp.mdx](nodes/whatsapp.mdx) |
| Android | 17 | [android.mdx](nodes/android.mdx) |
| Documents | 6 | [documents.mdx](nodes/documents.mdx) |
| Webhooks | 5 | [webhooks.mdx](nodes/webhooks.mdx) |
| Location | 3 | [android.mdx](nodes/android.mdx) |
| Code | 2 | [schedulers.mdx](nodes/schedulers.mdx) |
| Workflow | 1 | - |

### AI Providers

- **OpenAI** - GPT-4o, GPT-4 Turbo, o1, o3, o4-mini
- **Anthropic** - Claude 3.5 Sonnet, Claude 3 Opus, Claude 3 Haiku
- **Google** - Gemini 2.5 Pro, Gemini 2.5 Flash, Gemini 2.0 Flash Thinking
- **OpenRouter** - 200+ models via unified API
- **Groq** - Llama, Mixtral, Qwen (ultra-fast)
- **Cerebras** - Llama, Qwen (ultra-fast)

## Structure

```
docs-MachinaOs/
├── docs.json           # Mintlify config (Dracula theme)
├── introduction.mdx    # Home page
├── installation.mdx    # Setup guide
├── quickstart.mdx      # Quick start tutorial
├── faq.mdx             # FAQ
├── tutorials/          # Step-by-step guides
│   ├── first-workflow.mdx
│   ├── ai-agent-workflow.mdx
│   ├── whatsapp-automation.mdx
│   └── android-automation.mdx
├── nodes/              # Node documentation
│   ├── overview.mdx    # All 60 nodes overview
│   ├── ai-models.mdx   # 6 AI providers
│   ├── ai-agent.mdx    # AI Agent, Chat Agent, Memory
│   ├── skills.mdx      # 10 skill nodes
│   ├── tools.mdx       # 4 tool nodes
│   ├── documents.mdx   # 6 RAG pipeline nodes
│   ├── whatsapp.mdx
│   ├── android.mdx
│   ├── webhooks.mdx
│   └── schedulers.mdx
├── deployment/
│   ├── docker.mdx
│   └── production.mdx
├── .github/workflows/  # Auto-deploy on push
└── logo/
```

## Theme

Using Dracula color palette:
- Primary: `#BD93F9` (purple)
- Light: `#FF79C6` (pink)
- Dark: `#6272A4` (comment)
- Background: `#282A36` (dark)
- Code blocks: Dracula syntax highlighting

## Contributing

1. Edit `.mdx` files
2. Test locally with `mintlify dev`
3. Commit and push - auto-deploys via GitHub Actions

## Mintlify Components

- `<Card>`, `<CardGroup>` - Feature cards
- `<Tabs>` - Tabbed content
- `<Accordion>` - Collapsible sections
- `<Info>`, `<Warning>`, `<Tip>` - Callouts
- `<ParamField>` - Parameter docs

See [Mintlify docs](https://mintlify.com/docs) for full reference.
