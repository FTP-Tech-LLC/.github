# FTP Tech

Open-source tooling for **[x402](https://x402.org) on the [Canton Network](https://canton.network)** — pay-per-request payments in Canton Coin over plain HTTP, built under the Canton Network Development Fund.

We build and maintain the x402 facilitator, the payer (agent) and merchant SDKs, and the end-to-end reference stack.

## The x402-on-Canton suite

| Repo | What |
|---|---|
| [x402-canton-facilitator](https://github.com/FTP-Tech-LLC/x402-canton-facilitator) | Verify / settle facilitator — relays payer-signed transfers, sponsors gas |
| [x402-canton-agent](https://github.com/FTP-Tech-LLC/x402-canton-agent) | Payer-side SDK, self-custody wallet CLI, MCP server |
| [x402-canton-merchant](https://github.com/FTP-Tech-LLC/x402-canton-merchant) | Express / Next.js middleware to gate routes behind payment |
| [x402-canton-core](https://github.com/FTP-Tech-LLC/x402-canton-core) | Shared types + ledger primitives |
| [x402-canton-e2e](https://github.com/FTP-Tech-LLC/x402-canton-e2e) | End-to-end integration tests |

📖 **Docs:** https://ftp-tech.mintlify.site
🌐 **Facilitator:** https://facilitator.ftptech.xyz

All repositories are licensed under **Apache-2.0**. Contributions welcome — see each repo's `CONTRIBUTING` and `SECURITY` policy (defaults live in this `.github` repo).
