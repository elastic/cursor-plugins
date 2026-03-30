# Elastic Cursor Plugins

[Cursor](https://cursor.com) plugins from Elastic.

> [!NOTE]
> **Technical Preview**
>
> These skills and tooling are in early release and under active development. Expect changes as skills are codified with robust
> evaluations and as the model landscape evolves. Check back frequently for updates.

## Plugin

### elastic

Elastic skills and documentation — Elasticsearch, Kibana, Observability, Security, Cloud, ES|QL, OpenTelemetry, and MCP docs access.

**Documentation MCP tools:**

Connects Cursor to the [Elastic Documentation MCP server](https://elastic.github.io/docs-builder/mcp/), giving your AI assistant direct access to Elastic documentation.

- **search_docs** — Search all published Elastic documentation by meaning
- **find_related_docs** — Discover documentation related to a topic
- **get_document_by_url** — Retrieve a specific documentation page
- **analyze_document_structure** — Analyze the structure of a documentation page
- **check_docs_coherence / find_docs_inconsistencies** — Evaluate documentation coverage and consistency

**Skills:**

| Namespace | Description |
| --- | --- |
| `cloud` | Elastic Cloud — project setup, access management, network security, and Serverless project lifecycle |
| `elasticsearch` | Elasticsearch — ES\|QL queries, data ingestion, security (authn, authz, audit), and troubleshooting |
| `kibana` | Kibana — dashboards, alerting rules, connectors, Vega visualizations, Agent Builder, streams, and audit logging |
| `observability` | Elastic Observability — OpenTelemetry instrumentation and migration (.NET, Java, Python), LLM observability, log search, SLOs, and service health |
| `security` | Elastic Security — alert triage, case management, detection rule management, and sample data generation |
