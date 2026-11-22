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
