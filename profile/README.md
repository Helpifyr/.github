<p align="center"><img src="assets/jadda-helpifyr.webp" alt="Jadda Helpifyr" width="200"></p>

# Helpifyr

**An AI-agent operating stack for small and medium businesses** — governed agents that do real business work (finance, HR, operations) on top of a proven open-source ERP core, with verifiable evidence for every action.

> 🚧 **Status:** Private development, preparing an open-source release. Contributions will use the **DCO** (Developer Certificate of Origin, `git commit -s`). Watch this page — the public developer hub is already live at **[docs.helpifyr.com/developers](https://docs.helpifyr.com/developers/)**.

## What makes it different

- **Evidence over claims.** Every agent action is issue-driven, reviewed by an independent actor, and closed only after a live readback of the running system — "merged" is never mistaken for "deployed".
- **Governed autonomy.** Agents work behind human-in-the-loop gates for anything irreversible (payments, filings, customer-visible output). A three-account review model with server-side branch protection makes the gates mechanical, not conventional.
- **Layered knowledge, not one big prompt.** Role knowledge, company knowledge, live business data and per-task context are separate, permissioned layers — served to agents through a read-only gateway with provenance on every fact.

## Contribution status (DCO 1.1)

Contributions use the [Developer Certificate of Origin, version 1.1](https://developercertificate.org/) — every commit needs a `Signed-off-by` trailer (`git commit -s`). Inbound equals outbound under `AGPL-3.0-only`; no general CLA, no copyright assignment, no relicensing right (decision `JaddaHelpifyr/helpifyr-fabric#1542`, ANYFER GmbH, 2026-07-26).

| Repository | Rollout state |
|---|---|
| `jhf-weaver` | `ready_pre_live` |
| `jhf-docs` | `ready_pre_live` |
| `helpifyr-fabric` | `not_applicable` |

A repository not listed above has not yet been evaluated for public contribution intake.

## Repositories with a public posture

The repositories below are the only ones with a `public_candidate` or `public_contract_only` publication scope today; everything else remains Gitea-internal architecture detail, covered in the [Developer Hub repository map](https://docs.helpifyr.com/developers/repository-map).

| Repository | Class | Why public |
|---|---|---|
| `helpifyr-boost-advice-followup` | `boost` | generic_agpl_product_candidate |
| `helpifyr-boost-company-pulse` | `boost` | reference_boost_w0_bootstrap |
| `helpifyr-fabric` | `core` | proprietary_ip |
| `insurance-broker-core` | `application` | generic_agpl_product_candidate |
| `jhf-docs` | `documentation` | public_docs |
| `jhf-weaver` | `integration` | golden_path_pilot |

## Where to start

1. **[Developer Hub](https://docs.helpifyr.com/developers/)** — full repository map, roadmap, glossary, golden path.
2. **Golden Path** — `jhf-weaver` ships a devcontainer-based local lab (`docs.helpifyr.com/developers/golden-path-weaver`).
3. **Website** — [helpifyr.com](https://helpifyr.com).

---

*Development happens on a self-hosted Gitea (source of truth); these GitHub repositories are the distribution mirror, refreshed nightly. Issues and PRs here are not yet monitored — the public contribution path opens with the open-source release.*

## License

- License: AGPLv3
- Project: https://helpifyr.com

<sub>Generated projection. generated_from: `repository_landscape_v1@2026-09-23T21:13:04.694295+00:00`, `public_architecture_contract_v1@2026-09-23T21:13:04.694295+00:00`, `dco_contribution_policy_v1@1.1.0`. Source: helpifyr-fabric `scripts/build_org_profile.py` (helpifyr-fabric#1903). If this drifts from the live page, report a documentation issue.</sub>
