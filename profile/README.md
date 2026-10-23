# FTP Tech

Open-source tooling for **[x402](https://x402.org) on the [Canton Network](https://canton.network)**: pay-per-request payments in Canton Coin and CIP-56 tokens (USDCx, CBTC, USDXLR, cETH and others), over HTTP with the x402 `exact` scheme or from AI agents via MCP. Built under the Canton Development Fund.

We build and run the x402 facilitator, the payer (agent) and merchant SDKs, and the MCP servers.

**Status:** live on Canton MainNet. The Canton `exact` scheme is merged upstream in [x402-foundation/x402](https://github.com/x402-foundation/x402). Funded by [Canton Dev Fund PR #78](https://github.com/canton-foundation/canton-dev-fund/pull/78).

## Use it

| What | Where |
|---|---|
| Merchant middleware | `npm i @ftptech/x402-canton-express` or `npm i @ftptech/x402-canton-next` |
| Payer SDK (your own signer) | `npm i @ftptech/x402-canton-client` |
| Agent wallet and CLI | `npx @ftptech/canton-agent-wallet` |
| Local MCP server | `npx -y @ftptech/canton-x402-mcp --relay-url https://facilitator.ftptech.xyz` |
| Hosted MCP (Claude, ChatGPT, Perplexity) | https://pay.ftptech.xyz/mcp |
| Facilitator | https://facilitator.ftptech.xyz/supported |
| Docs | https://x402-docs.ftptech.xyz |
| Site | https://www.ftptech.xyz |

All packages are published under [@ftptech on npm](https://www.npmjs.com/org/ftptech). npm is the release channel.

## Repositories

The code repos are source snapshots of the released packages. They are synced periodically and can lag npm.

| Repo | What |
|---|---|
| [x402-canton-facilitator](https://github.com/FTP-Tech-LLC/x402-canton-facilitator) | Verify and settle facilitator: relays payer-signed transfers, pays the network fee |
| [x402-canton-agent](https://github.com/FTP-Tech-LLC/x402-canton-agent) | Payer SDK, self-custody wallet CLI, local MCP server |
| [x402-canton-merchant](https://github.com/FTP-Tech-LLC/x402-canton-merchant) | Express and Next.js middleware to gate routes behind payment |
| [x402-canton-core](https://github.com/FTP-Tech-LLC/x402-canton-core) | Shared types and ledger primitives |
| [x402-canton-docs](https://github.com/FTP-Tech-LLC/x402-canton-docs) | Source of the docs site |
| [x402-canton-e2e](https://github.com/FTP-Tech-LLC/x402-canton-e2e) | End-to-end MainNet payment test |
| [x402-canton-compatibility-matrix](https://github.com/FTP-Tech-LLC/x402-canton-compatibility-matrix) | Supported Canton, Splice and package versions |
| [x402-canton-maintenance-playbook](https://github.com/FTP-Tech-LLC/x402-canton-maintenance-playbook) | Maintenance scope and operator procedures |

The code repositories are licensed under **Apache-2.0**. Contributions welcome: see [CONTRIBUTING](https://github.com/FTP-Tech-LLC/.github/blob/main/CONTRIBUTING.md) and [SECURITY](https://github.com/FTP-Tech-LLC/.github/blob/main/SECURITY.md).
