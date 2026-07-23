# OpenDataLedger  
### The Open Ledger for the Internet’s Data  
*A universal, encrypted, open-source API engine for every database.*

---

## 🌐 Overview

**OpenDataLedger** is an independent, open-source, end-to-end encrypted platform that automatically generates APIs for virtually any database. Designed for developers, enterprises, researchers, and open-data communities, OpenDataLedger enables a unified, secure, zero-trust way to access, integrate, synchronize, and exchange data across all systems.

This project is licensed under **AGPL 3.0+**, with attribution required to **Roxanne Ardary** and **https://www.roxanneardary.com/** under **Section 7**.

---

# 🚀 Key Features

## 🔒 1. End-to-End Encryption (E2EE)
- Client-side cryptographic key ownership  
- Zero-knowledge transmission  
- Field-level encryption (AES-GCM)  
- Encrypted metadata mode  
- Post-quantum optional mode (CRYSTALS-Kyber)

---

## 🗄 2. Universal Database Connections

### **Supported SQL**
- MySQL / MariaDB  
- PostgreSQL  
- SQLite  
- SQL Server  
- Oracle  
- CockroachDB  
- YugabyteDB  

### **Supported NoSQL**
- MongoDB  
- Redis / Dragonfly  
- Cassandra  
- ScyllaDB  
- DynamoDB  
- CouchDB  

### **Supported Search & Analytics**
- Elasticsearch  
- OpenSearch  
- Meilisearch  

### **Supported Cloud & External Sources**
- Snowflake  
- BigQuery  
- Amazon Athena  
- Redshift  
- S3 / MinIO  
- Google Cloud Storage  
- Azure Blob  

### **Streaming & Real-Time**
- Kafka  
- Pulsar  
- Redpanda  
- Kinesis  
- WebSockets  

---

## 🧩 3. Automatic API Generation

OpenDataLedger automatically generates:

### **REST Endpoints**
- CRUD for all tables/collections  
- Join aggregation endpoints  
- System endpoints  
- Auto-pagination & filtering  

### **GraphQL API**
- Auto-generated GraphQL schema  
- Resolvers for every table, relationship, and query  
- GraphQL subscriptions for real-time changes  

### **WebSocket Event Streams**
- Push notifications on insert/update/delete  
- Custom channel creation  

---

## 🔍 4. Cross-Database Queries

Write a single query that spans multiple databases.

**Example GraphQL Query:**

```graphql
{
  orders(db: "mysql") {
    id
    total
    customer {
      email
      history(db: "mongodb") {
        lastLogin
        purchases
      }
    }
  }
}
```

---

## 🌉 5. API Gateway + Rate Limiting + WAF

The gateway includes:

- Query cost evaluation  
- Burst + sustained limits  
- Signature-based threat detection  
- Behavior-based threat detection  
- SQL/NoSQL/GraphQL injection firewall (WAF)  

---

## 🔐 6. Zero-Trust Access Control

- Identity-aware routing  
- Dynamic least-privilege rules  
- Field-level visibility rules  
- Row-level security (RLS)  
- Attribute-based access control (ABAC)  
- Policy Engine based on Rego  

---

## 🔁 7. SDK Auto-Generation

OpenDataLedger can generate full SDKs in:

- JavaScript / TypeScript  
- Python  
- Go  
- Rust  
- Java  
- PHP  
- C#  
- Dart (Flutter)  

Each SDK includes built-in:
- Encryption utilities  
- Query builder  
- Typed models (TS/Go)  

---

## 🧠 8. Intelligent Automation

### AI Query Optimizer
- Detects slow patterns  
- Suggests indexes  
- Suggests schema improvements  
- Auto-rewrites inefficient queries  

### AI Schema Mapper
- Maps SQL schema → NoSQL schema  
- SQL <→ Search engine index mapping  
- Normalization suggestions  

---

## 🧩 9. Plugin Ecosystem

OpenDataLedger supports safe, sandboxed plugins using:

- WASM  
- Rust  
- Python (sandboxed mode)  

Plugin types include:
- Database drivers  
- Authentication providers  
- Validation modules  
- Logging exporters  
- Encryption packs  
- Webhook/event extenders  

---

## 🗃 10. Data Lifecycle Management

- Data retention rules  
- Legal hold  
- Automated archival  
- Dataset versioning  
- Time-travel queries  
- Dataset diffs  

---

## 🛡 11. Auditing & Chain of Custody

Every action is:

- Hashed  
- Timestamped  
- Added to an append-only cryptographic ledger  
- Exportable for SOC 2, HIPAA, PCI, GDPR  

---

## 🛠 12. Developer Experience (DX)

### One-Command Deployment
```bash
odl deploy --all
```

### Local Developer Playground
- REST explorer  
- GraphQL Studio  
- WebSocket event viewer  
- Encryption sandbox  

### Infra-as-Code Support
- YAML  
- JSON  
- Terraform provider  

---

## 📊 13. Observability & Telemetry

- OpenTelemetry support  
- Tracing to Jaeger/Zipkin  
- Metrics to Prometheus  
- Logs to ELK / Loki  
- Query heatmaps  
- Performance dashboards  

---

## 🔮 14. Future-Proofing

- Post-quantum encryption mode  
- Distributed storage connectors:  
  - IPFS  
  - Filecoin  
  - Arweave  
- ENS-based API identifiers  
- Offline-first encrypted replicas  

---

# 🧱 Architecture

```
                ┌──────────────────────────┐
                │     Client SDKs (E2EE)   │
                └───────────┬──────────────┘
                            ▼
                ┌──────────────────────────┐
                │   OpenDataLedger Gateway │
                │  (WAF, Rate Limit, ABAC) │
                └───────────┬──────────────┘
                            ▼
                ┌──────────────────────────┐
                │  Query Translator Engine │
                ├──────────────────────────┤
                │  GraphQL Generator       │
                │  REST Generator          │
                │  AI Query Optimizer      │
                └───────────┬──────────────┘
                            ▼
          ┌──────────────────────────────────────────┐
          │         Multi-Database Connector         │
          │ (SQL, NoSQL, Search, Streaming, Cloud)   │
          └──────────────────────────────────────────┘
```

---

# 🧪 Example REST Query

```bash
curl -X GET "https://api.opendataledger.org/mysql/users?limit=10" \
  -H "Authorization: Bearer <token>" \
  -H "X-ODL-Encrypted: yes"
```

---

# 🔐 Example Encrypted Payload

```json
{
  "ciphertext": "a823bf901d2e…",
  "iv": "b39c12e91b2f…",
  "alg": "AES-256-GCM"
}
```

---

# 📦 Installation

```bash
git clone https://codeberg.org/opendataledger/opendataledger.git
cd opendataledger
./install.sh
```

---

# 📝 Roadmap

### Q1 2026
- Plugin marketplace  
- Full AI query optimizer  
- Terraform provider  

### Q2 2026
- Web3 distributed storage plugins  
- Time-travel queries  
- Post-quantum default mode  

### Q3 2026
- Multi-cluster replication  
- Cloud autoscaling toolkit  

### Q4 2026
- Encrypted analytics engine  
- Query cost predictor  

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/opendataledger/](https://roxanneardary.com/opendataledger/)

---

# 📄 License & Notice Requirements

**OpenDataLedger** is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- **OpenDataLedger** specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
---

# 🤝 Contributing

We welcome contributions—drivers, plugins, documentation, testing, integrations.

See: **CONTRIBUTING.md**

---

# 🏷 Project Status

**Alpha** — internal testing underway.  
**Beta** expected Q3 2026.
