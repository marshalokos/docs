# Documentation project instructions

## About this project

- **Product**: Solana Explorer — an open-source web app for browsing blocks, transactions, accounts, and programs on any Solana cluster
- **Source repo**: [`marshalokos/explorer`](https://github.com/marshalokos/explorer)
- **Stack**: Next.js, TypeScript, Webpack, pnpm
- **Docs stack**: [Mintlify](https://mintlify.com) — pages are MDX files with YAML frontmatter, config in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- **Explorer** — the app itself; not "the project" or "the site"
- **cluster** — a Solana network environment (Mainnet, Testnet, Devnet, or custom RPC); not "network" or "chain"
- **account** — a Solana on-chain account; not "wallet" unless it specifically holds SOL
- **program** — a Solana smart contract; not "contract"
- **`.sol` domain** — a Bonfida/SNS domain name; resolved via the inline `spl-name-service` utility
- **SPL Name Service** — the Solana Name Service protocol; the inline implementation lives at `app/utils/spl-name-service.ts`

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and inline code references
- Use `bash` code blocks for shell commands; always include `--legacy-peer-deps` when showing `npm install`
- Link to source files in `marshalokos/explorer` when referencing implementation details

## Content boundaries

- **Do document**: installation, local dev setup, cluster configuration, name service resolution, known build quirks (e.g. `--legacy-peer-deps`)
- **Do not document**: internal Mintlify platform features, Solana validator operation, wallet management
- Keep docs in sync with changes merged to `marshalokos/explorer` — especially `app/utils/`, `package.json`, and CI workflow changes
