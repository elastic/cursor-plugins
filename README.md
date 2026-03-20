# Elastic Cursor Plugins

[Cursor](https://cursor.com) plugins from Elastic.

> [!NOTE]
> **Technical Preview**
>
> These skills and tooling are in early release and under active development. Expect changes as skills are codified with robust
> evaluations and as the model landscape evolves. Check back frequently for updates.

## Plugins

### elastic-docs

Connects Cursor to the [Elastic Documentation MCP server](https://elastic.github.io/docs-builder/mcp/), giving your AI assistant direct access to Elastic documentation.

**Available tools:**

- **search_docs** — Search all published Elastic documentation by meaning
- **find_related_docs** — Discover documentation related to a topic
- **get_document_by_url** — Retrieve a specific documentation page
- **analyze_document_structure** — Analyze the structure of a documentation page
- **check_docs_coherence / find_docs_inconsistencies** — Evaluate documentation coverage and consistency

### Namespace skills plugins

Separate Cursor plugins for each top-level namespace in [elastic/agent-skills](https://github.com/elastic/agent-skills).

| Plugin | Namespace | Description |
| --- | --- | --- |
| **elastic-cloud** | `cloud` | Elastic Cloud skills — project setup, access management, network security, and Serverless project lifecycle |
| **elastic-elasticsearch** | `elasticsearch` | Elasticsearch skills — ES\|QL queries, data ingestion, security (authn, authz, audit), and troubleshooting |
| **elastic-kibana** | `kibana` | Kibana skills — dashboards, alerting rules, connectors, Vega visualizations, Agent Builder, streams, and audit logging |
| **elastic-observability** | `observability` | Elastic Observability skills — OpenTelemetry instrumentation and migration (.NET, Java, Python), LLM observability, log search, SLOs, and service health |
| **elastic-security** | `security` | Elastic Security skills — alert triage, case management, detection rule management, and sample data generation |
