# Connected Mobility — Privacy-Preserving GenAI for Vehicle Telemetry & Customer Data

**Fictional organization:** VectorPath Mobility Research  
**Project type:** Synthetic enterprise case repository  
**Data:** synthetic case evidence across multiple linked CSV/JSON datasets  
**Security:** No real employee/customer data, credentials, customer IP, or Bosch proprietary material.

## Project overview

This repository represents a fictional enterprise system and its operational evidence.
It includes business context, architecture and trust boundaries, source-system telemetry,
privacy records, IAM events, supplier claims and source documentation, knowledge-base
fragments, model output samples, audit records and software for a local read-only
review environment.

**All organizations, suppliers, individuals, incidents and systems are fictitious.**
External addresses use documentation IP ranges and `.example` domains where applicable.
Evidence may be incomplete, contradictory or outdated, as in actual operational reviews.
No documents in this repository represent an actual independent security certification.

## Repository structure

| Path | Contents |
|---|---|
| `case/` | Operating context, stakeholder responsibilities, case registry |
| `data/` | Synthetic records in CSV/JSON with identifiers and data dictionary |
| `docs/policies/` | Fictional enterprise policies and version history |
| `docs/vendors/` | Vendor submissions and synthetic assurance evidence |
| `docs/incident/` | Event dossier records from four operational workstreams |
| `architecture/` | Architecture, trust boundaries and simulated workflow configuration |
| `src/` | Read-only evidence/retrieval application example (standard-library Python) |
| `tests/` | Standard-library smoke tests |
| `scripts/` | Integrity verification and record inspection utilities |
| `metadata/` | Dataset manifest, SHA256 hashes and project metadata |

## Key datasets

| File | Records | Description |
|---|---:|---|
| `data/access_reviews.csv` | 260 | Access request and review records |
| `data/approval_audit.csv` | 260 | Associated audit entries |
| `data/assets.csv` | 90 | Enterprise assets and ownership |
| `data/baseline_comparison.csv` | 96 | Synthetic enterprise reference data |
| `data/control_catalog.csv` | 50 | Enterprise control catalog |
| `data/customer_cases.csv` | 320 | Support, purpose, consent and privacy information |
| `data/data_dictionary.csv` | 15 | Synthetic enterprise reference data |
| `data/identity_access.csv` | 900 | Identity and access events |
| `data/llm_analyst_outputs.csv` | 220 | Historical AI-generated draft output records |
| `data/mail_messages.csv` | 180 | Synthetic email content and message metadata |
| `data/model_evaluations.csv` | 180 | Historical model evaluation events |
| `data/network_flows.csv` | 1,300 | Network/session telemetry |
| `data/rag_chunks.csv` | 180 | Knowledge fragments with source and access metadata |
| `data/red_team_scenarios.json` | 20 | Fictional adversarial-scenario stimuli |
| `data/risk_register.csv` | 50 | Previously registered enterprise risks |
| `data/scenario_events.csv` | 37 | Synthetic enterprise reference data |
| `data/siem_alerts.csv` | 240 | Security detection alerts and their record links |
| `data/vehicle_location_segments.csv` | 400 | Synthetic enterprise reference data |
| `data/vendor_evidence_index.csv` | 40 | Vendor-document catalog |
| `data/vendor_questionnaire.csv` | 120 | Vendor assurance questionnaire submissions |

## Evidence and data integrity

- `data/README.md` contains data semantics and source descriptions.
- `metadata/data_manifest.json` records dataset size, row count and SHA256 hashes.
- `scripts/validate_repo.py` validates dataset integrity and cross-source references.
- `docs/` and `case/` contain original synthetic business evidence and records.

## Local verification and reference service

No installation is required to read the GitHub-hosted source files and datasets.
To run the optional local Python utilities, Python 3 standard library is sufficient:

```bash
python scripts/validate_repo.py
python -m unittest discover -s tests
```

The local software is a dry-run model and does **not** contact external systems,
change access privileges, call an LLM, run attacks or perform real-world actions.

## Repository boundaries

This is a **synthetic project evidence and source-code repository**. The historical
records and AI-generated drafts are source material and should not be considered
independently verified conclusions.

## Additional project documents

- `case/EVIDENCE_CATALOG.md` — neutral source index
- `docs/business/` — service charter and operating boundaries
- `docs/engineering/` — data contracts, ADRs, test strategy
- `docs/privacy/` — data processing register
- `docs/security/` — security model
- `docs/operations/` — service-readiness considerations
- `docs/standards/` — applicable external references
- `data/application_requests.csv`, `data/retrieval_access_log.csv`, `data/inference_telemetry.csv` — operational evidence
- `.github/workflows/ci.yml` — standard-library integrity checks and unit tests

## Maturity statement

The case, documentation, and source contracts are designed to resemble enterprise repositories, but **this is not a deployable or independently audited production system**. No real external integration, secrets, AI inference endpoint or industrial action is enabled.

### Domain context

`case/DOMAIN_OPERATIONS.md` describes the domain-specific source systems and technical boundaries.
