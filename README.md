# zkMe

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

zkMe is a decentralized identity network delivering privacy-preserving compliance for Web3. Using zero-knowledge proofs, self-sovereign identity (SSI) wallets, DID methods and soulbound tokens, zkMe lets applications verify their users and businesses without ever handling raw personal data. Its product suite spans zkKYC (customer identity with sanction, age, citizenship, location and uniqueness/anti-Sybil proofs), zkKYB (business entity and UBO verification), zkOBS (open-banking proof of accredited investor and proof of address), and KYT (on-chain wallet-address and transaction risk screening). Verification runs client-side through embeddable JavaScript and mobile widgets; integrators then query outcomes through the zkMe Open API on agw.zk.me using an AppID + API key pair. zkMe also publishes zkTLS verifier SDKs, DID registry/resolver tooling and smart contracts through its zkMeLabs GitHub org.

**Areas:** Company · Web3 · Identity · KYC · KYB · Compliance · Zero Knowledge · Decentralized Identity · Anti-Sybil · Transaction Monitoring

## zkMe on APIs.io

Everything profiled for zkMe is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/zkme/](https://apis.io/providers/zkme/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [zkMe Auth API](https://apis.io/apis/zkme/zkme-auth-api/) — Access-token issuance for SDK integration
- [zkMe KYT API](https://apis.io/apis/zkme/zkme-kyt-api/) — Know-Your-Transaction wallet-address and transaction risk screening
- [zkMe zkKYB API](https://apis.io/apis/zkme/zkme-zkkyb-api/) — Business entity and UBO verification status
- [zkMe zkKYC API](https://apis.io/apis/zkme/zkme-zkkyc-api/) — Customer identity verification results and proofs
- [zkMe zkOBS API](https://apis.io/apis/zkme/zkme-zkobs-api/) — Open banking / accredited-investor (proof of accreditation)

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [zkme](https://apis.io/servers/zkme/zkme/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Zkme Agentic Access](https://apis.io/agentic-access/zkme/zkme-agentic-access/)

#### Collections (5)

Postman and Open Collection request collections.

- [zkMe Protocol Auth API](https://apis.io/collections/zkme/open-zkme-auth-api/)
- [zkMe Protocol Auth KYT API](https://apis.io/collections/zkme/open-zkme-kyt-api/)
- [zkMe Protocol Auth zkKYB API](https://apis.io/collections/zkme/open-zkme-zkkyb-api/)
- [zkMe Protocol Auth zkKYC API](https://apis.io/collections/zkme/open-zkme-zkkyc-api/)
- [zkMe Protocol Auth zkOBS API](https://apis.io/collections/zkme/open-zkme-zkobs-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Zkme Openapi Overlay](https://apis.io/overlays/zkme/zkme-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Zkme Authentication](https://apis.io/security/zkme/zkme-authentication/)
- [Zkme Domain Security](https://apis.io/security/zkme/zkme-domain-security/)
- [Zkme Vulnerability Disclosure](https://apis.io/security/zkme/zkme-vulnerability-disclosure/)

#### Rate limits (1)

Published request limits.

- [Zkme Rate Limits](https://apis.io/rate-limits/zkme/zkme-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://zk.me)
- [Documentation](https://docs.zk.me/hub/start/onboarding)
- [Getting started](https://docs.zk.me/hub/start/onboarding)
- [API reference](https://docs.zk.me/hub/start/onboarding/integration/api)
- [Sign up](https://dashboard.zk.me)
- [Support](https://docs.zk.me)
- [Security](https://docs.zk.me/hub/explore/bounty)
- [GitHub](https://github.com/zkMeLabs)

## API Evangelist rating

**Kin Score 31.2** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 11.9 |
| Contract governance | 4.5 |
| Operational transparency | 34.2 |
| Developer ergonomics | 63.7 |
| Access clarity | 0.0 |

**Agent readiness 24.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/zkme/](https://apis.io/providers/zkme/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for zkMe: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/zkme/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
