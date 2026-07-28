# Sentryx

**Data protection, simplified.**

Sentryx is a fully open-source, cloud-based backup and data protection system designed for secure storage, resilient infrastructure, and privacy-first architecture. It provides encrypted backups, distributed storage, authentication security, and optional AI-assisted intelligence in a modular, scalable design.

Sentryx is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)** and is developed transparently on GitLab.

---

## Core Vision

Sentryx is built on a simple principle:

**Users should fully own, control, and understand their data without sacrificing usability or scalability.**

It supports three deployment models:
- Personal encrypted backup system
- Federated distributed storage network
- Enterprise-grade secure infrastructure platform

---

## Feature Overview (Modular Architecture)

Sentryx is designed as a collection of independent modules that can scale, extend, or be replaced without affecting the core system.

---

## 1. Core Backup Engine
- Incremental backups (change-based storage)
- Full snapshot backups
- Deduplication engine
- Compression pipeline
- Versioned restore points
- Scheduled and manual backups
- File change detection system
- Include/exclude rules for granular control
- Cross-platform client support (Linux, Windows, macOS)

---

## 2. Encryption & Key Management
- End-to-end client-side encryption (zero-knowledge architecture)
- AES-256 or equivalent encryption standards
- Per-backup encryption keys
- Key rotation system (manual + automated)
- Secure passphrase-based key derivation
- Optional hardware-backed key storage (TPM / Secure Enclave)
- Encrypted metadata support (optional file name encryption)
- Server-side inability to decrypt data

---

## 3. Storage Backend
- S3-compatible object storage support
- Self-hosted storage option (MinIO or equivalent)
- Multi-node distributed storage
- Erasure coding for redundancy
- Cross-region replication support
- Tiered storage (hot / warm / cold)
- Immutable storage mode (WORM protection)
- Retention and lifecycle policies
- Storage quotas per user or organization

---

## 4. Client Agent
- Lightweight background service
- CLI and optional GUI client
- Local encryption before upload
- Offline backup queue system
- Bandwidth throttling controls
- Battery-aware scheduling
- Multi-device synchronization
- Guided restore workflow

---

## 5. Authentication & Identity
- OAuth2 / OpenID Connect support
- Role-Based Access Control (RBAC)
- Multi-tenant organization support
- Two-Factor Authentication (TOTP)
- Device authorization system
- Session tracking and revocation
- Login anomaly detection hooks
- Fine-grained permission system

---

## 6. API Gateway
- RESTful API (primary interface)
- Optional GraphQL support
- Rate limiting and abuse protection
- API key management
- Versioned endpoints
- Webhook event system
- Full audit logging

---

## 7. Web Dashboard
- Backup timeline viewer
- One-click restore interface
- Storage usage analytics
- Device management panel
- Security settings dashboard
- Audit log viewer
- Role and permission management UI
- Multi-organization support

---

## 8. Monitoring & Observability
- Backup success/failure tracking
- Real-time system metrics
- Prometheus-compatible export
- Grafana dashboard integration
- Centralized logging system
- Alerting system (webhook/email)
- System anomaly detection hooks

---

## 9. Scheduling & Automation
- Cron-based scheduling engine
- Event-driven backup triggers
- Automatic retry system
- Retention policy automation
- Load-aware scheduling
- Multi-device sync coordination

---

## 10. Disaster Recovery
- Full system restore workflows
- Partial file restoration
- Cross-device restore capability
- Backup integrity verification (hash validation)
- Multi-node redundancy failover
- Offline restore capability
- Secure key recovery system
- Snapshot rollback system

---

## 11. Security & Hardening
- Zero-trust architecture
- Immutable backup mode (ransomware resistance)
- Intrusion detection integration hooks
- IP allow/deny listing
- Optional geo-restriction policies
- Tamper-resistant audit logs
- Automatic session invalidation on suspicious activity

---

## 12. Deployment & Infrastructure
- Docker / Podman support
- Kubernetes-ready deployment
- Horizontal scaling architecture
- CI/CD integration (GitLab CI)
- Infrastructure-as-code compatibility
- Hybrid or fully self-hosted deployment options
- Environment-based configuration system

---

## 13. Plugin & Extension System
- Modular plugin architecture
- External storage integrations
- Custom encryption modules
- Notification system extensions
- UI customization system
- Authentication extensions
- Event hook system (pre/post backup operations)

---

## 14. AI-Assisted Backup Intelligence
- Smart backup prioritization
- Behavioral scheduling optimization
- Ransomware/anomaly detection system
- Natural language restore queries
- Predictive backup optimization
- Local-first AI processing (optional, no cloud dependency)
- File importance detection engine

---

## 15. Storage Optimization & Efficiency
- Adaptive deduplication engine
- Delta-based storage for large files
- Automatic cold storage migration
- Intelligent backup pruning system
- Bandwidth-aware synchronization
- Predictive compression selection
- Storage footprint analytics dashboard

---

## 16. High-Assurance Enterprise Features
- Multi-region failover clusters
- SLA-backed backup guarantees
- Compliance-ready operating modes
- Immutable forensic logging
- Hardware Security Module (HSM) support
- Air-gapped master key architecture
- Enterprise RBAC + policy engine
- Disaster recovery orchestration system
- Audit export and compliance reporting tools

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
  - [https://roxanneardary.com/sentryx/](https://roxanneardary.com/sentryx/)  

---

## License & Notice Requirements

Sentryx is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Sentryx specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Final Note

Sentryx is designed to be more than a backup tool—it is a **modular, secure, and scalable data protection infrastructure** built for individuals, organizations, and distributed systems that require full control over their data.
