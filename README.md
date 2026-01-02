# MachinaOs Documentation

This folder contains the Mintlify documentation for MachinaOs.

## Setup

1. Create a new repository `trohitg/machinaos-docs` on GitHub
2. Copy the contents of this folder to the new repository
3. Connect the repository to Mintlify:
   - Go to [mintlify.com](https://mintlify.com)
   - Click "Get Started" and sign in with GitHub
   - Select your `machinaos-docs` repository
   - Mintlify will automatically deploy your docs

## Local Development

```bash
# Install Mintlify CLI
npm install -g mintlify

# Run local dev server
cd docs-mintlify
mintlify dev
```

The docs will be available at http://localhost:3000

## Structure

```
docs-mintlify/
├── docs.json           # Mintlify configuration
├── introduction.mdx    # Home page
├── installation.mdx    # Setup guide
├── quickstart.mdx      # Quick start tutorial
├── faq.mdx            # FAQ page
├── tutorials/         # Step-by-step guides
│   ├── first-workflow.mdx
│   ├── ai-agent-workflow.mdx
│   ├── whatsapp-automation.mdx
│   └── android-automation.mdx
├── nodes/             # Node documentation
│   ├── overview.mdx
│   ├── ai-models.mdx
│   ├── ai-agent.mdx
│   ├── whatsapp.mdx
│   ├── android.mdx
│   ├── webhooks.mdx
│   └── schedulers.mdx
├── deployment/        # Deployment guides
│   ├── docker.mdx
│   └── production.mdx
├── logo/              # Logo assets
│   ├── dark.svg
│   └── light.svg
├── images/            # Screenshots and diagrams
└── favicon.svg        # Browser favicon
```

## Adding Content

1. Create new `.mdx` files in the appropriate folder
2. Add frontmatter with title and description:
   ```mdx
   ---
   title: Page Title
   description: Brief description
   ---
   ```
3. Update `docs.json` navigation to include new pages
4. Commit and push - Mintlify auto-deploys

## Mintlify Components

Common components used in docs:

- `<Card>` - Feature cards with icons
- `<CardGroup>` - Grid layout for cards
- `<Tabs>` - Tabbed content
- `<Accordion>` - Collapsible sections
- `<Info>`, `<Warning>`, `<Tip>` - Callout boxes
- `<ParamField>` - Parameter documentation
- `<Check>` - Success checkmarks

See [Mintlify docs](https://mintlify.com/docs) for full component reference.
