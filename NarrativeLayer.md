# NarrativeLayer

**Organizing the flow of information.**

---

## Overview

NarrativeLayer is an open-source, modular information structuring system that transforms RSS feeds into synchronized content and discussion environments.

It provides a pure-source feed architecture where one authoritative account controls the information stream. Incoming RSS content is preserved as the canonical source while NarrativeLayer adds structured views, AI enrichment, discussion capabilities, information intelligence, archival preservation, and knowledge extraction layers.

NarrativeLayer presents information through two synchronized experiences:

- **RSS View** — a traditional chronological feed preserving source integrity
- **Forum View** — a discussion-driven interface where posts become threads and rise based on engagement and activity

Both views operate from the same underlying data model, ensuring comments, timestamps, and content state remain consistent.

---

# Design Principles

NarrativeLayer is built around the following principles:

- **Pure Source Model** — one authoritative source account dictates the feed
- **Single Source of Truth** — all views operate from shared data
- **Timestamp Integrity** — dates and times remain immutable and synchronized
- **Modular Architecture** — features are separated into independent components
- **Open Extensibility** — additional capabilities can be added through plugins
- **Information Preservation** — content history remains available over time
- **Knowledge Evolution** — discussions can become structured knowledge

---

# Core Architecture

NarrativeLayer is composed of core modules that provide the foundational system functionality.

---

# Core Modules

## Source Feed Module

The Source Feed Module manages the authoritative information stream.

Features:

- RSS feed ingestion
- Pure-source account management
- Feed validation
- Content normalization
- Source metadata preservation
- Canonical content storage
- Source identity tracking

---

## Content Processing Module

The Content Processing Module transforms raw RSS entries into structured information objects.

Features:

- RSS item normalization
- Original title preservation
- Content extraction
- Metadata management
- Thread seed creation
- Source relationship tracking
- Content structure preparation

---

## AI Enrichment Module

The AI Enrichment Module provides intelligent content structuring.

Features:

- One-sentence AI-generated thread titles
- Neutral content descriptions
- AI-generated thread summaries
- Context extraction
- Discussion summarization
- Narrative evolution tracking

---

## Thread Management Module

The Thread Management Module converts RSS entries into structured discussions.

Features:

- RSS-to-thread conversion
- Thread lifecycle management
- Shared thread state
- Comment association
- Thread linking
- Discussion history preservation
- Thread relationship management

---

## Comment System Module

The Comment System Module provides unified discussion capabilities.

Features:

- Single comment storage model
- Shared comments across RSS and Forum views
- User discussions
- Comment timestamps
- Reply structures
- Thread activity tracking

---

## View Rendering Module

The View Rendering Module provides synchronized user experiences.

Features:

### RSS View

- Chronological feed display
- Original source titles
- Published date ordering
- Traditional RSS behavior

### Forum View

- Thread-based display
- AI-generated titles
- Engagement-based ordering
- Comment visibility
- Discussion-focused presentation

---

## Ranking and Attention Module

The Ranking and Attention Module determines information visibility.

Features:

- Comment-based ranking
- Activity scoring
- Engagement measurement
- Attention velocity tracking
- Rising discussion detection
- Thread activity states

Thread states include:

- Breaking
- Rising
- Stable
- Fading

---

## Information Integrity Module

The Information Integrity Module maintains trust and transparency.

Features:

- Duplicate story detection
- Related story linking
- Update chain tracking
- Contradiction detection
- Source comparison
- Historical relationship preservation

---

## Semantic Search Module

The Semantic Search Module enables meaning-based discovery.

Features:

- Concept-based search
- Related thread discovery
- Cross-source exploration
- Narrative relationship discovery
- Topic-based retrieval
- Knowledge discovery

---

## Time Integrity Module

The Time Integrity Module ensures consistent chronological data.

Features:

- Immutable publication timestamps
- Immutable comment creation timestamps
- Shared timestamps across views
- Consistent event ordering
- Timeline preservation

---

## Content Archive Module

The Content Archive Module preserves the historical integrity of information within NarrativeLayer.

It creates a permanent record of source content, thread evolution, and discussion history while maintaining the original context of each information item.

Features:

- Immutable content snapshots
- Historical thread versions
- Original source preservation
- Publication history tracking
- Deleted or modified source archiving
- Content restoration support
- Archive search capabilities
- Historical comparison between versions

Purpose:

The Content Archive Module ensures that information remains available and traceable even when external sources change, disappear, or modify their original content.

Every narrative maintains a historical record of how it developed over time.

---

## Knowledge Extraction Module

The Knowledge Extraction Module transforms discussions and information streams into structured knowledge resources.

It identifies valuable information patterns from posts, comments, summaries, and linked sources.

Features:

- Key point extraction
- Recurring theme identification
- FAQ generation
- Knowledge summary creation
- Important discussion extraction
- Topic relationship discovery
- Structured knowledge entry generation
- Conversion of discussions into reusable references

Purpose:

The Knowledge Extraction Module allows NarrativeLayer to evolve from a discussion platform into a living knowledge system.

Information is not only consumed and discussed—it can be preserved, organized, and reused as structured knowledge.

---

# Optional Plugin Modules

NarrativeLayer supports optional plugins that extend functionality without changing the core system.

---

## Advanced AI Models Plugin

Features:

- Local AI model support
- Custom summarization models
- Custom prompt pipelines
- Specialized analysis models

---

## Topic Intelligence Plugin

Features:

- Topic clustering
- Topic pages
- Trend grouping
- Related topic discovery
- Topic evolution tracking

---

## Narrative Graph Plugin

Features:

- Thread relationship graphs
- Source relationship maps
- Topic networks
- Information flow visualization

---

## Perspective Analysis Plugin

Features:

- Argument extraction
- Consensus detection
- Disagreement mapping
- Multiple perspective summaries

---

## Source Reputation Plugin

Features:

- Source history tracking
- Community reputation scoring
- Source comparison
- Reliability metadata

---

## User Personalization Plugin

Features:

- Followed topics
- Saved threads
- Custom feed preferences
- Reading history
- Personalized discovery

---

## Notification Plugin

Features:

- Rising thread alerts
- New comment notifications
- Topic monitoring
- Source update notifications

---

## API Integration Plugin

Features:

- External API access
- Webhooks
- Data exports
- Third-party integrations

---

# Data Model

NarrativeLayer maintains a unified information model.

Core objects include:

- Source
- Feed
- Post
- Thread
- Comment
- Summary
- Archive Record
- Knowledge Entry
- Relationship
- Timeline Event
- Attention State

All modules operate on shared objects to prevent duplication and synchronization conflicts.

---

# System Philosophy

NarrativeLayer is designed to organize information without replacing the original source.

The system separates:

- source truth
- structured presentation
- discussion
- AI assistance
- historical preservation
- knowledge extraction
- information discovery

The result is a layered information environment where content can evolve while maintaining historical accuracy and source integrity.

---

# Information Lifecycle

NarrativeLayer follows a complete information lifecycle:

**Source → Structure → Discuss → Archive → Extract Knowledge → Discover**  

---

# Tagline

**Organizing the flow of information.**

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
  - [https://roxanneardary.com/narrativelayer/](https://roxanneardary.com/narrativelayer/)

---


## License & Notice Requirements

NarrativeLayer is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- NarrativeLayer specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain attribution requirements where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
