# SubscriptionIndex

**Turn recurring charges into clear insight.**

SubscriptionIndex is a privacy-first, open-source AI system that detects, analyzes, and explains recurring subscriptions from bank and credit card statements. It helps users understand what they are subscribed to, what they are really paying for, and when and how those subscriptions renew—while protecting their data through end-to-end encryption.

---

## 🔐 Core Principles

- **End-to-End Encryption (E2EE) by default**
- **Zero-knowledge architecture** (servers cannot read user data)
- **Local-first AI processing**
- **User-controlled data ownership**
- **AGPL 3.0+ open-source licensing**

---

## 🧠 What SubscriptionIndex Does

SubscriptionIndex helps users:

- Detect hidden or forgotten subscriptions from financial statements
- Identify recurring billing patterns automatically
- Interpret subscription contracts and renewal terms
- Track cancellation rules and deadlines
- Prevent surprise renewals and auto-charges
- Maintain a clear registry of all active subscriptions

---

## ⚙️ Core Features

### 📥 Financial Data Import
- Upload bank statements (PDF, CSV, OFX)
- Analyze 2+ months of transaction history
- Extract merchant, amount, and date patterns

### 🔍 Subscription Detection
- Automatic recurring charge detection
- Merchant normalization (cleaning messy bank labels)
- Confidence scoring (high / medium / low likelihood)

### 🤖 AI Analysis (Local First)
- Subscription classification (streaming, SaaS, utilities, etc.)
- Pattern recognition for billing cycles
- Anomaly detection for irregular charges

### 📄 Contract Intelligence
- Upload or manually enter subscription terms
- Extract:
  - renewal dates
  - cancellation rules
  - contract length
  - auto-renew clauses

### ⚠️ User Awareness Layer
- Forces user confirmation of subscription terms
- Flags unknown or missing contract data
- Tracks cancellation requirements

### 🔔 Smart Alerts
- 30-day renewal reminders
- 14-day warning notifications
- 3-day urgent alerts
- Price change detection

### 🧾 Cancellation Tracking
- Step-by-step cancellation guidance
- Proof storage (screenshots, confirmations)
- Cancellation status tracking

### 🌍 Jurisdiction Awareness
- User-defined location (country/state)
- Consumer protection awareness layer
- Subscription law context summaries (informational only, not legal advice)

### 🔄 Cross-Device Sync (E2EE)
- End-to-end encrypted sync across devices
- Zero-knowledge server architecture
- Self-hosted or optional hosted sync
- Device authorization and revocation

### 👥 Household Support
- Multi-user profiles
- Shared subscription tracking
- Cost splitting and visibility

---

## 🔐 Security Model

- AES-256-GCM encryption for all sensitive data
- Argon2id key derivation
- Keys never leave user devices
- No plaintext storage on servers
- Optional encrypted backups and recovery phrase support

---

## ⚖️ Legal & Privacy

SubscriptionIndex is designed for transparency and user control, not legal enforcement.

- Jurisdiction-aware guidance is informational only
- No legal advice is provided
- Users remain responsible for their financial decisions

---

## 🧱 Architecture Overview

- **Frontend:** React / Next.js
- **Backend:** FastAPI (Python)
- **Database:** PostgreSQL (encrypted payload storage)
- **AI Layer:** Local LLM (Ollama / HuggingFace compatible)
- **Sync Layer:** Zero-knowledge encrypted API

---

## 🚀 Getting Started (Development)

> Coming soon: full setup instructions, Docker environment, and local development guide.

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
  - [https://roxanneardary.com/subscriptionindex/](https://roxanneardary.com/subscriptionindex/)

---


## 📜 License & Notice Requirements

SubscriptionIndex is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- SubscriptionIndex specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## 🤝 Contributing

We welcome contributions that improve:
- Subscription detection accuracy
- Privacy and encryption systems
- AI classification models
- UI/UX clarity
- Jurisdiction rule sets

All contributions must respect the AGPL 3.0+ license and privacy-first design principles.

---

## 🧠 Project Vision

SubscriptionIndex exists to eliminate hidden financial dependency traps by making every recurring charge understandable, transparent, and user-controlled.

---

## 📌 Name

**SubscriptionIndex**  
*Turn recurring charges into clear insight.*
