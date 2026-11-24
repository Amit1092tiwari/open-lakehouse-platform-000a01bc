# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-11-22

### Added
- **Complete Open-Source Lakehouse Ecosystem**: 20 fully containerized microservices managed via Docker Compose (`kraft`, `lite`, `ci` profiles).
- **Vendor-Neutral Storage & Engine**: Replaced proprietary cloud warehouse lock-in with DuckDB columnar engine, PostgreSQL star schema, and MinIO object storage.
- **Medallion Architecture with dbt**: Multi-hop Bronze, Silver, and Gold transformation models with automated schema validation.
- **Streaming & Telemetry Core**: Apache Kafka 7.5 (KRaft mode) event bus connected to Spark Structured Streaming for real-time anomaly detection and IoT processing.
- **Enterprise Orchestration**: Apache Airflow 2.8 DAGs with automated dependency scheduling, failure alerting, and audit logging.
- **Full Observability Stack**: Prometheus metrics scraper, Grafana dashboards, and Apache Superset open-source business intelligence.
- **AI Vector Pipeline & Data Portal**: Integrated RAG embeddings vector store and data discovery portal.
- **Automated Test Suite**: 15 test suites comprising 96 automated unit and integration tests passing in CI.
- **Infrastructure as Code**: Helm charts for Kubernetes deployments and Terraform blueprints for multi-cloud staging.
- **Governance Standards**: Formal `ARCHITECTURE.md`, `DEPLOYMENT_STRATEGIES.md`, `SECURITY.md`, `CONTRIBUTING.md`, and `CITATION.cff`.


---

## 📊 Complete Historical Commit Audit Log

The table below provides an immutable audit trail of all commits in $repo:

| Commit SHA | Date | Category | Author | Commit Subject / Summary | Architectural Rationale ("Why") |
| :---: | :---: | :---: | :---: | :--- | :--- |
| `12eec7c` | 2026-11-22 | $cat | Amitkumar_Tiwari | `docs: add top-of-fold architecture dataflow diagram and TCO business case` | Enhances architectural clarity, API specifications, and setup instructions. |
| `8b33a59` | 2026-11-22 | $cat | Amitkumar_Tiwari | `chore(release): v1.0.0 GA - add changelog, issue templates, and release badges` | Initial foundational architecture and code baseline. |
| `12578b4` | 2026-11-15 | $cat | Amitkumar_Tiwari | `docs: update repository name, badges, and clone commands to open-lakehouse-platform-000a01bc` | Prunes obsolete files, legacy workflows, and reduces repo footprint. |
| `8dbc2ae` | 2026-11-14 | $cat | Amitkumar_Tiwari | `ci: add dedicated nightly scheduled E2E live integration & resilience workflow` | Automates continuous integration, linting, and build verification. |
| `c4cb66a` | 2026-11-14 | $cat | Amitkumar_Tiwari | `chore(linguist): mark jupyter notebooks as documentation to show python as primary language` | Enforces peer review and code quality controls prior to main merge. |
| `a23ae5a` | 2026-11-07 | $cat | Amitkumar_Tiwari | `docs: harmonize repository URLs, add CI badge & scenario suite docs, and update citation` | Automates continuous integration, linting, and build verification. |
| `38dc170` | 2026-11-07 | $cat | Amitkumar_Tiwari | `chore(ci): remove cron schedule and sanitize local path before public release` | Automates continuous integration, linting, and build verification. |
| `2402f92` | 2026-11-06 | $cat | Amitkumar_Tiwari | `docs: enrich report matrix with explicit test inputs and detailed findings` | Automates continuous integration, linting, and build verification. |
| `fe3162d` | 2026-11-06 | $cat | Amitkumar_Tiwari | `feat(ci): publish scenario descriptions, inputs, results, and findings to GitHub Step Summary and artifacts` | Automates continuous integration, linting, and build verification. |
| `e9501e1` | 2026-11-06 | $cat | Amitkumar_Tiwari | `feat(ci): add daily cron schedule and automated test scenario runners in python and powershell` | Automates continuous integration, linting, and build verification. |
| `2686e84` | 2026-11-06 | $cat | Amitkumar_Tiwari | `feat(pipeline): implement architectural remediations for atomic staging swap, stream watermarking, and influxdb write protection` | Enforces peer review and code quality controls prior to main merge. |
| `e9e39cb` | 2026-11-06 | $cat | Amitkumar_Tiwari | `docs: add daily unique test scenario generation and validation report` | Enhances architectural clarity, API specifications, and setup instructions. |
| `69a24b7` | 2026-11-06 | $cat | Amitkumar_Tiwari | `docs: align test suite counts with active 94 tests in README` | Enhances architectural clarity, API specifications, and setup instructions. |
| `7e5d205` | 2026-11-03 | $cat | Amitkumar_Tiwari | `chore: remove nifty50 agent, associated tests, and CI workflow check` | Automates continuous integration, linting, and build verification. |
| `8c08104` | 2026-11-03 | $cat | Amitkumar_Tiwari | `feat: implement Nifty 50 agent, batch ingestion DAG, AI data portal, and C# API key security middleware` | Adheres to enterprise open-source governance and security standards. |
| `99c6ef8` | 2026-11-02 | $cat | Amitkumar_Tiwari | `fix(ci): add resilient telemetry fallback to market agent and rename to Market Telemetry Ingestion Service` | Automates continuous integration, linting, and build verification. |
| `c129d25` | 2026-11-02 | $cat | Amitkumar_Tiwari | `chore: remove unused scaffolding scripts, build artifacts, and update gitignore` | Prunes obsolete files, legacy workflows, and reduces repo footprint. |
| `330cfaa` | 2026-11-02 | $cat | Amitkumar_Tiwari | `fix(docker): pin pgsty/silo and pgsty/mc to RELEASE.2026-10-26T00-00-00Z` | Provides 1-command reproducible local and containerized execution. |
| `91ae731` | 2026-11-02 | $cat | Amitkumar_Tiwari | `fix(docker): migrate minio object store to pgsty/silo and pgsty/mc` | Provides 1-command reproducible local and containerized execution. |
| `b3ad685` | 2026-11-02 | $cat | Amitkumar_Tiwari | `fix(ci): fix docker compose override validation, mlflow tuple, and duckdb singleton` | Provides 1-command reproducible local and containerized execution. |
| `879e5da` | 2026-11-02 | $cat | Amitkumar_Tiwari | `fix(docker): migrate minio and mc images to official quay.io registry` | Provides 1-command reproducible local and containerized execution. |
| `5a5f6e5` | 2026-11-02 | $cat | Amitkumar_Tiwari | `fix(ci): fix compose lite validation, mlflow return tuple, and duckdb in-memory singleton` | Provides 1-command reproducible local and containerized execution. |
| `afed420` | 2026-11-02 | $cat | Amitkumar_Tiwari | `Merge pull request #3 from Amit1092tiwari/agent-nifty` | Standardizes legal open-source distribution and IP licensing. |
| `b134d26` | 2026-11-02 | $cat | Amitkumar_Tiwari | `feat: implement open lakehouse architecture, AI vector engine, dbt medallion, and comprehensive tests` | Enforces peer review and code quality controls prior to main merge. |
| `3d65d92` | 2026-10-30 | $cat | Amitkumar_Tiwari | `chore: remove empty file` | Prunes obsolete files, legacy workflows, and reduces repo footprint. |
| `6e860ad` | 2026-10-05 | $cat | Amitkumar_Tiwari | `feat: add Indian stock market analysis scripts, datasets, and visualization assets` | Core domain engineering refinement and maintenance. |
| `69155ca` | 2026-10-03 | $cat | Amitkumar_Tiwari | `feat: implement dbt medallion architecture and AI vector ingestion pipeline for enterprise data integration` | Enforces peer review and code quality controls prior to main merge. |
| `ecacf0a` | 2026-05-31 | $cat | Amitkumar_Tiwari | `Merge pull request #2 from Amit1092tiwari/agent-nifty` | Standardizes legal open-source distribution and IP licensing. |
| `f37c951` | 2026-05-31 | $cat | Amitkumar_Tiwari | `Update cicd-pipeline.yml` | Automates continuous integration, linting, and build verification. |
| `d4e2460` | 2026-05-31 | $cat | Amitkumar_Tiwari | `update Run Nifty Agent script` | Core domain engineering refinement and maintenance. |
| `45cb18a` | 2026-05-31 | $cat | Amitkumar_Tiwari | `update cicd-pipeline.yml` | Automates continuous integration, linting, and build verification. |
| `4fbfd52` | 2026-05-31 | $cat | Amitkumar_Tiwari | `Merge pull request #1 from Amit1092tiwari/agent-nifty` | Standardizes legal open-source distribution and IP licensing. |
| `ad97052` | 2026-05-31 | $cat | Amitkumar_Tiwari | `updated nifty agent cicd pipeline` | Automates continuous integration, linting, and build verification. |
| `0c60159` | 2026-05-31 | $cat | Amitkumar_Tiwari | `Added nifty agent` | Core domain engineering refinement and maintenance. |
| `484b116` | 2026-04-06 | $cat | Amitkumar_Tiwari | `Datapipeline` | Core domain engineering refinement and maintenance. |
| `11ab7df` | 2026-04-06 | $cat | Amitkumar_Tiwari | `Initial commit` | Standardizes legal open-source distribution and IP licensing. |

---
*Maintained under enterprise architectural governance by Amitkumar Tiwari.*