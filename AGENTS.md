# Documentation project instructions

## About this project

- This is the customer-facing documentation site for BuiltBlock, built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- The product source of truth is the BuiltBlock app and the Account API. Write what a customer sees or does
- For Mintlify components and configuration, install the Mintlify skill: `npx skills add https://mintlify.com/docs`

## Terminology

- The product name is BuiltBlock
- Desk is the home workspace. The sidebar controls are **New chat**, **Focus**, **Accounts**, **Create work**, and **Customer model**
- The account menu contains **MCP**, **API**, and **Settings**
- Sources customers connect: HubSpot, Gong, Granola, Gmail, Slack, and Google Calendar
- Clients customers connect: Claude, ChatGPT, and Cursor
- MCP tools are `ask`, `run_account`, and `intake`. `run_account` and `intake` are admin-only
- The public API is the Account API at `https://api.builtblock.com`

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise. One idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Do not use em dashes

## Content boundaries

Document the signed-in app, source connections, MCP, and the Account API.

Do not name internal vendors or infrastructure. That includes WorkOS, AuthKit, Nango, Firecrawl, Exa, Falkor, Jev, Vertex, Stripe, Cloud Run, and Postgres. Say "sign in to BuiltBlock", "API key", and "Billing" instead.

Do not document internal pipelines, evals, paused features, or service runbooks. The error code `no_tenant_map` is part of the API. Explain it as a key that is not linked to an organization.

If the app and an internal note disagree, document what the app does.
