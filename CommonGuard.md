# CommonGuard
**Eyes Wide Open. Detect. Flag. Enforce.**  
- HTML Mirror:  [https://roxanneardary.com/commonguard-specification/](https://roxanneardary.com/commonguard-specification/)

---

CommonGuard is an open-source AI trademark intelligence and enforcement platform that continuously monitors the web for potential trademark misuse, brand impersonation, counterfeit activity, and unauthorized commercial use. Designed with a modular architecture, CommonGuard combines AI-powered detection, evidence collection, human review, and enforcement workflows into a single extensible platform that organizations, legal teams, investigators, and open-source communities can deploy on their own infrastructure.

Rather than making legal determinations, CommonGuard assists investigators by identifying potential violations, collecting evidence, prioritizing cases through risk scoring, and streamlining enforcement workflows while maintaining human oversight throughout the review process.

---

## Design Goals

- Open-source and self-hosted
- Privacy-first architecture
- AI-assisted, human-reviewed enforcement
- Modular plugin architecture
- Vendor neutral
- API-first design
- Distributed monitoring
- Enterprise scalable
- Multi-jurisdiction support
- Fully auditable workflows

---

## Core Modules

### Search Intelligence Module

Monitors search engines for trademark and brand usage.

Features:

- Search engine monitoring
- Trademark keyword tracking
- Search result collection
- SERP history
- Ranking change monitoring
- Advertisement monitoring
- Search result archiving
- Metadata collection

---

### Website Intelligence Module

Analyzes websites that reference monitored trademarks.

Features:

- Full website crawling
- Header analysis
- Title analysis
- Meta description analysis
- Structured data extraction
- URL analysis
- Domain relationship mapping
- Technology fingerprinting
- Content snapshots

---

### Brand Detection Module

Detects textual references to brands and trademarks.

Features:

- Trademark recognition
- Company name recognition
- Product name recognition
- Service name detection
- Brand variation detection
- Misspelling detection
- Typo-squatting detection
- Keyword expansion
- Language normalization

---

### Image Intelligence Module

Analyzes visual assets for brand misuse.

Features:

- Logo detection
- Similar logo recognition
- Watermark detection
- Product image comparison
- AI-generated image detection
- Reverse image lookup support
- OCR text extraction
- Image similarity analysis

---

### AI Analysis Module

Provides intelligent evaluation of collected evidence.

Features:

- Risk scoring
- Pattern recognition
- Similarity analysis
- Historical comparison
- Behavioral analysis
- Repeat offender detection
- Confidence scoring
- Context analysis
- AI-generated summaries

---

### Evidence Management Module

Collects and preserves investigation evidence.

Features:

- Screenshots
- HTML snapshots
- PDF generation
- Timestamp recording
- Hash verification
- Evidence storage
- Chain of custody
- Audit logging
- Case attachments

---

### Investigation Module

Centralized case management.

Features:

- Investigation workspaces
- Case creation
- Investigator assignments
- Internal notes
- Evidence review
- Priority management
- Status tracking
- Case timelines
- Resolution history

---

### Human Review Module

Ensures AI findings receive human validation.

Features:

- Review queues
- Approval workflow
- False positive handling
- Reviewer comments
- Multi-review approval
- Escalation workflow
- Confidence verification
- Decision history

---

### Enforcement Module

Assists with enforcement activities.

Features:

- Takedown preparation
- Trademark complaint generation
- Evidence packages
- Enforcement tracking
- Repeat violation monitoring
- Resolution tracking
- Escalation management
- Reporting history

---

### Notification Module

Keeps investigators informed.

Features:

- Email alerts
- Webhooks
- SMS support
- Desktop notifications
- Slack integration
- Microsoft Teams integration
- Daily summaries
- Critical alert escalation

---

### Dashboard Module

Provides centralized visibility.

Features:

- Live monitoring dashboard
- Risk heat maps
- Investigation metrics
- Enforcement statistics
- Trend analysis
- Repeat offender reports
- Investigator workload
- Activity timeline

---

### Security Module

Protects investigation data.

Features:

- Role-based permissions
- Multi-factor authentication
- API authentication
- Audit logging
- Encryption
- Session management
- Access policies
- Secure evidence storage

---

## Optional Plugin Modules

CommonGuard supports an extensible plugin ecosystem.

### Marketplace Monitor

Monitor marketplaces including:

- Amazon
- eBay
- Etsy
- Walmart Marketplace
- Alibaba
- AliExpress
- Mercari
- Facebook Marketplace

---

### Social Media Monitor

Monitor brand usage across:

- X
- Facebook
- Instagram
- TikTok
- LinkedIn
- Reddit
- YouTube
- Pinterest

---

### Domain Watch Plugin

- New domain registrations
- Whois monitoring
- DNS analysis
- Certificate monitoring
- Domain ownership changes
- Domain reputation

---

### Counterfeit Detection Plugin

- Counterfeit product detection
- Seller analysis
- Marketplace intelligence
- Product comparison
- Packaging comparison
- Listing similarity

---

### Reseller Verification Plugin

- Authorized reseller database
- Dealer verification
- Distributor validation
- Partner verification
- Affiliate monitoring

---

### AI Impersonation Plugin

Detects AI-generated brand abuse.

Features:

- AI-generated websites
- Fake support portals
- Brand impersonation
- Deepfake branding
- Synthetic marketing content
- AI phishing campaigns

---

### Copyright Monitoring Plugin

- Copyright detection
- Content duplication
- Image theft
- Document monitoring
- Website copying
- Publication tracking

---

### Patent Monitoring Plugin

- Patent references
- Technology claims
- Patent citation monitoring
- Patent misuse detection

---

### Geographic Intelligence Plugin

- Country analysis
- Regional enforcement
- Jurisdiction mapping
- Geographic heat maps
- Cross-border activity

---

### Threat Intelligence Plugin

- Known bad actors
- Blacklists
- Watchlists
- Fraud indicators
- Threat feeds
- Reputation scoring

---

### Blockchain Evidence Plugin

- Evidence hashing
- Timestamp verification
- Immutable audit trail
- Chain-of-custody verification

---

### API Integration Plugin

Connect CommonGuard with:

- CRM systems
- Legal software
- Ticketing systems
- SIEM platforms
- Case management software
- Internal APIs

---

### Reporting Plugin

Generate:

- Investigation reports
- Executive summaries
- Enforcement statistics
- Compliance reports
- Audit reports
- PDF exports
- CSV exports

---

## Future Modules

- Trademark registration database integration
- International trademark verification
- Customs enforcement integration
- Mobile investigation application
- Browser investigation extension
- AI legal research assistant
- Court filing assistant
- Collaborative investigation network
- Federated investigation nodes
- Public transparency portal

---

## Technology Stack

Backend

- Python
- FastAPI

Database

- PostgreSQL
- Redis

AI

- Large Language Models
- Hugging Face
- Local AI support
- Computer Vision

Frontend

- React
- TypeScript

Monitoring

- Playwright
- Scrapy

Deployment

- Docker
- Kubernetes
- Linux
- Windows
- macOS

---

## Project Principles

- AI assists but does not make legal decisions.
- Human review is required before enforcement.
- Evidence should be verifiable and auditable.
- Organizations maintain ownership of their own data.
- Modular architecture enables community extensions.
- Open standards encourage interoperability.
- AGPL-3.0+ ensures improvements remain open.

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
  - [https://roxanneardary.com/commonguard/](https://roxanneardary.com/commonguard/)

---

## License & Notice Requirements

CommonGuard is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- CommonGuard specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.  
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
