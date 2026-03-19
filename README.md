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
| **elastic-skills-cloud** | `cloud` | Skills for Elastic Cloud — hosted cluster operations, deployment, and platform patterns |
| **elastic-skills-elasticsearch** | `elasticsearch` | Skills for Elasticsearch — search, indexing, ES\|QL, security, authentication, and ingestion |
| **elastic-skills-kibana** | `kibana` | Skills for Kibana — alerts, connectors, dashboards, and administration |
| **elastic-skills-observability** | `observability` | Skills for Elastic Observability — APM, logs, metrics, and Synthetics |
| **elastic-skills-security** | `security` | Skills for Elastic Security — SIEM, detection, and security operations |
