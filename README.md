# eulertools organization

The `eulertools` GitHub organization is **sunset**. Product source of truth has moved.

| What | Where |
|------|--------|
| **Organized archive** (private) | https://github.com/tebayoso/eulertools |
| **Raw dump** (private, July 2026) | https://github.com/tebayoso/euler-tools-platform |
| **Poxme** | https://github.com/tebayoso/poxme-monorepo and https://github.com/tebayoso/poxme (also `tebayoso/poxme*`) |
| **Omnicost** | https://github.com/tebayoso/omnicost |

The 122 product repos under this org are **archived** and point at dest paths in `tebayoso/eulertools` (or the Poxme / Omnicost repos above). This repository stays public as the org landing pointer and audit manifest. `.github` stays live for org profile/templates.

Cutover date: **2026-08-12**.

---

# eulertools-platform Manifest

> Historical consolidation manifest for the [eulertools](https://github.com/eulertools) GitHub organization. See the table above for current locations.

## Purpose

Audited all 123 repositories in the `eulertools` organization to build a comprehensive manifest for consolidation into a single `eulertools-platform` repository.

## Scope

| Metric | Count |
|--------|-------|
| Total repositories | 123 |
| Active repos (pushed ≥2023) | 60 |
| Archived repos | 38 |
| Public repos | 5 |
| Private repos | 118 |
| Forked repos | 0 |

## Language Distribution

| Language | Count |
|----------|-------|
| TypeScript | 69 |
| Python | 14 |
| HCL (Terraform) | 9 |
| JavaScript | 9 |
| Solidity | 6 |
| Go | 4 |
| Ruby | 3 |
| HTML | 7 |
| PL/pgSQL | 1 |
| Java | 1 |
| Shell | 1 |
| Dockerfile | 1 |
| Vue | 2 |
| Jupyter Notebook | 1 |
| Unknown | 5 |

## Category Breakdown

### Platform Core
| Repo | Lang | Size | Stacked | Recommendation |
|------|------|------|---------|----------------|
| platform-api | TS | 2.5 MB | AWS CDK, API Gateway, Lambda | KEEP |
| platform-core | TS | 3.9 MB | | KEEP |
| platform-datalake | TS | 447 KB | | KEEP |
| platform-infra | TS | 1.6 MB | AWS CDK (VPC, Security Groups) | KEEP |
| platform-directory | JS | 1 MB | Auth, subscriptions, payments | KEEP |
| platform-communications | HTML | 828 KB | Centralized comms hub | KEEP |
| platform-cms | TS | 398 KB | | KEEP |
| platform-oms | TS | 511 KB | | KEEP |

### Blockchain & DeFi
| Repo | Lang | Size | Recommendation |
|------|------|------|----------------|
| blockchain-worker | TS | 5 MB | KEEP — core streaming pipeline |
| blockchain-clients | TS | 943 KB | KEEP |
| blockchain-contracts | Solidity | 674 KB | KEEP |
| blockchain-hardhat-contracts | Solidity | 2.9 MB | KEEP |
| blockchain-laboratory | TS | 32 KB | ARCHIVE |
| blockchain-marketplace-worker | TS | 227 KB | ARCHIVE |
| euler-blockchain-contracts | Solidity | 172 KB | KEEP |
| contracts | Solidity | 4 MB | KEEP |
| platform-nft | TS | 9.5 MB | KEEP |
| platform-nft-factory | TS | 2.7 MB | KEEP |
| platform-nft-zksnark | TS | 23 KB | ARCHIVE |
| explorer-v2 | TS | 2 MB | KEEP |
| explorer-client | JS | 51 MB | KEEP |
| explorer-backend | TS | 4.5 MB | KEEP |
| explorer-platform | HTML | 7.3 MB | KEEP |
| euler-assets | TS | 230 MB | CDN — KEEP |
| polygon-node | Go | 140 MB | ARCHIVE |
| gethexporter | Go | 19 KB | ARCHIVE |
| heco-geth-exporter | Go | 20 KB | ARCHIVE |
| ethereum-etl-postgres | Shell | 2.5 MB | KEEP |
| ethereum-node | HCL | 11 KB | ARCHIVE |
| bsc-datalake | Python | 819 KB | ARCHIVE |
| bsc-etl-streaming | Python | 731 KB | ARCHIVE |
| blockchain-bots | TS | 25 KB | REMOVE |
| opticks | TS | 9.6 MB | KEEP — Feathers.js microservice |

### Data & ETL
| Repo | Language | Size | Recommendation |
|------|----------|------|----------------|
| data-crawlers | Jupyter | 23 MB | ARCHIVE (old) |
| data-datalake | TS | 1.2 MB | KEEP |
| data-processors | TS | 3.1 MB | KEEP |
| data-services | TS | 1.5 MB | KEEP |
| data-price-avg-kinesis | Java | 7 KB | REMOVE |
| etl | HCL | 112 KB | ARCHIVE |
| etl-cex | TS | 12 KB | REMOVE |
| etl-ethscan | TS | 1.8 MB | KEEP |
| eth-extractors | Python | 1.3 MB | KEEP |
| lambda-observers | Python | 6.6 MB | ARCHIVE |
| omnicost-scrapers | Python | 1 MB | KEEP |

### Frontend & Kits
| Repo | Lang | Size | Recommendation |
|------|------|------|----------------|
| kit-devias-4 | TS | 16 MB | KEEP (Devias template) |
| kit-devias-3 | TS | 9.7 MB | KEEP (Devias template) |
| kit-devias-6 | TS | 23 MB | KEEP (Devias template) |
| kit-setdesign | JS | 5.5 MB | KEEP (React components) |
| kit-euler-tools | TS | 7.6 MB | KEEP (Web3/React libs) |
| poxme-webapp | TS | 27.3 MB | KEEP (PoxMe browser client) |
| poxme-next | TS | 12.6 MB | KEEP (PoxMe Next.js) |
| poxme-platform | HTML | 25.5 MB | KEEP (PoxMe infra) |
| poxme-ssr | JS | 3 MB | ARCHIVE |
| poxme-ssr-prototype | TS | 1.9 MB | REMOVE |
| poxme-landing | JS | 12.8 MB | KEEP |
| poxme-ssr | JS | 3 MB | ARCHIVE |
| euler-app | TS | 2.7 MB | KEEP |
| euler-static | HTML | 43 MB | KEEP |
| static-site-template | HTML | 9 MB | KEEP |

### API & Backend Services
| Repo | Lang | Size | Recommendation |
|------|------|------|----------------|
| customers-api | TS | 915 KB | SEED (V1 API) |
| charting-backend | Python | 2.7 MB | KEEP |
| charts-backend | Python | 3.3 MB | KEEP |
| service-farms-backend | JS | 2.5 MB | KEEP |
| automate-jobs-backend | TS | 88 MB | KEEP (n8n) |
| automate-jobs-client | Vue | 6.8 MB | KEEP (n8n) |
| automate-jobs-platform | HTML | 1.2 MB | KEEP |
| automate-jobs-templates | | 38 KB | KEEP |
| inverti-client | TS | 10 MB | KEEP |
| inverti-backend | Ruby | 360 KB | KEEP |
| websocket-clients | TS | 2.2 MB | KEEP |
| subscriptions-client | TS | 2.8 MB | ARCHIVE |
| marketplace-client | TS | 313 KB | REMOVE |
| platform-communications | HTML | 828 KB | KEEP |
| clients-explorer-v1 | JS | 21 MB | ARCHIVE |
| onestic-smartie | TS | 3.2 MB | KEEP |
| onestic-smartie-frontend | | 2.7 MB | REMOVE |
| euler-cli | TS | 131 KB | KEEP |
| euler-unstoppable-login | TS | 3 MB | KEEP |

### Infrastructure & DevOps
| Repo | Lang | Size | Recommendation |
|------|------|------|----------------|
| terraform-modules | HCL | 36 KB | KEEP |
| infrastructure | HCL | 127 KB | KEEP |
| prometheus | HCL | 20 KB | KEEP |
| grafana | HCL | 7 KB | KEEP |
| database-scripts | PL/pgSQL | 449 KB | KEEP |
| typescript-sdk | TS | 4 KB | KEEP |
| cdk-constructs | TS | 6 KB | KEEP |
| cdk-sam-test | JS | 418 KB | KEEP |
| devops-blockchain-nodes | TS | 1.2 MB | KEEP |
| binance-node | Dockerfile | 48 KB | ARCHIVE |
| onboarding | Ruby | 203 KB | KEEP |
| docs.euler.tools | | 392 KB | KEEP |

### Bots & Automation
| Repo | Lang | Size | Recommendation |
|------|------|------|----------------|
| euler_chat_bot | Vue | 14 MB | ARCHIVE |
| eulert_bot | HCL | 53 KB | ARCHIVE |
| dialva-bot | TS | 506 KB | KEEP |
| Discord-Bot | JS | 35 KB | ARCHIVE |
| playoffnations | JS | 171 KB | ARCHIVE/REMOVE |

### Archive / Remove Candidates
| Repo | Size | Reason |
|------|------|--------|
| argocd-test | 13 KB | Test repo |
| bot-arbitrage | 0 KB | Empty |
| blockchain-bots | 25 KB | Empty/dead |
| data-price-avg-kinesis | 7 KB | Tiny/dead |
| etl-cex | 12 KB | Tiny/dead |
| market-place-client | 313 KB | Archived/dead |
| marketplace-client | 313 KB | Archived/dead |
| onestic-smartie-frontend | 2.7 MB | Dead/deprecated |
| poxme-ssr-prototype | 1.9 MB | Prototype/dead |
| blockchain-laboratory | 32 KB | Dead/unused |
| blockchain-marketplace-worker | 227 KB | Archived/dead |
| subscriptions-client | 2.8 MB | Archived/dead |
| private-assets | 4.9 MB | Archived assets |
| hubspot-website | 24 MB | Archived corporate site |
| euler_chat_bot | 14 MB | Archived bot |
| eulert_bot | 53 KB | Archived bot |
| data-crawlers | 23 MB | Archived (2021) |
| lambda-observers | 6.6 MB | Archived/dead |
| plotball-nations | 171 KB | Dead extension |
| urban-train | 617 KB | Archived |
| client-admin | 906 KB | Archived |
| etl-cex | 12 KB | Tiny/dead |
| omnicost-\* repos (6) | Varies | Many archived — review for consolidation |

### Metadata & Templates
| Repo | Size | Recommendation |
|------|------|----------------|
| .github | 19 KB | KEEP — GitHub templates |
| .github-private | 2 KB | KEEP — Private templates |
| support | 2 KB | ARCHIVE (support repo) |

### Public Repos
| Repo | Stars | Topic | Recommendation |
|------|-------|-------|----------------|
| contracts | 0 | blockchain, contracts | KEEP |
| ethereum-etl-postgres | 1 | ETL + PostgreSQL | KEEP |
| euler-unstoppable-login | 2 | Staking + Unstoppable | KEEP |
| DefiLlama-Adapters | 0 | DeFi Llama | KEEP |
| docs.euler.tools | 3 | docs | KEEP |
| panoramix | 0 | Eveem decompiler | KEEP |
| websocket-clients | 0 | services | KEEP |
| .github | 0 | templates | KEEP |

## Directory Structure (Proposed)

```
eulertools-platform/
├── .github/                    # Templates & workflows
├── .github-private/            # Private templates
├── platform/
│   ├── core/                    # platform-ap, platform-core, platform-infra
│   ├── api/                     # platform-api, customers-api, service-farms-backend
│   ├── datalake/               # platform-datalake, data-services, data-processors
│   ├── clients/                # platform-directory, platform-communications
│   ├── cms/                    # platform-cms, platform-oms
│   ├── nft/                    # platform-nft, platform-nft-factory, platform-nft-zksnark
│   └── infra/                  # terraform-modules, prometheus, grafana, database-scripts
├── blockchain/
│   ├── contracts/              # contracts, euler-blockchain-contracts, blockchain-contracts
│   ├── hardhat/               # blockchain-hardhat-contracts
│   ├── workers/               # blockchain-worker
│   ├── clients/               # blockchain-clients, evm-socket-client
│   ├── explorers/             # explorer-v2, explorer-backend, explorer-client
│   ├── etl/                   # ethereum-etl-postgres, etl-ethscan, eth-extractors
│   ├── nodes/                 # polygon-node, gethexporter
│   └── assets/                # euler-assets
├── frontend/
│   ├── kits/                  # kit-devias-3, kit-devias-4, kit-devias-6
│   ├── euler-tools/           # kit-euler-tools, kit-setdesign
│   ├── poxme/                 # poxme-webapp, poxme-next, poxme-platform, poxme-landing
│   ├── euler/                 # euler-app, euler-static, static-site-template
│   └── onestic/               # onestic-smartie
├── data-pipeline/
│   ├── crawlers/              # omnicost-scrapers, data-crawlers
│   ├── processors/            # lambda-observers, eth-extractors
│   ├── streaming/             # bsc-etl-streaming, data-price-avg-kinesis
│   └── charts/                # charting-backend, charts-backend
├── devops/
│   ├── cdks/                  # cdk-constructs, typescript-sdk, cdk-sam-test
│   ├── ci-cd/                 # devops-blockchain-nodes, ethereum-node
│   └── monitoring/            # prometheus, grafana
├── bots/
│   ├── dialva-bot/
│   ├── discord-bot/
│   └── euler-chat-bot/
├── docs/
│   ├── docs.euler.tools/
│   └── onboarding/
├── archive/                   # Archived repos kept for reference
│   ├── omnicost/
│   ├── legacy/
│   └── prototypes/
├── remove/                    # Marked for deletion
└── README.md
```

## Audit Details

See `reports/` for individual repo audit reports. Each report includes:
- Overview (metadata, visibility, activity)
- Stack & Tech (frameworks, dependencies)
- Routes & Endpoints (API paths)
- Fork Analysis (parent, custom commits)
- Contributors (top authors)
- Key Features (what the repo does)
- SOTA / Standout Code
- Consolidation Recommendation (SEED/KEEP/ARCHIVE/REMOVE)
- Risk Assessment

## How to Use

1. Review `manifest.yml` for structured repo metadata
2. Read individual reports in `reports/{repo}.md` for deep audit results
3. Use the consolidation sections in each report to prioritize migration
4. Follow the proposed directory structure to plan code movement
