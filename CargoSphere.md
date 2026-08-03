# CargoSphere

**Track Assets. Operators. Risk. Opportunity.**

CargoSphere is an **AGPL-3.0+ licensed open specification** for building modular commercial maritime intelligence platforms. It provides a standardized framework for collecting, structuring, analyzing, and visualizing information about ports, maritime infrastructure, ownership structures, operators, trade relationships, and economic activity.

CargoSphere is designed as a flexible intelligence architecture that enables organizations to build transparent, extensible systems for understanding maritime infrastructure. The specification connects physical assets, corporate entities, trade flows, geographic data, and economic indicators into a unified intelligence ecosystem.

The platform is designed for logistics companies, investment firms, insurers, researchers, infrastructure analysts, governments, and organizations requiring deeper visibility into maritime operations.

---

# Design Principles

CargoSphere follows several core principles:

## Modular Architecture

CargoSphere separates essential intelligence capabilities into core modules while allowing specialized functionality to be added through optional plugin modules.

Organizations can deploy only the modules required for their use case while maintaining compatibility with the broader ecosystem.

## Open Data Interoperability

The specification is designed to integrate with:

- Public records
- Government datasets
- Geographic information systems
- Corporate registries
- Trade databases
- Logistics systems
- Commercial intelligence platforms

## Entity-Based Intelligence

CargoSphere organizes information around connected entities:

- Ports
- Facilities
- Companies
- Properties
- Assets
- Countries
- Industries
- Cargo
- Trade routes

## Relationship-Based Analysis

The system is designed to identify relationships between entities rather than storing isolated records.

---

# System Architecture

CargoSphere consists of:

## Core Modules

Core modules provide the foundation of the specification and define the minimum intelligence framework.

## Optional Plugin Modules

Plugin modules extend functionality for specialized analysis, industries, and commercial use cases.

## Data Layer

The data layer manages:

- Structured records
- Geographic information
- Historical records
- Corporate relationships
- Intelligence metadata

## Intelligence Layer

The intelligence layer provides:

- Entity resolution
- Relationship mapping
- Risk analysis
- Opportunity detection
- Predictive analytics

---

# Core Modules

## Port Registry Module

Provides the foundational registry of maritime infrastructure.

Features:

- Port identification
- Port authority information
- Geographic boundaries
- Facility classification
- Federal and regional identifiers
- Operational status
- Historical changes
- Infrastructure relationships

---

# Asset Management Module

Tracks physical maritime infrastructure and operational assets.

Features:

- Docks
- Berths
- Piers
- Wharves
- Terminals
- Warehouses
- Distribution centers
- Rail terminals
- Intermodal yards
- Truck facilities
- Cranes
- Grain elevators
- Fuel terminals
- Storage facilities
- Pipelines
- Cold storage
- Infrastructure capacity
- Asset lifecycle tracking
- Asset condition records

---

# Property Intelligence Module

Tracks real estate and land information associated with maritime infrastructure.

Features:

- Property ownership
- Parcel boundaries
- Property records
- Historical sales
- Tax assessments
- Property taxes
- Land use
- Easements
- Development history
- Zoning information

---

# Ownership Intelligence Module

Maps corporate ownership, control structures, and investment relationships.

Features:

- Parent companies
- Subsidiaries
- Beneficial ownership
- Joint ventures
- Holding companies
- Corporate hierarchy
- Ownership timelines
- Acquisitions
- Mergers
- Public and private ownership
- Foreign ownership participation
- Investment relationships

---

# Operator Intelligence Module

Tracks organizations operating within maritime infrastructure.

Features:

- Terminal operators
- Facility operators
- Shipping companies
- Logistics providers
- Tenants
- Service providers
- Operator history
- Operational relationships
- Facility assignments

---

# Foreign Interest Intelligence Module

Tracks international participation within maritime infrastructure.

Features:

- Foreign ownership
- Foreign operators
- International investments
- Country relationships
- Cross-border corporate structures
- Foreign-controlled assets
- International partnerships

---

# Risk Intelligence Module

Provides commercial and strategic risk analysis.

Features:

- Supply chain risk
- Ownership concentration
- Operator dependency
- Foreign exposure
- Infrastructure vulnerabilities
- Geographic risk
- Operational disruption analysis
- Regulatory risk
- Investment risk indicators
- Insurance risk indicators
- Critical infrastructure analysis

---

# Operations Intelligence Module

Tracks maritime activity and operational capabilities.

Features:

- Cargo handling
- Terminal operations
- Cruise operations
- Industrial activity
- Capacity analysis
- Facility utilization
- Logistics connections
- Operational performance

---

# Analytics Module

Provides intelligence analysis and reporting.

Features:

- Interactive dashboards
- Historical analysis
- Trend analysis
- Risk scoring
- Opportunity scoring
- Market analysis
- Infrastructure intelligence reports
- Data visualization

---

# Optional Plugin Modules

Plugin modules extend CargoSphere for specialized intelligence applications.

---

# Country of Origin Module

Tracks international trade origins and destinations.

Features:

- Import countries
- Export countries
- Trade relationships
- Country dependency analysis
- Country risk profiles
- International trade trends

---

# Cargo Type Module

Classifies and analyzes cargo activity.

Features:

- Container cargo
- Bulk cargo
- Breakbulk
- Liquid bulk
- LNG
- Agricultural products
- Energy products
- Automotive cargo
- Consumer goods
- Commodity trends
- Cargo volume analysis

---

# Industry Intelligence Module

Provides industry-specific analysis.

Supported industries:

- Agriculture
- Manufacturing
- Energy
- Mining
- Automotive
- Retail
- Construction
- Chemical
- Defense
- Food processing
- Maritime services
- Logistics

Features:

- Industry dependencies
- Facility relationships
- Market analysis
- Supply chain exposure
- Economic contribution

---

# Trade Lane Module

Maps global and domestic maritime trade corridors.

Features:

- Origin ports
- Destination ports
- Shipping routes
- Trade corridors
- Transit analysis
- Carrier participation
- Trade volume
- Seasonal patterns
- Route dependencies
- Trade relationship visualization

---

# Economic Impact Module

Measures the economic significance of maritime infrastructure.

Features:

- Employment impact
- Regional economic contribution
- Tax generation
- Import value
- Export value
- Cargo value
- Industry impact
- Public investment
- Infrastructure funding
- Economic trends

---

# Maritime Relationship Graph Module

Provides a graph-based intelligence model connecting maritime entities.

## Entity Nodes

Includes:

- Ports
- Authorities
- Facilities
- Assets
- Companies
- Operators
- Properties
- Countries
- Industries
- Cargo types
- Shipping lines
- Trade lanes
- Investors
- Government agencies

## Relationship Types

Includes:

- Owns
- Operates
- Leases
- Invests in
- Parent company of
- Subsidiary of
- Imports from
- Exports to
- Ships through
- Connected to
- Supplies
- Located within
- Financed by

Features:

- Relationship visualization
- Ownership tracing
- Supply chain mapping
- Dependency analysis
- Entity discovery
- Network analysis
- AI knowledge graph integration

---

# Technology Stack

## Backend

- Python
- FastAPI
- Celery
- Redis

## Data Processing

- Apache Airflow
- Apache Spark
- DuckDB
- Pandas
- Polars

## Databases

- PostgreSQL
- PostGIS
- Neo4j
- OpenSearch
- MinIO

## Data Collection

- Scrapy
- Playwright
- Government APIs
- GIS APIs
- Document extraction pipelines
- OCR processing

## Geospatial

- GDAL
- GeoPandas
- MapLibre
- Vector tiles
- Spatial databases

## Frontend

- React
- TypeScript
- MapLibre GL JS
- Deck.gl

## APIs

- REST API
- GraphQL
- OGC APIs
- Event-driven integrations

## Deployment

- Docker
- Kubernetes
- Helm
- Linux
- CI/CD pipelines

---

# AI Integration

CargoSphere can support AI-assisted intelligence capabilities including:

- Entity matching
- Corporate relationship discovery
- Document analysis
- Risk prediction
- Market analysis
- Opportunity identification
- Automated classification
- Knowledge graph reasoning

---

# Federation & Extensions

CargoSphere is designed for distributed deployment.

Organizations may:

- Host their own instances
- Create private intelligence networks
- Add custom modules
- Publish compatible extensions
- Integrate external datasets
- Build commercial applications

---

# Future Development Areas

Potential future modules include:

- Vessel intelligence
- Environmental intelligence
- Security intelligence
- Workforce intelligence
- Compliance intelligence
- Infrastructure forecasting
- Insurance analytics
- Supply chain simulation

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
  - [https://roxanneardary.com/cargosphere/](https://roxanneardary.com/cargosphere/)  

---

# License & Notice Requirements

CargoSphere is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- CargoSphere specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
