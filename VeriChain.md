# VeriChain

**Proof in Every Link**

VeriChain is an open-source AI-powered truth verification system that evaluates claims by analyzing publicly available data, linking evidence, and producing probabilistic truth assessments with full transparency and explainability.

---

## Overview

VeriChain is designed to move beyond simple fact-checking by building a **structured evidence network** for every claim. Instead of returning a binary true/false result, it generates a **probability-based truth score**, supported by citations, reasoning, and contradiction analysis.

The system is fully open-source and intended to be self-hosted, auditable, and extensible.

---

## Core Principles

- No single source of truth — only weighted evidence  
- Uncertainty must always be visible  
- Every claim must be traceable to its origin  
- All outputs must be explainable and auditable  

---

## Full Feature List

### 1. Core Verification Engine
- Natural language claim parsing into atomic statements  
- Multi-source evidence aggregation  
- Cross-referencing across independent sources  
- Claim decomposition into verifiable components  
- Temporal validation of claims  
- Multi-language support  
- Context-aware interpretation (geography, law, time sensitivity)  

---

### 2. AI & Machine Learning Intelligence Layer

#### Semantic Understanding Engine
- Transformer-based NLP models  
- Named entity recognition  
- Semantic similarity matching  
- Multi-document summarization  
- Context disambiguation  

#### Adversarial Fact Testing
- Dual-model system:
  - Verifier model (supports claims with evidence)  
  - Attacker model (attempts to disprove claims)  
- Truth vs Attack competitive evaluation  
- Contradiction mining across sources  
- Adversarial resistance scoring  
- Strengthens confidence via structured challenge loops  

#### Uncertainty Modeling (Bayesian Layer)
- Probabilistic truth scoring instead of binary outputs  
- Bayesian updating with new evidence  
- Outputs:
  - Likelihood probability  
  - Confidence interval  
  - Stability score  
- Dynamic belief adjustment over time  

#### Hallucination Detection Layer
- Detects unsupported AI-generated statements  
- Separates outputs into:
  - Verified facts  
  - Inferred conclusions  
  - Model assumptions  
- Cross-checking against evidence graph  
- Citation consistency validation  

---

### 3. Truth Scoring System
- Probability-based scoring (0–100%)  
- Source credibility weighting  
- Contradiction penalties  
- Consensus modeling  
- Confidence intervals  
- Adjustable modes:
  - Strict  
  - Balanced  
  - Exploratory  

---

### 4. Evidence Linking System
- Claim-to-source evidence graph  
- Full citation traceability  
- Evidence clustering  
- Source reliability indicators  
- Persistent evidence chains  
- Direct document linking  
- Evidence strength scoring  

---

### 5. Knowledge Graph System
- Global graph of claims, entities, and sources  
- Relationship mapping  
- Time-versioned truth tracking  
- Queryable graph API  
- Authority ranking nodes  
- Contradiction networks  

---

### 6. Data Collection Layer
- Web crawling and indexing  
- Common Crawl integration  
- Academic sources (arXiv, PubMed)  
- Government records ingestion  
- News aggregation  
- Continuous update pipelines  
- Deduplication and clustering  

---

### 7. Explainability Engine
- Full reasoning breakdown per claim  
- Step-by-step inference trace  
- “Why this score” explanations  
- Evidence conflict visualization  
- Source contribution breakdown  
- Audit trail of decisions  

---

### 8. Logical Integrity System
- Internal contradiction detection  
- Logical consistency validation  
- Impossible claim detection  
- Cross-document coherence scoring  
- Dependency validation  

---

### 9. Distributed Verification Network
- Optional community-run nodes  
- Federated verification aggregation  
- Consensus-based scoring  
- Node reputation system  
- Decentralized validation layer  

---

### 10. Source Reputation System
- Dynamic trust scoring for domains and authors  
- Historical accuracy tracking  
- Misinformation propagation detection  
- Source lineage tracking  
- Reputation adjustment over time  

---

### 11. Visualization Layer
- Truth score dashboard  
- Evidence graph visualization  
- Supporting vs contradicting views  
- Confidence heatmaps  
- Truth timeline tracking  
- Layered “Truth Stack” view:
  - raw data  
  - interpreted data  
  - inference layer  
  - final score  

---

### 12. API & Developer Tools
- REST API for verification  
- Batch processing endpoints  
- Webhooks for real-time analysis  
- Python SDK support  
- JavaScript SDK support  
- Plugin system for external data sources  

---

### 13. System Architecture
- Modular microservices  
- Docker-based deployment  
- Scalable worker queues  
- Caching layer for repeated queries  
- Offline/self-hosted mode  
- Plugin-based extensions  

---

### 14. Security & Integrity
- Tamper-resistant audit logs  
- Dataset poisoning detection  
- Source authenticity validation  
- Model versioning and rollback  
- Transparent training logs  

---

### 15. Experimental Features
- Simulation-based verification models  
- Unknown truth detection (insufficient evidence flagging)  
- Counterfactual reasoning engine  
- Multi-hypothesis reasoning  
- Truth drift tracking over time  

---

### 16. Real-World Integration
- Browser extension for live verification  
- Social media claim scanning  
- News publisher API integration  
- Embeddable verification widgets  
- Real-time misinformation detection  

---

### 17. Governance & Open Source
- Licensed under AGPL-3.0+  
- Network-use copyleft enforcement  
- Public contribution tracking  
- Transparent dataset registry  
- Community-reviewed source inclusion  

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
  - [https://roxanneardary.com/verichain/](https://roxanneardary.com/verichain/)

---

## License & Notice Requirements

VeriChain is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- VeriChain specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Getting Started (Conceptual)

VeriChain is currently in early design phase. Planned components include:

- API server (FastAPI)  
- Evidence graph database (Neo4j or similar)  
- NLP inference pipeline (Hugging Face models)  
- Web interface (React + visualization layer)  

---

## Vision

VeriChain aims to become a **global open verification layer for information**, enabling anyone to trace claims back to their underlying evidence and understand not just what is “true,” but how and why it is considered true.

---
