# Helpifyr

**An AI-agent operating stack for small and medium businesses** — governed agents that do real business work (finance, HR, operations) on top of a proven open-source ERP core, with verifiable evidence for every action.

> 🚧 **Status:** Private development, preparing an open-source release. Contributions will use the **DCO** (Developer Certificate of Origin, `git commit -s`). Watch this page — the public developer hub is already live at **[docs.helpifyr.com/developers](https://docs.helpifyr.com/developers/)**.

## What makes it different

- **Evidence over claims.** Every agent action is issue-driven, reviewed by an independent actor, and closed only after a live readback of the running system — "merged" is never mistaken for "deployed".
- **Governed autonomy.** Agents work behind human-in-the-loop gates for anything irreversible (payments, filings, customer-visible output). A three-account review model with server-side branch protection makes the gates mechanical, not conventional.
- **Layered knowledge, not one big prompt.** Role knowledge, company knowledge, live business data and per-task context are separate, permissioned layers — served to agents through a read-only gateway with provenance on every fact.

## Repository map

| Area | Repositories | Role |
|---|---|---|
| **Governance & truth** | `helpifyr-fabric` | Contracts, gates, event modeling — the control plane every other repo answers to |
| **Agent runtime** | `jhf-warp`, `jhf-openclaw-env` | Agent supervision, goal envelopes, runtime environment materialization |
| **Identity & secrets** | `jhf-heddle`, `jhf-keystore` | OIDC identity, session attestation, secret references |
| **Knowledge & memory** | `jhf-bobbin`, `jhf-loom`, `jhf-reed` | Context graph (Graphiti/Neo4j + Mem0), document evidence, read-only context gateway |
| **Business core** | `jhf-spindle` | ERPNext/CRM bridge — invoices, approvals, settlement runs with fail-closed guards |
| **Orchestration** | `jhf-pattern`, `jhf-shuttle`, `jhf-weaver` | Work materialization, transport, release & distribution |
| **Surfaces** | `jhf-lantern`, `jhf-docs`, `jhf-web` | Operator UI (Plan Studio), developer hub, website |
| **Quality & safety** | `jhf-swatch`, `jhf-selvage`, `jhf-dobby`, `jhf-beam`, `jhf-weft` | Test programs, compliance review, trajectory evaluation, artifact certification |

Additional `helpifyr-boost-*` repositories package domain-specific agent capabilities ("Boosts") that plug into the core.

## Where to start

1. **[Developer Hub](https://docs.helpifyr.com/developers/)** — repository map, roadmap, glossary, golden path.
2. **Golden Path** — `jhf-weaver` ships a devcontainer-based local lab (`docs.helpifyr.com/developers/golden-path-weaver`).
3. **Website** — [helpifyr.com](https://helpifyr.com).

---

*Development happens on a self-hosted Gitea (source of truth); these GitHub repositories are the distribution mirror, refreshed nightly. Issues and PRs here are not yet monitored — the public contribution path opens with the open-source release.*
