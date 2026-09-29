# personal-agent

This fork is the live personal agent: Nuxt web chat + Eve runtime, with Slack, iMessage, GitHub, Linear, and user-approved long-term memory.

**Run:** `pnpm install && cp .env.example .env && pnpm db:migrate && pnpm dev` → http://localhost:3000  
**Required env:** `BETTER_AUTH_SECRET`, `BETTER_AUTH_URL`, `INTERNAL_API_SECRET`  
**Do not** start a second agent repo. Customize `shared/agent.ts` and `agent/lib/base-instructions.ts` here.

---

<img src="./public/banner.png" width="100%" alt="Personal Agent Template" />

# Personal Agent Template

[![CI](https://img.shields.io/github/actions/workflow/status/vercel-labs/personal-agent-template/ci.yml?branch=main&color=black)](https://github.com/vercel-labs/personal-agent-template/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/github/license/vercel-labs/personal-agent-template?color=black)](https://github.com/vercel-labs/personal-agent-template/blob/main/LICENSE)
[![Vercel](https://img.shields.io/badge/Vercel-black?logo=vercel&logoColor=white)](https://vercel.com)

**Template.** Fork it, customize it, and deploy your own personal agent.

Open source personal agent template. Web chat, Slack, iMessage, GitHub, Linear, and long-term memory — one codebase, durable sessions, user-approved memory saves.

See [AGENTS.md](./AGENTS.md) and [docs/](./docs/) for architecture, env, and customization. Upstream template: [vercel-labs/personal-agent-template](https://github.com/vercel-labs/personal-agent-template).
