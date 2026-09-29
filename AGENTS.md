# personal-agent (smokyjunk-design fork)

Durable personal AI assistant. Eve runtime + Nuxt web. This repo is the live fork of vercel-labs/personal-agent-template — edit here, not a second copy.

## Commands

| Command | Description |
|---------|-------------|
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start Nuxt + Eve |
| `pnpm build` | Production build |
| `pnpm typecheck` | TypeScript check |
| `pnpm db:generate` | Generate Drizzle migrations |
| `pnpm db:migrate` | Apply migrations |

## Structure

```
agent/          Eve agent (channels, tools, skills)
app/            Nuxt UI
server/         Nitro API, Drizzle, utils
shared/         Cross-layer types
docs/           Architecture, env, customization
```

## Rules

- Writes that change GitHub, Linear, or memory need durable user approval.
- Eve talks to Nuxt only through `/api/internal/*` with `Authorization: Bearer <INTERNAL_API_SECRET>`.
- Memory: one prose block per category in `shared/types/memory.ts`. Saves replace the whole block.
- Customize branding in `shared/agent.ts`, persona in `agent/lib/base-instructions.ts`, model in `agent/agent.ts`.
- Do not commit `.env`, secrets, or session tokens.

## Docs

- [Architecture](docs/ARCHITECTURE.md)
- [Environment](docs/ENVIRONMENT.md)
- [Customization](docs/CUSTOMIZATION.md)
- [README](README.md)
