👋 Hi, I'm Rohit Dole

Senior Go Backend Engineer based in Hamburg, Germany. I build reliable, high-throughput distributed systems with a focus on data pipelines, event-driven architectures, and clean API design.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-rohit--dole-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rohit-dole-66aa1b105)

---

## Tech Stack

| Category           | Technologies                       |
| ------------------ | ---------------------------------- |
| **Language**       | Go                                 |
| **Messaging**      | Apache Kafka                       |
| **Databases**      | PostgreSQL, MongoDB, Elasticsearch |
| **Observability**  | Prometheus, Grafana                |
| **Infrastructure** | Docker, AWS                        |

---

## Featured Projects

### CDC Pipeline — PostgreSQL to Elasticsearch

A change data capture pipeline that streams row-level changes from PostgreSQL to Elasticsearch in near real-time.

- Captures WAL events via **Debezium** (logical replication)
- Publishes change events to **Kafka** topics per table
- Go consumers transform and index documents into **Elasticsearch**
- Designed for zero data loss with offset tracking and at-least-once delivery guarantees

**Stack:** Go · PostgreSQL · Debezium · Kafka · Elasticsearch · Docker

---

### Bulk Data Import / Export Service

A service for processing large-scale data transfers without overwhelming downstream systems or holding open long-lived transactions.

- Handles datasets of **1M+ records** using server-side streaming (chunked reads/writes)
- Import pipeline enforces **idempotency** via deterministic record keys to safely support retries
- Export pipeline streams results directly to the response writer, keeping memory overhead flat
- Configurable batch size and concurrency with back-pressure support

**Stack:** Go · PostgreSQL · Docker · Prometheus

---

## Currently Exploring

- Node.js and GraphQL for full-stack backend versatility
- Contributing to open source Go projects
