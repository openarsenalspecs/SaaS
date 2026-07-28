# MeshCore

**Privacy-first infrastructure for identity.**

MeshCore is a modular, open-source identity and security system designed to manage passwords, credentials, API keys, secure notes, and digital identity data across devices. It is built as a **distributed identity framework**, not just a password manager.

It is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.

---

## 🔐 Overview

MeshCore transforms identity management into a **connected, encrypted system layer** that works across:

- Mobile (iOS / Android / iPadOS)
- Desktop (Windows / macOS / Linux)
- Browser extensions (autofill system)
- Self-hosted sync environments

Instead of storing credentials in isolated vaults, MeshCore organizes them into a **secure identity graph** linking passwords, tokens, notes, and identity records.

---

## 🧩 Core Architecture

MeshCore is fully modular, with independent components that can evolve separately.

### 🔐 Vault Core (Security Engine)
- Master password–derived encryption keys (Argon2id)
- End-to-end encrypted vault storage
- Zero-knowledge design (no plaintext storage of master secrets)
- Portable encrypted vault format
- Shared cryptographic layer across all platforms

---

### 🗂 Identity Store Module
- Website credentials (username/password pairs)
- API keys and developer tokens
- Secure notes and recovery codes
- Identity documents (encrypted references)
- Tagging, indexing, and search system
- Relational linking between identity entries

---

### 🤖 Autofill Engine
- Browser form detection
- URL + context-based credential matching
- Multi-account handling per site
- Multi-step login flow support
- Cross-platform autofill compatibility (browser, desktop, mobile)

---

### 🧠 Intelligence Layer
A local-first analytics and security enhancement system:

#### 📊 Password Health Dashboard
- Weak password detection
- Reused credential detection
- Unused account tracking
- Risk scoring per identity entry

#### 🔍 Breach Awareness (Opt-In)
- Detects compromised credentials using privacy-preserving methods
- Flags exposed accounts locally
- Fully optional and encrypted

#### 📈 Usage Intelligence
- Tracks local usage patterns
- Identifies frequently used credentials
- Improves autofill prioritization

#### ⚡ Smart Recommendations
- Password upgrade suggestions
- Duplicate account detection
- Security improvement insights

---

### 🌉 Bridge Layer
- Secure local API (Rust/Go)
- Browser extension communication bridge
- Desktop ↔ mobile messaging system
- Plugin communication interface

---

### 🔄 Sync Module (Optional)
- End-to-end encrypted synchronization
- Self-hosted server support (AGPL-compliant)
- Peer-to-peer or LAN sync options
- Conflict resolution system
- No plaintext data ever transmitted

---

### 🪪 Identity Expansion Module
Extends MeshCore beyond passwords into full identity management:

#### 🧾 Secure Identity Vault
- Government IDs (encrypted storage)
- Memberships and licenses
- Software license keys
- Recovery credentials

#### 🔐 API & Token Vault
- API keys
- OAuth tokens
- SSH key references
- Developer credentials

#### 🧠 Secure Notes System
- Encrypted notes tied to identities
- Tagging and search functionality
- Optional expiration/self-destruct rules

#### 🔗 Identity Graph System
- Links credentials, notes, and tokens together
- Creates relational identity structures
- Enables cross-service identity mapping

#### 📦 Portable Identity Export
- Encrypted export bundles
- Partial or full identity exports
- Cross-device import support

---

## ⚙️ Technology Stack

### Core Engine
- Rust (preferred) or Go
- libsodium
- Argon2id
- XChaCha20-Poly1305 encryption

---

### Desktop Application
- Tauri (preferred) or Electron
- React or Svelte UI
- Encrypted local storage
- System tray integration

---

### Mobile Application
- Flutter (cross-platform)
- iOS Keychain / Android Keystore
- Biometric authentication (Face ID / fingerprint)
- Offline-first design

---

### Browser Extension
- WebExtension API (Chrome / Firefox / Edge)
- TypeScript implementation
- Secure bridge communication
- No local credential storage

---

### Sync Infrastructure
- Self-hosted encrypted server (AGPL required)
- Optional WebDAV compatibility
- Peer-to-peer sync capability

---

### Bridge API
- Local encrypted API server
- WebSocket secure channel support
- Native messaging bridge for browser integration

---

## 🧩 Plugin System
MeshCore supports extensibility through plugins:

- Autofill behavior plugins
- Storage backend plugins
- Authentication method plugins
- UI and theme extensions
- Intelligence Layer extensions
- Sync provider modules

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
  - [https://roxanneardary.com/meshcore/](https://roxanneardary.com/meshcore/)

---

## 📜 License & Notice Requirements

MeshCore is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- MeshCore specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request. 
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## 🚀 Project Vision

MeshCore is not just a password manager.

It is a:

> **Privacy-first infrastructure for identity**

A modular, encrypted, self-hostable system that unifies credentials, authentication, and digital identity into a single secure graph across all devices.

---

## 📁 Repository Structure

- `/core-vault`
- `/identity-store`
- `/autofill-engine`
- `/intelligence-layer`
- `/bridge-api`
- `/sync-server`
- `/desktop-app`
- `/mobile-app`
- `/browser-extension`
- `/plugins`
- `/docs`

---

## 🤝 Contributing

Contributions are welcome under the AGPL 3.0+ license terms.  
Please ensure all changes align with the modular architecture and maintain security-first design principles.

---

## 📄 License

This project is licensed under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
