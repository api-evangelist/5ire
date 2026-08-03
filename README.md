# 5ire

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
