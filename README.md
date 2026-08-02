# 5ire

5ire (5ireChain) is a layer-1, EVM-compatible smart contract blockchain built on the Polkadot SDK (Substrate),
founded in 2021 and headquartered in Dubai with engineering in India. Its Sustainable Proof of Stake /
"Proof of 5ire" consensus weights validator selection and rewards by ESG performance, aligned to the UN
Sustainable Development Goals.

- Website: https://5ire.org/
- Docs: https://docs.5ire.org/
- Source: https://github.com/5ire-tech
- Blog: https://5ire.medium.com/
- Secondary market listing: https://forgeglobal.com/5ire_stock/

## Not to be confused with

This repo profiles **5ire / 5ireChain, the blockchain company**. It is **not** [5ire.app](https://5ire.app)
(`github.com/nanbingxyz/5ire`), an unrelated open-source cross-platform desktop AI assistant and MCP client that
shares the name. Do not merge artifacts from the two.

## API surface

5ire publishes **no OpenAPI, AsyncAPI, GraphQL, MCP server or A2A agent card.** The developer contract is the
Ethereum JSON-RPC 2.0 method set on the EVM machine, plus the Polkadot-SDK RPC set on the native chain:

| Network | Chain ID | RPC | Explorer |
|---|---|---|---|
| Mainnet | 995 | `https://rpc.5ire.network` | https://5irescan.io |
| Thunder testnet | 997 | `https://rpc.testnet.5ire.network` | https://testnet.5irescan.io |

Both endpoints are public and unauthenticated — there is no API key. Authority for state changes comes from the
transaction signature, not from a credential presented to the endpoint.

## Availability note — observed 2026-08-02

Every 5ire-operated production host (`5ire.org`, `docs.5ire.org`, `rpc.5ire.network`, `5irescan.io`,
`testnet.5irescan.io`, `explorer/staking/validator/nominator.5ire.network`) returned **Cloudflare HTTP 530
(origin error 1016)**, and `rpc.testnet.5ire.network` did not resolve in DNS. Domain registration, DNSSEC and TLS
certificates are intact, and the last Internet Archive 200 for `docs.5ire.org` is 2025-12-11 — so this reads as an
origin/hosting outage rather than a lapsed domain. Documentation content captured in this repo was verified against
Internet Archive snapshots; every probe and its status code is recorded in `lifecycle/5ire-lifecycle.yml`.

Third-party surfaces remain live: GitHub (`5ire-tech`, 10 repos), npm (`@5ire` scope), Docker Hub (`5irechain`),
Medium, Discord, X and Telegram.
