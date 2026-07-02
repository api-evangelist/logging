# Logging (logging)
An index and topic collection covering log ingestion, log search, log aggregation, and log pipeline services. Logging platforms collect event records from applications, infrastructure, containers, network devices, and security tooling, then parse, index, route, and retain them for search, alerting, troubleshooting, audit, and analytics. This collection spans hosted SaaS log platforms (Splunk, Sumo Logic, Datadog Logs, Coralogix, Axiom, Logz.io, Better Stack Logs), open-source log stacks (Elasticsearch / OpenSearch, Loki, Graylog, OpenObserve, SigNoz), log pipeline and shipper tooling (Fluentd, Fluent Bit, Logstash, Vector, Cribl), and cloud-native log services (AWS CloudWatch Logs, Google Cloud Logging, Azure Log Analytics, OpenTelemetry Logs).

**URL:** [https://apievangelist.com](https://apievangelist.com)

## Tags:

 - Logs, Log Aggregation, Log Ingestion, Log Search, Log Pipeline, Log Management

## Timestamps

- **Created:** 2026-05-19
- **Modified:** 2026-05-19

## Common Properties

- [Portal](https://apievangelist.com)
- [GitHubOrganization](https://github.com/api-evangelist)
- [JSONSchema - Log Event Schema](https://raw.githubusercontent.com/api-evangelist/logging/refs/heads/main/json-schema/logging-log-event-schema.json)
- [JSONSchema - Log Stream Schema](https://raw.githubusercontent.com/api-evangelist/logging/refs/heads/main/json-schema/logging-log-stream-schema.json)
- [JSON-LD](https://raw.githubusercontent.com/api-evangelist/logging/refs/heads/main/json-ld/logging-context.jsonld)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/logging/refs/heads/main/vocabulary/logging-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Log Ingestion and Collection | Logging platforms collect log events from applications, hosts, containers, cloud services, and network devices via HTTP endpoints, syslog, agents, and shippers such as Fluent Bit, Vector, and OpenTelemetry collectors. |
| Parsing and Enrichment | Incoming log lines are parsed into structured fields, enriched with metadata (host, service, environment, trace ID), and normalized so downstream search and analytics behave consistently across sources. |
| Indexing and Full-Text Search | Platforms like Elasticsearch, OpenSearch, Splunk, Graylog, and OpenObserve index log content for fast keyword, field, and time-range queries against very large data sets. |
| Log Routing and Pipelines | Log pipeline tools like Cribl, Vector, Fluentd, Fluent Bit, and Logstash route, transform, filter, sample, and replicate log streams between sources, destinations, and storage tiers. |
| Retention, Tiering, and Archival | Logging services manage hot, warm, and cold retention policies, archive raw logs to object storage, and enforce retention windows for cost control and compliance. |
| Alerting and Detection on Logs | Log platforms expose alert rules, saved searches, and detection content that fire on patterns, thresholds, anomalies, or security signatures observed in log streams. |
| Live Tail and Troubleshooting | Engineers stream live logs, filter by service or request, and pivot from a log line into traces, metrics, and related events during incident response and debugging. |
| Log-Based Audit and Compliance | Immutable log capture, retention policies, and access controls support SOC 2, HIPAA, PCI, and other audit and compliance use cases driven by log evidence. |

## Use Cases

| Name | Description |
|------|-------------|
| Application Troubleshooting and Debugging | Engineers search application and request logs across services to diagnose errors, latency spikes, and failed deployments in production environments. |
| Centralized Log Aggregation Across Clouds | Organizations aggregate logs from AWS CloudWatch, Google Cloud Logging, Azure Log Analytics, Kubernetes clusters, and on-prem systems into a single search and analytics surface. |
| Security and SIEM Use Cases | Security teams ingest authentication, network, endpoint, and audit logs into platforms like Splunk, Sumo Logic, Graylog, and QRadar to drive detections, investigations, and threat hunting. |
| Cost Control Through Log Pipelines | Teams use Cribl, Vector, and Fluent Bit to reduce, sample, route, and reshape log volume before it lands in expensive indexing tiers, optimizing cost per useful log. |
| Compliance and Audit Trail Retention | Regulated organizations retain structured logs for prescribed windows, with tamper-evident storage and access controls, to demonstrate compliance during audits. |
| OpenTelemetry-Native Logging | Modern stacks emit logs from applications as OpenTelemetry log records, correlate them with traces and metrics, and ship them through OTLP into back-ends like Axiom, OpenObserve, and SigNoz. |
| Kubernetes and Container Log Collection | Cluster operators run Fluent Bit, Fluentd, or Vector as DaemonSets to collect container logs and forward them into Loki, Elasticsearch, OpenSearch, or hosted log services. |
| Business and Product Analytics on Logs | Product and platform teams query structured event logs to build dashboards, funnels, and KPIs without standing up a separate analytics pipeline. |

## Integrations

| Name | Description |
|------|-------------|
| Splunk | Enterprise log search, indexing, and SIEM platform widely used for IT operations and security operations on high-volume log data. |
| Datadog Logs | Hosted log management integrated with Datadog metrics and APM, with log-to-metric pipelines, archives, and detection rules. |
| Elasticsearch / OpenSearch | Open-source distributed search engines that power many log stacks, including ELK and the OpenSearch project, for indexing and querying logs at scale. |
| Grafana Loki | Horizontally scalable, label-based log aggregation system designed to pair with Prometheus metrics and Grafana dashboards. |
| OpenTelemetry Logs | Open standard for emitting and transporting log records over OTLP, with collector pipelines that fan out to many logging back-ends. |
| Fluent Bit and Fluentd | Lightweight and feature-rich open-source log shippers used across Kubernetes, edge, and server fleets to collect and forward logs. |
| Vector | High-performance open-source observability data pipeline that collects, transforms, and routes logs, metrics, and traces. |
| Cribl Stream | Vendor-neutral observability pipeline that reduces, shapes, routes, and replays log and event data between sources and destinations. |

## Artifacts

Machine-readable API specifications organized by format.

### JSON Schema

- [Log Event Schema](json-schema/logging-log-event-schema.json)
- [Log Stream Schema](json-schema/logging-log-stream-schema.json)

### JSON Structure

- [Log Event Structure](json-structure/logging-log-event-structure.json)
- [Log Stream Structure](json-structure/logging-log-stream-structure.json)

### JSON-LD

- [Logging Context](json-ld/logging-context.jsonld)

### Examples

- [Log Event Example](examples/logging-log-event-example.json)
- [Log Stream Example](examples/logging-log-stream-example.json)

## Vocabulary

- [Logging Vocabulary](vocabulary/logging-vocabulary.yaml) — Unified taxonomy mapping 7 resources, 9 actions, 4 workflows, and 4 personas across log ingestion, search, aggregation, and pipeline platforms

## Network

This index references the following logging platform repositories:

- [Amazon CloudWatch](https://github.com/api-evangelist/aws-cloudwatch)
- [Axiom](https://github.com/api-evangelist/axiom)
- [Azure Log Analytics](https://github.com/api-evangelist/azure-log-analytics)
- [Better Stack](https://github.com/api-evangelist/betterstack)
- [Chronosphere](https://github.com/api-evangelist/chronosphere)
- [Coralogix](https://github.com/api-evangelist/coralogix)
- [Cribl](https://github.com/api-evangelist/cribl)
- [Datadog](https://github.com/api-evangelist/datadog)
- [Dynatrace](https://github.com/api-evangelist/dynatrace)
- [Elastic Stack (ELK Stack)](https://github.com/api-evangelist/elk-stack)
- [Elasticsearch](https://github.com/api-evangelist/elasticsearch)
- [Fluent Bit](https://github.com/api-evangelist/fluent-bit)
- [Fluentd](https://github.com/api-evangelist/fluentd)
- [Google Cloud Logging](https://github.com/api-evangelist/google-cloud-logging)
- [Grafana](https://github.com/api-evangelist/grafana)
- [Graylog](https://github.com/api-evangelist/graylog)
- [Honeycomb](https://github.com/api-evangelist/honeycomb)
- [IBM QRadar](https://github.com/api-evangelist/qradar)
- [Logstash](https://github.com/api-evangelist/logstash)
- [Loki](https://github.com/api-evangelist/loki)
- [New Relic](https://github.com/api-evangelist/new-relic)
- [OpenObserve](https://github.com/api-evangelist/openobserve)
- [OpenSearch](https://github.com/api-evangelist/opensearch)
- [OpenTelemetry](https://github.com/api-evangelist/opentelemetry)
- [SigNoz](https://github.com/api-evangelist/signoz)
- [SolarWinds](https://github.com/api-evangelist/solarwinds)
- [Splunk](https://github.com/api-evangelist/splunk)
- [Sumo Logic](https://github.com/api-evangelist/sumo-logic)
- [Vector](https://github.com/api-evangelist/vector)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
