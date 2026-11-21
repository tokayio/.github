# Tokay

**Bring working code. We'll get it running and keep it that way.**

Tokay is a platform as a service (PaaS) that takes working code, written by you or your AI agent, and runs it in production. Whether you've built a web app, API, scheduled job, webhook, or background worker, Tokay handles the hosting, managed databases, and ongoing upkeep, with no deployment config to write.

Ask your AI assistant to deploy your code, or connect GitHub, paste or upload your files, or push with Git. Tokay works out what your app needs, shows you how everything will run, and asks only for the decisions it can't make safely. No Dockerfile, YAML, or Tokay SDK needed.

[Get started](https://tokay.io/getting-started) · [Use your AI assistant](https://tokay.io/getting-started/use-your-ai-assistant) · [Examples](https://tokay.io/examples) · [Use cases](https://tokay.io/use-cases) · [Docs](https://tokay.io/docs) · [Pricing](https://tokay.io/pricing)

## Bring the stack you already use

Build with the tools you like. Tokay works with what you already have.

- **Languages.** [Node.js, Bun, Python, Go, Ruby, Rust, PHP, Bash, and static HTML](https://tokay.io/docs/languages-and-stacks).
- **Frameworks.** Tested end to end, including Express, Next.js, NestJS, SvelteKit, Astro, Django, FastAPI, Flask, Streamlit, Rails, Laravel, Symfony, Gin, Fiber, and Axum.
- **Static sites.** Built with Hugo, Astro, Eleventy, Docusaurus, or VitePress, and served with HTTPS like any other app.

## Deploy from Claude, ChatGPT, Codex, or Cursor

Take your application from code to production without leaving your AI assistant. Connect [Tokay MCP](https://tokay.io/docs/platform-mcp), the official MCP server at `https://mcp.tokay.io/mcp`, and ask for a deployment. Your assistant can also read logs, query your databases without changing them, roll back releases, and troubleshoot failures. Decisions that need you still come to you.

Your assistant gets its own Tokay identity, and you stay in control. [Choose exactly what it can access](https://tokay.io/use-cases/let-an-ai-agent-deploy-safely). Tokay checks permissions on every request, lets your assistant set secrets without reading them back, and records every action under the identity that performed it.

- **tokay-deploy.** A Claude Code plugin, and a skill for Codex, Cursor, and other agents, that tells your agent when Tokay fits and how to connect. [tokayio/tokay-deploy](https://github.com/tokayio/tokay-deploy)
- **Tokay API.** A public GraphQL API at `https://api.tokay.io/graphql` for scripts and CI, the same one our web interface uses. [Tokay API docs](https://tokay.io/docs/api)
- **Agent instructions.** The full deploy sequence, with every query, mutation, and recovery step. [app.tokay.io/llms.txt](https://app.tokay.io/llms.txt)

## Your own virtual machine that stays on

Each workspace runs on its own virtual machine, isolated using KVM, the same virtualization technology used by major cloud providers. Your apps stay on, so visitors get a response right away, background workers stay ready between events, and WebSocket connections stay open. Every app gets HTTPS, and your services reach each other over a private network.

Your workspace's memory is reserved for you, so performance stays predictable. There's no server for you to configure, patch, or maintain.

## Private apps, public webhooks

Not every app should be public. [Turn on access control](https://tokay.io/docs/who-can-open-your-app) and choose who can open your app. Tokay handles sign-in and checks access before a request reaches your code, so there's no authentication for you to build or maintain. When an outside service needs to call a webhook, you can [keep that one endpoint public](https://tokay.io/docs/public-endpoints) and the rest of the app private.

## Managed databases and files

Tokay runs [Postgres, MySQL, MongoDB, and Redis](https://tokay.io/docs/databases) for you. Database connections stay private, and credentials are available where your application expects them. Need to generate PDFs, process images, or run a headless browser? Tokay includes the system libraries you need. Files persist like they would on any disk, so uploads and SQLite databases work as you'd expect. Your data is [backed up offsite every day](https://tokay.io/docs/persistent-storage).

## Zero downtime deploys and rollback

New releases go live only after passing health checks. Your users stay on the previous version until the replacement is ready, so deployments don't interrupt a running application. Crashed apps restart automatically. When a deployment fails, Tokay keeps the evidence and explains what went wrong and how to fix it. Need to go back? Roll back to an earlier release in one click. Anything you delete can be recovered for 30 days.

Database changes get the same care. [Migrations are rehearsed](https://tokay.io/use-cases/deploy-database-migrations-safely) before they touch live data, so you see the result first. Risky changes require your approval, and Tokay takes a snapshot of the managed database before the migration runs.

## Start free

Every account includes a Free workspace with 2 vCPU, 2.5 GB RAM, and 20 GB storage, and no credit card is required. One workspace, one predictable price. Run multiple applications without paying extra for each one. When you need more, a Small workspace is $30 a month for 4 vCPU, 8 GB RAM, and 60 GB storage, and [larger sizes](https://tokay.io/pricing) go well beyond that.

[tokayio/tokay-examples](https://github.com/tokayio/tokay-examples) has complete apps you can deploy yourself or hand to your AI assistant. Start from the source, download a ZIP, or follow a guide at [tokay.io/examples](https://tokay.io/examples).

Questions? Email [hello@tokay.io](mailto:hello@tokay.io).
