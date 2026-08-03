# Tokay

Tokay is a platform as a service (PaaS) that makes it simple to get your code running in production. Paste files, upload a folder, connect GitHub, or push with Git. We detect what the application needs, show you how everything will run, and ask only for decisions that require your judgment. You don't need a Dockerfile, YAML, or a Tokay SDK.

Tokay adapts to your code so you can use the language, framework, and application design that fit the job, whether that means [Node.js, Bun, Python, Go, Ruby, Rust, PHP, or static HTML](https://tokay.io/docs/languages-and-stacks). Verified frameworks include Express, Next.js, SvelteKit, Astro, Django, FastAPI, Flask, Streamlit, Rails, Laravel, Gin, and Axum. Web apps, APIs, workers, scheduled jobs, and webhooks can all run the way you or your AI agent built them.

[Get started](https://tokay.io/getting-started) · [Tokay MCP](https://tokay.io/docs/platform-mcp) · [Examples](https://tokay.io/examples) · [Use cases](https://tokay.io/use-cases) · [Documentation](https://tokay.io/docs) · [Pricing](https://tokay.io/pricing)

## Let your agent handle deployment

You don't have to deploy the application yourself or babysit your agent while they do it. [Give a coding agent such as Claude Code or Codex their own Tokay identity](https://tokay.io/use-cases/let-an-ai-agent-deploy-safely) and ask them to put the application live. You can give them only the access they need, and we check it on every request. They can set secrets but cannot read them back, and every action is recorded under the appropriate identity.

With the [Tokay MCP server](https://tokay.io/docs/platform-mcp), your agent can handle the deployment from source code through setup and verification. They recover from failures on their own and ask for your judgment only when a decision requires it. The full deployment protocol at [app.tokay.io/llms.txt](https://app.tokay.io/llms.txt) also covers the public GraphQL API when an agent needs lower level control.

## Leave the infrastructure to us

Your application is always ready because it runs on a dedicated server that stays on. KVM isolates your server from other customers with the same type of virtualization boundary used by major cloud providers such as AWS. Your visitors never have to wait for your server to start. Background workers stay ready between events and WebSocket connections stay open. We also handle HTTPS and private networking for you.

If you want to keep an application private, you can [turn on access control](https://tokay.io/docs/who-can-open-your-app) and give the right people access without building or maintaining authentication. We enforce access rules before requests reach your code. You can leave [individual webhook endpoints public](https://tokay.io/docs/public-endpoints) for outside services if you want to.

Tokay manages the databases and storage behind your application so you don't have to. That includes [Postgres, MySQL, MongoDB, and Redis](https://tokay.io/docs/databases). We provide required system libraries, keep database connections private, and put credentials where the application expects them. The persistent filesystem keeps ordinary file access fast, so uploads, generated reports, and SQLite data work as expected.

Your application keeps running without constant attention. Tokay restarts crashed processes automatically and preserves the evidence when a deployment fails. Clear diagnoses show what needs attention so you can fix the application quickly.

You get predictable performance and cost because your services, databases, and files share reserved capacity. There is no server for you to configure or maintain.

## Deploy with zero downtime

Your application stays online while you ship changes. A new version receives traffic only after it passes health checks, so a failed release never replaces the version already serving your users. You can return to an earlier release with one click, and deleted resources are recoverable for 30 days.

When you need to change your database structure, you can [deploy database changes safely](https://tokay.io/use-cases/deploy-database-migrations-safely) without becoming a database expert. Tokay rehearses each migration and shows you the result before changing your live database. We evaluate the risk, ask for your approval when needed, and take a snapshot before every managed database migration runs in production.

## Start free

Launch your application for free on a machine that stays on. No credit card is required, and you get 2 vCPU, 2.5 GB RAM, and 20 GB storage. When you need more capacity, the Standard plan provides 4 vCPU, 8 GB RAM, and 60 GB storage for $20 per month. Larger dedicated machines support heavier production workloads well beyond the Standard plan.

[tokayio/tokay-examples](https://github.com/tokayio/tokay-examples) contains complete applications you or your AI agent can deploy. Start with the source, download a ZIP, or follow the guides at [tokay.io/examples](https://tokay.io/examples).

Questions? Email [hello@tokay.io](mailto:hello@tokay.io).
