# CodeDrop Specification
**Your apps, on their merry way.**
- HTML Mirror:  [https://roxanneardary.com/codedrop-specification/](https://roxanneardary.com/codedrop-specification/)

---

## Vision

**CodeDrop** is an open-source executable transmission platform that makes software distribution as simple as sending a text message.

Instead of uploading files to cloud storage, attaching large email attachments, or directing users to download pages, CodeDrop allows applications to be securely packaged, transmitted, verified, and prepared for installation in a single workflow.

---

# Design Philosophy

Sending software should feel like sending a text message.

Instead of:

> Download → Upload → Share Link → Download Again → Install

CodeDrop becomes:

> Select → Send → Receive → Install

---

# Feature Specification

---

## Intelligent Packaging

CodeDrop automatically prepares software for transport.

Features include:

- Executable discovery
- Dependency detection
- Runtime analysis
- Shared library collection
- Configuration file detection
- Portable application support
- Package optimization
- Compression
- Package signing
- Metadata generation

---

## Package Manifest

Every package includes a signed manifest describing the contents before installation.

The manifest may include:

- Application name
- Package identifier
- Version
- Publisher
- Description
- Homepage
- License
- Build number
- Build date
- Package size
- Target operating systems
- Supported architectures
- Dependency list
- Installation type
- Required runtime
- Cryptographic checksums
- Digital signatures
- Release notes
- Optional screenshots
- Application icon

The manifest allows recipients to inspect software before installation.

---

## Trust Levels

Recipients control how software is accepted.

Trust options include:

- Trust once
- Always trust
- Never trust
- Ask every time
- Always sandbox
- Always verify signatures
- Organization managed trust
- Trusted publishers
- Trusted devices
- Revocable trust

---

## Secure Transmission

- End-to-end encryption
- Forward secrecy
- Ephemeral session keys
- Authenticated encryption
- Integrity verification
- Replay protection
- Tamper detection
- Package verification

---

## Addressing System

CodeDrop supports temporary addressing instead of permanent identities.

Supported methods include:

- One-time codes
- QR codes
- Peer IDs
- Public keys
- NFC pairing
- Local discovery
- Organization directories

No phone numbers or email addresses are required.

---

## Expiring Access

Senders choose how long packages remain available.

Examples:

- 5 minutes
- 15 minutes
- 30 minutes
- 1 hour
- 6 hours
- 12 hours
- 24 hours
- Custom expiration

Expired packages are automatically removed.

---

## Offline Relay

When recipients are unavailable, CodeDrop can temporarily relay encrypted packages.

Features:

- End-to-end encrypted storage
- Zero-knowledge relay
- Automatic deletion after download
- Automatic deletion after expiration
- Resume interrupted downloads
- One-time retrieval
- Delivery confirmation
- Optional self-hosted relays

Relay servers never possess decryption keys.

---

## Peer-to-Peer Networking

Supported transport methods include:

- LAN
- Internet
- Wi-Fi Direct
- Bluetooth
- WebRTC
- NAT traversal
- Relay fallback

Connections automatically select the fastest available route.

---

## Installation Modes

CodeDrop supports multiple installation options.

Examples:

- Install immediately
- Download only
- Portable mode
- Silent installation
- Sandbox installation
- Verify only
- Developer extraction

---

## Delta Updates

When recipients already possess an application:

- Detect installed version
- Compare package versions
- Transfer only changed files
- Reduce bandwidth usage
- Resume previous updates

---

## Transfer Engine

- Parallel transfers
- Chunked transmission
- Automatic resume
- Compression
- Encryption
- Integrity validation
- Duplicate elimination
- Adaptive bandwidth management

---

## User Experience

Designed for simplicity.

Features include:

- Drag-and-drop
- Progress indicators
- Transfer history
- Delivery notifications
- Installation notifications
- Countdown timers
- Package previews
- QR generation
- QR scanning
- Dark mode
- Accessibility support

---

## Security

CodeDrop is privacy-first.

Security features include:

- No telemetry by default
- No personal data transmission
- No advertising
- No trackers
- No analytics required
- Package verification
- Signature verification
- Trust management
- Secure deletion
- Cryptographic integrity

---

## Organization Support

Organizations can operate private CodeDrop environments.

Features include:

- Internal package repositories
- Software catalogs
- Department collections
- Organization relay servers
- Trusted publishers
- Organization trust policies
- Package approvals
- Version management
- Software deployment
- Internal updates
- Private networking
- Self-hosting
- Administrative controls
- Optional audit logging

Suitable for:

- Businesses
- Schools
- Universities
- Nonprofits
- Government agencies
- Development teams

---

## Developer API

CodeDrop provides an open API for integration.

Capabilities include:

- Package creation
- Package inspection
- Manifest generation
- Transmission initiation
- Progress monitoring
- Transfer cancellation
- Trust management
- Relay management
- Verification
- Signature generation
- Package signing
- Installation events
- Delivery events
- Notification events

Possible integrations:

- IDEs
- Build systems
- CI/CD platforms
- Package managers
- Enterprise deployment tools
- Desktop applications
- Mobile applications
- Automation platforms

---

# Guiding Principles

Every feature should satisfy one or more of the following:

- Faster
- Simpler
- More secure
- More private
- More transparent
- Easier to self-host
- Easier to integrate
- Easier to audit

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
  - [https://roxanneardary.com/codedrop/](https://roxanneardary.com/codedrop/)

---

## License & Notice Requirements

CodeDrop is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- CodeDrop specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
