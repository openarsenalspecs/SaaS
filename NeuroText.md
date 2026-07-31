# NeuroText

**Where chatting meets coding magic.**

NeuroText is an open source specification for building AI-powered applications entirely through messaging platforms. It provides a modular architecture that enables users to create, modify, test, and collaborate on software projects using natural language conversations across SMS, WhatsApp, iMessage, Signal, Telegram, Slack, Discord, and other messaging services.

The specification is platform-independent, AI-provider agnostic, and designed to support both cloud-hosted and self-hosted deployments.

Website: https://www.roxanneardary.com/

---

# Specification

NeuroText defines a standardized framework for conversational software development using AI. Rather than treating messaging platforms as simple communication tools, NeuroText transforms them into interactive development environments where users can design applications, generate code, manage projects, collaborate with teams, and automate workflows entirely through natural language.

The specification is designed around independent modules that communicate through well-defined interfaces, allowing developers to replace, extend, or customize individual components without affecting the overall system.

---

# Design Goals

- AI provider independent
- Messaging platform independent
- Modular architecture
- Local-first compatible
- Cloud deployment compatible
- Self-hosting friendly
- Extensible through plug-ins
- Privacy-first architecture
- Secure by default
- Human-in-the-loop workflows
- Multi-user collaboration
- Open standards
- Vendor neutral

---

# Core Modules

### Messaging Gateway

Provides a common interface for messaging platforms.

Features:

- SMS integration
- WhatsApp integration
- iMessage integration
- Signal integration
- Telegram integration
- Slack integration
- Discord integration
- Matrix integration
- IRC integration
- Web chat integration
- Incoming webhook support
- Outgoing webhook support
- Attachment handling
- Rich message formatting
- Conversation threading
- Session management

---

### AI Processing Engine

Responsible for interpreting user requests and coordinating AI operations.

Features:

- Natural language understanding
- Multi-model AI support
- Prompt management
- Context management
- Conversation memory
- Prompt optimization
- Code generation
- Content generation
- Documentation generation
- Project planning
- AI explanations
- AI tutoring
- Code optimization
- Refactoring assistance
- Error interpretation

---

### Project Builder

Creates and manages software projects.

Features:

- Application generation
- Script generation
- API generation
- Website generation
- Template generation
- Project scaffolding
- Modular project creation
- Project templates
- Configuration management
- File generation
- Asset organization

---

### Programming Engine

Provides language-aware development capabilities.

Features:

- Multi-language support
- Syntax validation
- Code formatting
- Static analysis
- Dependency management
- Package recommendations
- Framework templates
- Boilerplate generation

---

### Collaboration Engine

Coordinates multi-user development.

Features:

- Shared conversations
- Team collaboration
- AI-assisted merge recommendations
- Change tracking
- Contributor tracking
- Conflict detection
- Conflict resolution suggestions
- Project comments
- Review workflow

---

### Version Control Module

Provides repository integration.

Features:

- Git repository support
- GitLab integration
- GitHub integration
- Codeberg integration
- Commit generation
- Branch management
- Merge request support
- Repository synchronization

---

### Execution Engine

Safely executes generated projects.

Features:

- Secure sandbox execution
- Runtime monitoring
- Debugging assistance
- Error reporting
- Unit test generation
- Automated testing
- Output previews
- Log collection

---

### Documentation Engine

Automatically maintains project documentation.

Features:

- README generation
- API documentation
- Workflow documentation
- Architecture documentation
- Changelog generation
- Release notes
- User guides
- Technical documentation

---

### Automation Engine

Provides workflow automation.

Features:

- Scheduled tasks
- Project reminders
- Build automation
- Deployment preparation
- Notification routing
- Task management
- Feature tracking
- Workflow automation

---

### Security Module

Protects users and projects.

Features:

- Permission management
- Authentication integration
- Authorization controls
- Encryption support
- Secure messaging
- Data anonymization
- Audit logging
- Local AI support

---

### Accessibility Module

Improves usability.

Features:

- Voice-to-text
- Multi-language interface
- Prompt translation
- Mobile optimization
- Accessibility support
- Cross-platform compatibility

---

# Optional Plug-in Modules

The NeuroText specification supports optional plug-ins that extend the core platform without modifying the base implementation.

### Diagram Generator

- Flowchart generation
- UML generation
- Architecture diagrams
- Mind maps

### UI Designer

- Wireframe generation
- UI mockups
- Component previews
- Layout suggestions

### Database Designer

- Schema generation
- ER diagrams
- Migration planning
- Query generation

### Graphics Studio

- AI image generation
- Icon generation
- Illustration creation
- Asset management

### Voice Assistant

- Speech recognition
- Speech synthesis
- Voice commands
- Hands-free interaction

### Code Review Assistant

- Security analysis
- Performance analysis
- Best practice recommendations
- Style enforcement

### CI/CD Connector

- Build server integration
- Deployment pipelines
- Release automation
- Environment management

### API Connector Library

- Third-party integrations
- REST connectors
- GraphQL connectors
- Webhook libraries

### Knowledge Base

- Documentation indexing
- Semantic search
- Project knowledge graph
- Context retrieval

### Learning Assistant

- Interactive tutorials
- Coding lessons
- Project walkthroughs
- Skill tracking

### Analytics Dashboard

- Usage metrics
- Collaboration metrics
- AI performance metrics
- Project insights

### Marketplace

- Community plug-ins
- Template sharing
- Project starter kits
- Integration catalog

---

# Objectives

- Make software development conversational.
- Enable AI-powered collaboration from any messaging platform.
- Remove barriers between communication and development.
- Support every major AI provider.
- Support every major messaging platform.
- Encourage modular development.
- Preserve user privacy.
- Enable local-first deployments.
- Promote open standards.
- Build an extensible ecosystem through optional modules.  

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
  - [https://roxanneardary.com/neurotext/](https://roxanneardary.com/neurotext/)

---

## License & Notice Requirements

NeuroText is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- NeuroText specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
