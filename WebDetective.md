# WebDetective
**Follow the Trail. Discover the Strategy.**
- HTML Mirror:  [https://roxanneardary.com/webdetective-specification/](https://roxanneardary.com/webdetective-specification/)  

---

## Multi Agent Website Research and Intelligence Specification

WebDetective is a modular, multi-agent website research and intelligence specification for discovering, archiving, analyzing, and understanding websites and their broader search presence. It combines specialized research agents, search-engine-specific intelligence, comprehensive website discovery, page archival, backlink analysis, keyword intelligence, content analysis, technical SEO analysis, and SEO strategy reconstruction into a unified research system.

WebDetective is designed to investigate a website from multiple perspectives simultaneously. Each agent specializes in a defined research function while the Research Coordinator combines their findings into a structured evidence-based research dataset.

## Design Principles

- Multi-agent architecture
- Modular design
- Search-engine-specific specialization
- Comprehensive website discovery
- Evidence-based research
- Full-page archival
- Reproducible research
- Structured provenance
- Search-engine diversity
- Vendor-neutral architecture
- Local-first operation where practical
- Human-in-the-loop research
- Extensible plugin architecture
- Historical research
- Observable evidence over unsupported assumptions
- Separation of observations, patterns, techniques, strategies, and inferences
- Respect for applicable access restrictions and responsible crawling practices

---

## Core Modules

### Research Coordinator Module

The Research Coordinator manages the overall research operation.

Features include:

- Research objective intake
- Website and domain intake
- Research plan generation
- Agent selection
- Agent task delegation
- Parallel task execution
- Sequential task execution
- Task prioritization
- Research queue management
- Agent result aggregation
- Result reconciliation
- Conflict detection
- Research gap detection
- Coverage monitoring
- Automatic follow-up research
- Research session management
- Research session resumption
- Research session history
- Human review checkpoints
- Final research dataset generation
- Research report generation

### Search Engine Intelligence Module

The Search Engine Intelligence Module provides the common interface for independent search-engine agents.

Features include:

- Search abstraction
- Native query translation
- Search capability detection
- Search operator management
- Query validation
- Query generation
- Query expansion
- Query decomposition
- Query chaining
- Result normalization
- Result classification
- Result deduplication
- Result clustering
- Search-result metadata extraction
- Search-result evidence capture
- Search-engine comparison
- Search-engine behavior tracking
- Search-engine version tracking

Each search engine should have its own specialized module containing detailed knowledge of that engine's commands, operators, syntax, filters, capabilities, limitations, result formats, and supported search verticals.

### Search Engine Knowledge Module

The Search Engine Knowledge Module maintains a versioned knowledge base for each supported search engine.

Features include:

- Search operator registry
- Boolean operator registry
- Exact-match operators
- Domain operators
- URL operators
- Title operators
- Text operators
- File-type operators
- Date filters
- Language filters
- Geographic filters
- Related-page operators
- Link-oriented operators
- Image search capabilities
- News search capabilities
- Video search capabilities
- Shopping search capabilities
- Academic search capabilities where supported
- API capabilities
- Pagination behavior
- Rate limitations
- Query limitations
- Deprecated operators
- Unsupported operators
- Operator compatibility
- Search-engine-specific result fields
- Search-engine-specific restrictions
- Search-engine change history
- Knowledge verification dates

### Website Discovery Module

The Website Discovery Module identifies publicly accessible pages and resources associated with a target website.

Features include:

- Domain discovery
- Subdomain discovery
- URL discovery
- Page discovery
- Sitemap discovery
- Sitemap index discovery
- Robots.txt discovery
- RSS discovery
- Atom discovery
- Internal-link discovery
- External-link discovery
- Canonical discovery
- Alternate URL discovery
- Pagination discovery
- Structured-data discovery
- Open Graph discovery
- Web manifest discovery
- Public API discovery
- Feed discovery
- Archive reference discovery
- Redirect discovery
- URL parameter discovery
- URL pattern discovery
- Orphan-page discovery
- Public page discovery through search engines

Every discovered URL should receive a unique research record regardless of how many sources discover it.

### Website Crawler Module

The Website Crawler retrieves publicly accessible website resources for research and analysis.

Features include:

- Recursive crawling
- Domain-restricted crawling
- Subdomain crawling
- URL-pattern crawling
- Depth-limited crawling
- Breadth-limited crawling
- Incremental crawling
- Sitemap-driven crawling
- Search-driven crawling
- Link-driven crawling
- Redirect-chain tracking
- HTTP status tracking
- Content-type detection
- MIME-type detection
- Character encoding detection
- Response-header collection
- ETag collection
- Last-modified collection
- Cache-control collection
- Content-length collection
- Retrieval timestamping
- Crawl-session logging
- Crawl-error reporting
- Duplicate-request prevention
- Crawl deduplication
- Crawl prioritization
- Request throttling
- Concurrency controls
- Robots-aware crawling
- Crawl policy configuration

### Page Archive Module

The Page Archive Module preserves discovered pages as research evidence.

Features include:

- Raw HTML archival
- Extracted-text archival
- Response archival
- HTTP-header archival
- Metadata archival
- Structured-data archival
- Link archival
- Image-reference archival
- Resource-reference archival
- Screenshot archival where supported
- Timestamped snapshots
- Versioned page archives
- Content hashing
- Archive integrity verification
- Duplicate snapshot detection
- Near-duplicate detection
- Historical page comparison
- Deleted-page detection
- Changed-page detection
- Archive manifests
- Evidence preservation
- Archive search
- Archive export
- Research snapshot creation

Archived pages should preserve sufficient information to reproduce the research observation whenever technically and legally appropriate.

### Website Structure Analysis Module

The Website Structure Analysis Module reconstructs the architecture of a website.

Features include:

- URL hierarchy analysis
- Directory hierarchy analysis
- Subdomain analysis
- Page-depth analysis
- Navigation analysis
- Breadcrumb analysis
- Parent-child relationships
- Content hierarchy analysis
- Website graph generation
- Site-cluster detection
- Topic-cluster detection
- Hub-page detection
- Authority-flow modeling
- Orphan-page detection
- Deep-page detection
- Duplicate URL detection
- URL normalization analysis
- Canonical relationship analysis
- Redirect topology analysis
- Pagination analysis

### Internal Link Analysis Module

The Internal Link Analysis Module analyzes how pages within a website connect to one another.

Features include:

- Internal-link inventory
- Incoming-link analysis
- Outgoing-link analysis
- Link-frequency analysis
- Anchor-text analysis
- Anchor-context analysis
- Contextual-link detection
- Navigation-link detection
- Footer-link detection
- Sidebar-link detection
- Breadcrumb-link detection
- Hub-page identification
- Authority-page identification
- Internal authority distribution
- Link concentration analysis
- Link dilution analysis
- Link-depth analysis
- Orphan-page detection
- Internal-link opportunity detection
- Internal-link graph generation
- Historical internal-link comparison

### Backlink Intelligence Module

The Backlink Intelligence Module researches external links pointing toward the target website.

Features include:

- Backlink discovery
- Referring-domain discovery
- Referring URL discovery
- Destination-page analysis
- Anchor-text analysis
- Link-context analysis
- Follow and nofollow classification
- Sponsored-link classification
- UGC-link classification
- Redirected-link detection
- Broken-backlink detection
- Lost-backlink detection
- New-backlink detection
- Historical-backlink tracking
- Link-velocity analysis
- Referring-domain diversity
- Link concentration analysis
- Anchor distribution analysis
- Branded-anchor detection
- Exact-match-anchor detection
- Partial-match-anchor detection
- Naked-URL detection
- Editorial-link detection
- Directory-link detection
- Resource-link detection
- Partner-link detection
- Organization-link detection
- Geographic-link detection
- Industry-link detection
- Media-link detection
- Educational-link detection
- Government-link detection
- Social-link detection
- Backlink graph generation
- Historical backlink analysis

The module must distinguish between confirmed backlinks, search-engine-reported backlinks, crawler-observed backlinks, historical observations, and inferred relationships.

### Keyword Intelligence Module

The Keyword Intelligence Module reconstructs the vocabulary and keyword targeting of the website.

Features include:

- Keyword extraction
- Keyword normalization
- Keyword frequency
- Keyword density
- Keyword prominence
- Keyword placement
- Phrase extraction
- N-gram analysis
- Long-tail keyword discovery
- Short-tail keyword discovery
- Branded keyword discovery
- Non-branded keyword discovery
- Local keyword discovery
- Commercial keyword discovery
- Informational keyword discovery
- Navigational keyword discovery
- Transactional keyword discovery
- Question keyword discovery
- Entity keyword discovery
- Semantic keyword discovery
- Keyword clustering
- Topic clustering
- Keyword-to-page mapping
- Keyword-to-topic mapping
- Keyword cannibalization detection
- Keyword gap detection
- Keyword coverage analysis
- Keyword evolution tracking
- Keyword strategy timeline

### Semantic Analysis Module

The Semantic Analysis Module analyzes the concepts and entities represented throughout a website.

Features include:

- Entity extraction
- Entity resolution
- Entity relationship detection
- Topic extraction
- Concept extraction
- Semantic similarity
- Semantic clustering
- Related-term analysis
- Knowledge relationship mapping
- Entity consistency analysis
- Topic authority analysis
- Semantic gap detection
- Semantic overlap detection
- Content cannibalization detection
- Search-intent classification
- Query-intent modeling
- Entity-to-page mapping
- Entity-to-topic mapping

### Content Intelligence Module

The Content Intelligence Module evaluates the website's content as a connected body of information.

Features include:

- Content inventory
- Content classification
- Content clustering
- Topic modeling
- Topic hierarchy
- Topic authority analysis
- Content-depth analysis
- Content-completeness analysis
- Content-overlap detection
- Duplicate-content detection
- Near-duplicate detection
- Thin-content detection
- Content-gap analysis
- Content-pruning detection
- Content-consolidation detection
- Content-refresh detection
- Publishing-frequency analysis
- Content-aging analysis
- Evergreen-content detection
- Time-sensitive-content detection
- Pillar-page detection
- Supporting-page detection
- Cornerstone-content detection
- Content-series detection
- Question-content detection
- Comparison-content detection
- Tutorial-content detection
- Commercial-content detection
- Informational-content detection

### Metadata Analysis Module

The Metadata Analysis Module analyzes metadata and machine-readable information.

Features include:

- Title extraction
- Meta-description extraction
- Meta-robots analysis
- Canonical analysis
- Language metadata analysis
- Hreflang analysis
- Open Graph analysis
- Social-card analysis
- Structured-data extraction
- Schema.org detection
- JSON-LD analysis
- Microdata analysis
- RDFa analysis
- Author metadata
- Publisher metadata
- Publication metadata
- Modification metadata
- Image metadata

### Technical SEO Module

The Technical SEO Module analyzes observable technical search-engine optimization characteristics.

Features include:

- HTTPS analysis
- HTTP status analysis
- Redirect analysis
- Canonical analysis
- Crawlability analysis
- Indexability analysis
- Robots.txt analysis
- XML sitemap analysis
- Sitemap coverage
- Duplicate-content analysis
- URL normalization
- Pagination analysis
- Faceted-navigation analysis
- JavaScript dependency analysis
- Rendering analysis
- Mobile metadata analysis
- Structured-data analysis
- Breadcrumb analysis
- International SEO analysis
- Page-speed indicators
- Resource analysis
- Image-delivery analysis
- Script analysis
- Stylesheet analysis
- Performance-resource mapping

### SEO Strategy Analysis Module

The SEO Strategy Analysis Module identifies, classifies, and connects the SEO techniques utilized across a website.

The module analyzes observable implementation rather than claiming knowledge of the website owner's private intentions.

Features include:

- Complete SEO technique discovery
- SEO technique classification
- SEO strategy reconstruction
- On-page SEO analysis
- Technical SEO strategy analysis
- Content SEO analysis
- Keyword strategy analysis
- Internal-linking strategy analysis
- Backlink strategy analysis
- Local SEO strategy analysis
- Entity SEO analysis
- Structured-data strategy analysis
- SERP feature strategy analysis
- Off-page SEO analysis
- Programmatic SEO detection
- Automated SEO pattern detection
- International SEO analysis
- Competitive SEO analysis
- Historical SEO strategy analysis
- SEO strategy timeline
- SEO technique frequency analysis
- SEO technique distribution
- SEO technique correlation
- SEO technique dependency analysis
- SEO strategy graph
- SEO implementation mapping
- SEO pattern detection
- SEO change detection
- SEO anomaly detection
- SEO opportunity identification

#### On-Page SEO Strategy

Features include:

- Title optimization analysis
- Meta-description optimization
- Heading hierarchy
- Keyword placement
- Keyword frequency
- Keyword variation
- Semantic keyword usage
- Long-tail targeting
- Search-intent alignment
- URL optimization
- Content length
- Content depth
- Content freshness
- Content updating patterns
- Internal linking
- Anchor-text optimization
- Image optimization
- Alternative-text optimization
- Featured-snippet targeting
- FAQ optimization
- List optimization
- Table optimization
- Entity optimization
- Author signals
- Publication signals
- Content clustering
- Pillar and supporting content structures

#### Technical SEO Strategy

Features include:

- Crawlability strategy
- Indexability strategy
- XML sitemap implementation
- Robots.txt configuration
- Canonicalization strategy
- Redirect strategy
- URL normalization
- Duplicate-content management
- Pagination
- Faceted navigation
- JavaScript rendering
- Structured-data implementation
- Breadcrumb implementation
- International SEO signals
- Hreflang implementation
- Mobile optimization signals
- Performance optimization signals
- Image-delivery strategy
- Resource optimization
- Site-architecture strategy
- Crawl-depth management

#### Keyword Strategy

Features include:

- Primary keyword identification
- Secondary keyword identification
- Long-tail keyword targeting
- Local keyword targeting
- Commercial keyword targeting
- Informational keyword targeting
- Navigational keyword targeting
- Transactional keyword targeting
- Branded keyword targeting
- Geographic keyword targeting
- Industry terminology
- Entity terminology
- Question-based queries
- Keyword clusters
- Keyword-to-page assignments
- Keyword overlap
- Keyword cannibalization candidates
- Untargeted semantic areas
- Changes in keyword targeting

The module should produce a Keyword Strategy Map connecting keywords to pages, topics, search intent, metadata, headings, internal links, and observed search visibility.

#### Content Strategy

Features include:

- Content clusters
- Topic clusters
- Pillar pages
- Supporting articles
- Cornerstone content
- Evergreen content
- Time-sensitive content
- Location-based content
- Question-based content
- Comparison content
- List content
- Tutorial content
- Commercial landing pages
- Supporting informational pages
- Content publishing frequency
- Content refresh frequency
- Topic expansion patterns
- Content consolidation
- Content pruning
- Content repurposing patterns

#### Internal Linking Strategy

Features include:

- Hub-page identification
- Authority-page identification
- Supporting-page identification
- Link-silo detection
- Topic-cluster detection
- Contextual-link analysis
- Navigation-link analysis
- Footer-link analysis
- Sidebar-link analysis
- Breadcrumb-link analysis
- Anchor-text patterns
- Link concentration
- Link distribution
- Deep-linking strategy
- Orphan-page identification
- Internal authority-flow analysis

#### Backlink Strategy

Features include:

- Referring-domain diversity
- Backlink concentration
- Anchor-text distribution
- Branded anchors
- Exact-match anchors
- Partial-match anchors
- Naked URLs
- Contextual backlinks
- Editorial backlinks
- Directory links
- Resource links
- Partner links
- Citation links
- Geographic links
- Industry links
- Media links
- Educational links
- Government links
- Link velocity
- Historical link acquisition
- Lost-link patterns
- Newly discovered backlinks

#### Local SEO Strategy

Features include:

- Geographic landing pages
- City targeting
- Regional targeting
- Local keyword targeting
- LocalBusiness structured data
- Organization information
- Address information
- Phone information
- Service-area signals
- Local content
- Local citations
- Local backlink patterns
- Geographic internal linking
- Location-specific metadata
- Local search queries
- Neighborhood terminology
- Regional terminology

#### Entity SEO Strategy

Features include:

- Organization entities
- Person entities
- Product entities
- Service entities
- Location entities
- Brand entities
- Schema.org entities
- Entity relationships
- Consistent entity naming
- About-page signals
- Author pages
- Organization pages
- SameAs relationships
- External authority references

#### SERP Feature Strategy

Features include:

- Featured-snippet analysis
- Rich-result analysis
- FAQ-result analysis
- Review-result analysis
- Product-result analysis
- Local-result analysis
- Image-result analysis
- Video-result analysis
- News-result analysis
- Sitelink analysis
- Breadcrumb-result analysis
- Other supported structured-result analysis

#### Off-Page SEO Strategy

Features include:

- Brand mentions
- External references
- Digital citations
- Public profiles
- Organization references
- Author references
- Community references
- Industry references
- Media references
- External content relationships
- Reputation signals
- Link acquisition patterns

#### SEO Automation Detection

Features include:

- Large-scale page generation detection
- Template-generated page detection
- Programmatic landing-page detection
- Automated metadata detection
- Automated internal-link detection
- Location-page generation patterns
- Keyword-page generation patterns
- Repeated content-template detection
- Structured-data generation patterns
- Automated sitemap patterns
- Automated content-update patterns
- Machine-generated content indicators

The system must identify observable patterns without presenting unsupported assumptions about the people, organizations, or technologies responsible for them as established facts.

#### SEO Technique Classification

Each identified technique should record:

- Technique
- Technique category
- Pages affected
- Frequency
- First observed date
- Most recent observed date
- Evidence
- Source
- Confidence
- Related techniques
- Search-engine observations
- Historical changes

The system should distinguish between:

- Observation
- Pattern
- Technique
- Strategy
- Inference

### Search Visibility Module

The Search Visibility Module records how websites and pages appear across supported search environments.

Features include:

- Search query tracking
- Search-result position tracking
- Search-result URL tracking
- Displayed-title tracking
- Displayed-description tracking
- Result-type classification
- Search-feature detection
- Search-engine comparison
- Search-result history
- Search-result volatility
- Search visibility mapping
- Search visibility change detection

Each observation should preserve the search engine, query, timestamp, region, language, result position where available, URL, displayed metadata, and result type.

### Local SEO Module

The Local SEO Module evaluates geographic search signals.

Features include:

- Geographic keyword analysis
- Location-page detection
- City-page detection
- Regional-page detection
- Service-area analysis
- LocalBusiness schema detection
- Organization schema analysis
- Address analysis
- Phone analysis
- Local citation discovery
- Local backlink analysis
- Geographic anchor analysis
- Local content analysis
- Local search-result analysis
- Regional search visibility
- Geographic topic clustering

### Entity SEO Module

The Entity SEO Module analyzes how a website establishes and reinforces identifiable entities.

Features include:

- Person entity detection
- Organization entity detection
- Brand entity detection
- Product entity detection
- Service entity detection
- Location entity detection
- Schema entity mapping
- SameAs relationship analysis
- Entity consistency analysis
- Entity relationship mapping
- Author identity signals
- Organization identity signals
- External entity references

### AI Search Analysis Module

The AI Search Analysis Module analyzes observable website characteristics relevant to AI-mediated search and answer systems.

Features include:

- AI-search visibility research
- Answer-engine discovery
- Citation-surface analysis
- Answer-content analysis
- Entity-clarity analysis
- Structured-information analysis
- Citation-friendly-content detection
- Direct-answer detection
- Question-answer structure analysis
- Machine-readable-content analysis
- AI search-result comparison
- Observable AI citation tracking where supported

The module must distinguish observable evidence from assumptions about proprietary ranking or retrieval systems.

### Competitive Research Module

The Competitive Research Module compares the target website with other relevant websites.

Features include:

- Competitor discovery
- Competitor URL discovery
- Competitor keyword comparison
- Competitor content comparison
- Competitor backlink comparison
- Competitor topic comparison
- Competitor internal-link comparison
- Competitor technical comparison
- Competitor SEO technique comparison
- Competitor search visibility comparison
- Competitor content-gap analysis
- Competitor keyword-gap analysis
- Competitor backlink-gap analysis
- Competitive strategy mapping

### Historical Analysis Module

The Historical Analysis Module compares website observations across research sessions.

Features include:

- Website snapshots
- Page snapshots
- Keyword history
- Content history
- Metadata history
- Internal-link history
- Backlink history
- Search-visibility history
- Technical-change history
- SEO-strategy history
- URL migration detection
- Domain migration detection
- Content-pruning detection
- Content-expansion detection
- SEO-technique adoption tracking
- SEO-technique abandonment tracking
- Historical comparison reports

### Change Detection Module

The Change Detection Module identifies changes between research snapshots.

Features include:

- Page-change detection
- Content-change detection
- Metadata-change detection
- Keyword-change detection
- Link-change detection
- Backlink-change detection
- URL-change detection
- Redirect-change detection
- Canonical-change detection
- Sitemap-change detection
- Robots-change detection
- Structured-data change detection
- SEO-technique change detection
- Website-structure change detection
- Search-visibility change detection

### Research Provenance Module

The Research Provenance Module maintains the evidence chain behind research findings.

Features include:

- Source attribution
- Observation provenance
- Search-query provenance
- Search-engine provenance
- Agent provenance
- Retrieval timestamps
- Processing timestamps
- Archive hashes
- Evidence hashes
- Confidence scoring
- Verification status
- Evidence relationships
- Observation history
- Source classification
- Evidence-chain reconstruction

### Research Graph Module

The Research Graph Module represents research entities and relationships as an interconnected graph.

Entities may include:

- Websites
- Domains
- Subdomains
- Pages
- URLs
- Search engines
- Search queries
- Keywords
- Entities
- Topics
- Links
- Backlinks
- Referring domains
- Authors
- Organizations
- Structured-data entities
- Archive snapshots
- SEO techniques
- Research observations

Relationships may include:

- Links to
- Redirects to
- Canonicalizes to
- Discovered by
- Indexed by
- References
- Contains keyword
- Belongs to topic
- Refers to
- Archived as
- Changed from
- Changed to
- Implements technique
- Supports finding
- Discovered through

### Evidence Management Module

The Evidence Management Module manages research evidence independently from analytical conclusions.

Features include:

- Evidence collection
- Evidence preservation
- Evidence hashing
- Evidence manifests
- Evidence versioning
- Evidence deduplication
- Evidence comparison
- Evidence verification
- Evidence confidence
- Evidence-chain tracking
- Evidence export
- Evidence search
- Research snapshot locking

### Research Quality Module

The Research Quality Module evaluates the completeness and reliability of a research session.

Features include:

- Coverage scoring
- Evidence-completeness scoring
- Source-diversity scoring
- Search-engine-diversity scoring
- Crawl-completeness scoring
- Archive-completeness scoring
- Agent-agreement scoring
- Finding-confidence scoring
- Research-quality scoring
- Contradiction detection
- Unsupported-claim detection
- Missing-evidence detection
- Reproducibility validation

### Reporting Module

The Reporting Module transforms research datasets into human-readable and machine-readable outputs.

Features include:

- Executive research reports
- Complete website reports
- Page-by-page reports
- SEO reports
- SEO strategy reports
- Keyword reports
- Backlink reports
- Internal-link reports
- Technical SEO reports
- Content reports
- Semantic reports
- Search-engine comparison reports
- Competitive reports
- Historical reports
- Change reports
- Evidence reports
- Archive reports
- Research coverage reports
- Agent activity reports
- Research methodology reports
- Machine-readable reports
- JSON export
- CSV export
- Graph export
- Archive export

### Research Automation Module

The Research Automation Module enables recurring and event-driven research.

Features include:

- Scheduled research
- Recurring website audits
- Scheduled crawling
- Scheduled SERP monitoring
- Automated change detection
- Automated backlink monitoring
- Automated keyword monitoring
- Automated content monitoring
- Automated SEO-strategy monitoring
- Automatic report generation
- Research alerts
- Threshold alerts
- Anomaly alerts
- Change alerts
- New-page alerts
- Deleted-page alerts
- New-backlink alerts
- Lost-backlink alerts
- Search-visibility alerts

### Data Management Module

The Data Management Module manages structured research datasets.

Features include:

- Local research database
- Structured datasets
- URL deduplication
- Page deduplication
- Content deduplication
- Entity deduplication
- Keyword normalization
- Domain normalization
- URL normalization
- Dataset versioning
- Dataset snapshots
- Incremental updates
- Data-integrity validation
- Research-session isolation
- Data export
- Data import
- Backup support

### Security Module

The Security Module protects research data, credentials, agents, and system resources.

Features include:

- Credential isolation
- API-key protection
- Secret management
- Agent permission boundaries
- Module permission boundaries
- Crawl-domain restrictions
- Request-rate controls
- Resource limits
- Audit logging
- Research activity logging
- Configuration auditing
- Research-session isolation

### Responsible Research Module

The Responsible Research Module provides configurable controls for responsible website research.

Features include:

- Robots.txt awareness
- Rate-limit enforcement
- Crawl-delay configuration
- Request throttling
- Domain allowlists
- Domain blocklists
- Authentication-boundary protection
- Access-control respect
- Terms-aware configuration
- Research-purpose logging
- Source attribution
- Archive provenance
- Responsible crawling controls

The system must not be designed to bypass authentication, access controls, paywalls, technical restrictions, or other barriers intended to restrict access.

---

## Optional Plugin Modules

WebDetective should support independent plugins that extend the core system without requiring changes to the core research architecture.

### Search Engine Plugins

- Additional search-engine agents
- Specialized search operators
- Search vertical integrations
- Search API integrations
- Search-result parsers
- Search-engine-specific historical datasets
- Search-engine-specific ranking observations

### Web Archive Plugins

- Public web archive integrations
- Historical snapshot providers
- Archive comparison services
- Historical URL discovery
- Historical backlink discovery

### Domain Intelligence Plugins

- DNS research
- Domain registration research
- Certificate research
- Subdomain intelligence
- Domain relationship analysis
- Hosting intelligence
- CDN detection

### Technology Detection Plugins

- CMS detection
- Framework detection
- JavaScript framework detection
- Analytics technology detection
- Advertising technology detection
- CDN detection
- Hosting detection
- E-commerce platform detection
- Marketing technology detection
- SEO platform detection

### Performance Plugins

- Performance testing
- Resource timing analysis
- Page-load analysis
- Core Web Vitals-related analysis
- Image-performance analysis
- JavaScript-performance analysis
- CSS-performance analysis
- Resource waterfall analysis

### Accessibility Plugins

- Accessibility analysis
- Semantic HTML analysis
- Alternative-text analysis
- Heading structure analysis
- Keyboard accessibility indicators
- ARIA analysis
- Form accessibility analysis
- Accessibility reporting

### Social Intelligence Plugins

- Public social-profile discovery
- Public social-link analysis
- Brand mention discovery
- Public social-content research
- Social backlink analysis
- Social identity relationships

### Media Intelligence Plugins

- Image discovery
- Image metadata analysis
- Reverse-reference research where supported
- Video discovery
- Video metadata analysis
- Audio discovery
- Media relationship mapping

### Geographic Research Plugins

- Geographic search
- Local-result research
- Location intelligence
- Regional content analysis
- Geographic backlink analysis
- Geographic keyword analysis

### Multilingual Research Plugins

- Language detection
- Translation-assisted analysis
- Multilingual keyword extraction
- Cross-language topic mapping
- International SEO analysis
- Hreflang validation
- Cross-language content comparison

### AI Research Plugins

- AI model integrations
- Embedding analysis
- Semantic retrieval
- Local language models
- AI search research
- AI citation research
- Agent-specific reasoning modules
- Custom research models

### Notification Plugins

- Email notifications
- Webhook notifications
- Messaging integrations
- Research alerts
- Change alerts
- Monitoring alerts
- Report delivery

### Visualization Plugins

- Website graph visualization
- Backlink graph visualization
- Keyword maps
- Topic maps
- SEO strategy maps
- Search-result visualization
- Historical timelines
- Research dashboards

### Export Plugins

- Database export
- Graph export
- JSON export
- CSV export
- XML export
- Research package export
- Archive package export
- Custom report formats

### Custom Agent Plugins

Third-party developers may create specialized research agents for domains such as:

- Industry research
- Legal research
- Academic research
- Regulatory research
- Market research
- Financial research
- Real estate research
- Product research
- Competitive intelligence
- Brand intelligence
- Content intelligence

---

## Agent Interface

Every agent should expose standardized capabilities for integration with the Research Coordinator.

Agent metadata should include:

- Agent name
- Agent version
- Agent purpose
- Agent capabilities
- Required inputs
- Generated outputs
- Dependencies
- Evidence requirements
- Confidence methodology
- Supported data formats
- Configuration options
- Resource requirements

Agents should preserve provenance for their findings and identify which observations support each conclusion.

---

## Search Engine Module Interface

Every search-engine plugin should define:

- Search-engine identity
- Module version
- Supported search types
- Native query syntax
- Supported operators
- Operator limitations
- Authentication requirements
- API capabilities
- Rate limitations
- Result schema
- Pagination behavior
- Geographic capabilities
- Language capabilities
- Search verticals
- Evidence fields
- Query translation rules
- Version information
- Capability verification date

The core system should not assume that all search engines provide identical functionality.

---

## Research Workflow

A typical WebDetective investigation may follow this process:

- Define the research objective.
- Identify the target website and domains.
- Initialize the research session.
- Activate relevant search-engine agents.
- Discover URLs through multiple sources.
- Crawl publicly accessible pages.
- Archive discovered pages.
- Build the website structure graph.
- Analyze internal links.
- Research backlinks.
- Extract keywords and entities.
- Analyze content and metadata.
- Analyze technical SEO.
- Analyze the website's SEO techniques.
- Reconstruct observable SEO strategies.
- Compare search-engine visibility.
- Compare historical observations where available.
- Identify patterns and changes.
- Validate evidence and confidence.
- Generate the final research dataset.
- Generate human-readable reports.

---

## Observation and Inference Model

WebDetective must distinguish between evidence and interpretation.

### Observation

A directly measurable or directly retrievable fact.

### Pattern

A repeated observation across multiple pages, sources, or research sessions.

### Technique

A recognized implementation supported by observable evidence.

### Strategy

A collection of related techniques that form an observable pattern across a website.

### Inference

A reasoned interpretation that is not directly established by the available evidence.

The system should never silently convert an inference into an observation.

---

## Confidence Model

Findings may be classified as:

- Confirmed
- Strong
- Moderate
- Weak
- Inferred
- Unverified

Confidence should be assigned to individual observations and findings rather than automatically assigning one confidence level to an entire research session.

---

## Research Reproducibility

A research session should preserve sufficient information to reproduce the investigation.

Research metadata should include:

- Research objective
- Target domains
- Target URLs
- Search engines
- Search queries
- Search-engine module versions
- Agent versions
- Crawl configuration
- Retrieval timestamps
- Analysis configuration
- Archive hashes
- Evidence hashes
- Research results

## Archive Integrity

Archived evidence should be protected against accidental modification.

The system should support:

- Cryptographic content hashes
- Immutable research snapshots
- Timestamped observations
- Archive versioning
- Integrity verification
- Duplicate detection
- Evidence manifests
- Archive provenance

## Extensibility

WebDetective should allow new research capabilities to be introduced without modifying the core specification.

New modules should:

- Declare their capabilities
- Use standardized interfaces
- Preserve provenance
- Produce structured outputs
- Identify dependencies
- Report confidence
- Integrate with the Research Coordinator
- Integrate with the Research Graph where appropriate
- Maintain independent versioning

A module may operate as an independent agent, service, plugin, library, or local process provided that it conforms to the WebDetective specification.

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
  - [https://roxanneardary.com/webdetective/](https://roxanneardary.com/webdetective/)  

---

## License & Notice Requirements

WebDetective is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- WebDetective specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
