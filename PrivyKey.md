# PrivyKey

**The Open Way to Safe Logins**

PrivyKey is a fully open-source, privacy-first authentication specification designed to provide secure, user-controlled identity verification through encrypted key management and modular authentication services.

PrivyKey replaces closed authentication ecosystems with a transparent, auditable, and extensible framework where users maintain ownership of their authentication secrets. Built around local-first security, zero-knowledge principles, and strong cryptographic protection, PrivyKey provides a foundation for secure 2FA authentication while allowing future expansion into broader identity and credential management systems.

---

# Specification Overview

PrivyKey defines a modular authentication architecture consisting of independent security components. Each core module performs a dedicated function while maintaining strict separation between user interfaces, application logic, cryptographic operations, storage systems, and external integrations.

The modular approach ensures that security improvements, platform expansions, and future authentication standards can be integrated without requiring a complete system redesign.

---

# Core Modules

## Authentication Engine Module

The Authentication Engine provides the foundation for secure login verification.

Features:
- TOTP authentication support compliant with RFC 6238
- HOTP compatibility compliant with RFC 4226
- Secure one-time code generation
- Time synchronization handling
- Configurable authentication intervals
- Multi-account authentication support
- Offline authentication capability
- Secure verification workflows

---

## Cryptography Core Module

The Cryptography Core provides all security-critical cryptographic operations.

Features:
- Strong encryption algorithms
- AES-256-GCM encryption support
- ChaCha20-Poly1305 encryption support
- Argon2id password-based key derivation
- Secure random number generation
- Cryptographic key management
- Secure memory handling
- Sensitive data zeroization
- Versioned encryption format support

The Cryptography Core is isolated from user interface components to prevent unauthorized access to sensitive authentication data.

---

## Secure Vault Module

The Secure Vault Module manages encrypted storage of authentication credentials.

Features:
- Encrypted local credential storage
- Zero plaintext secret storage
- Secure account organization
- Encrypted metadata storage
- Vault locking and unlocking
- Automatic timeout protection
- Secure deletion and cryptographic wiping
- Encrypted import and export capabilities

---

## Key Management Module

The Key Management Module controls creation, storage, and lifecycle management of authentication keys.

Features:
- Device-generated authentication secrets
- Unique key generation per account
- Secure key rotation support
- Key ownership tracking
- Key recovery workflows
- Hardware-backed key storage support when available
- Protection against unauthorized extraction

---

## QR Provisioning Module

The QR Provisioning Module enables secure account setup and migration.

Features:
- QR code scanning
- QR code generation
- Standard `otpauth://` URI compatibility
- Secure provisioning validation
- Account metadata extraction
- Protected secret import workflow

---

## User Interface Module

The User Interface Module provides user interaction while maintaining strict security boundaries.

Features:
- Account dashboard
- Authentication code display
- Countdown timers
- Vault management interface
- Secure setup workflows
- Accessibility support
- Platform-native user experiences

The UI layer never directly manages raw cryptographic secrets.

---

## Backup and Recovery Module

The Backup and Recovery Module provides secure methods for restoring authentication access.

Features:
- Encrypted backup creation
- Encrypted backup restoration
- Offline recovery options
- User-controlled backup ownership
- Recovery verification workflows
- Migration between trusted devices

---

## Security Monitoring Module

The Security Monitoring Module provides transparency and protection against misuse.

Features:
- Security event tracking
- Local encrypted audit records
- Failed authentication monitoring
- Suspicious activity detection
- Integrity verification
- Security health checks

---

# Optional Plugin Modules

PrivyKey supports optional plug-in modules that extend functionality without modifying the secure core architecture.

---

## WebAuthn / FIDO2 Plugin Module

Adds modern passwordless authentication capabilities.

Features:
- Hardware security key support
- Passkey integration
- Browser authentication support
- Phishing-resistant authentication

---

## Hardware Security Plugin Module

Provides integration with external security devices.

Features:
- Hardware token support
- Secure element integration
- Smart card compatibility
- External cryptographic device support

---

## Encrypted Synchronization Plugin Module

Provides optional multi-device synchronization.

Features:
- End-to-end encrypted synchronization
- Zero-knowledge server architecture
- Self-hosted synchronization support
- Encrypted vault replication
- User-controlled sync infrastructure

---

## Enterprise Policy Plugin Module

Adds organizational security controls.

Features:
- Organization authentication policies
- Required 2FA enforcement
- Device approval workflows
- Security compliance reporting
- Administrative controls

---

## Identity Credential Plugin Module

Expands PrivyKey beyond traditional authentication.

Features:
- Digital identity credentials
- Verifiable credential support
- Decentralized identity integrations
- Secure identity storage

---

## Post-Quantum Security Plugin Module

Provides future cryptographic upgrade paths.

Features:
- Post-quantum cryptography experiments
- Algorithm migration support
- Hybrid cryptographic modes
- Future-proof security upgrades

---

# Architecture Principles

PrivyKey follows these core principles:

## User Ownership
Authentication secrets belong to the user and remain under user control.

## Zero-Knowledge Security
Systems storing encrypted data should never have access to plaintext authentication secrets.

## Modular Security
Every security component should be independently replaceable and auditable.

## Open Standards
PrivyKey uses publicly documented authentication and cryptographic standards.

## Privacy by Design
No tracking, hidden telemetry, or unnecessary data collection.

---

# Technology Foundation

PrivyKey is designed around:

- Kotlin and Jetpack Compose for Android
- Swift and SwiftUI for iOS
- libsodium cryptographic libraries
- Argon2id key derivation
- AES-256-GCM and ChaCha20-Poly1305 encryption
- SQLCipher encrypted storage
- RFC-compliant authentication protocols
- Reproducible builds and security auditing workflows

---

# Future Vision

PrivyKey is designed to evolve from a secure authenticator into a broader open identity security platform.

Future possibilities include:

- Passwordless authentication
- Decentralized identity systems
- Secure credential wallets
- Hardware-backed authentication ecosystems
- Encrypted personal identity infrastructure

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
  - [https://roxanneardary.com/privykey/](https://roxanneardary.com/privykey/)

---

## 🧾 License & Notice Requirements

PrivyKey is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PrivyKey specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
