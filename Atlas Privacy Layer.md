# Atlas Privacy Layer

**A programmable privacy layer for Earth data.**

Atlas Privacy Layer is an open-source geospatial privacy and rendering framework that provides programmable control over how satellite and map imagery is processed, transformed, and presented. Rather than modifying imagery at its source, Atlas introduces a configurable privacy layer between geospatial data providers and mapping applications, allowing developers to apply privacy-aware rendering policies to protected areas.

Designed for self-hosted deployments, Atlas combines spatial analysis, configurable rendering pipelines, and AI-assisted computer vision into a modular platform that integrates with modern GIS infrastructure.

---

# Design Goals

- Modular and extensible architecture
- Privacy-first rendering pipeline
- Self-hosted deployment
- Standards-based GIS compatibility
- AI-assisted spatial analysis
- Plugin-driven extensibility
- Scalable tile processing
- Developer-friendly APIs

---

# Core Modules

## Privacy Tile Proxy

The Privacy Tile Proxy serves as the primary entry point into Atlas. It intercepts map tile requests, evaluates configured privacy policies, and routes imagery through the rendering pipeline before delivery.

### Features

- XYZ tile interception
- Tile request routing
- Tile caching support
- Multi-provider compatibility
- Real-time tile transformation
- Cached rendering mode
- High-performance proxy architecture

---

## Boundary Engine

The Boundary Engine manages protected geographic regions and determines where privacy policies should be applied.

### Features

- Property boundary management
- Polygon-based privacy zones
- Buffer zones
- GeoJSON import
- Coordinate-based protection
- Spatial indexing
- Boundary intersection testing
- Multi-zone management

---

## Privacy Rendering Engine

The rendering engine transforms imagery according to configured privacy policies.

### Features

- Gaussian blur
- Pixelation
- Mosaic rendering
- Tile scrambling
- Edge degradation
- Noise generation
- Opacity masking
- Layer compositing
- Multiple rendering modes

---

## Synthetic Terrain Engine

Generates replacement imagery that conceals sensitive features while preserving overall geographic context.

### Features

- Procedural terrain generation
- Vegetation synthesis
- Soil and grass replacement
- Terrain blending
- Texture synthesis
- AI-assisted inpainting support
- Context-aware replacement
- Synthetic landscape generation

---

## AI Object Detection Engine

Provides intelligent feature recognition before privacy transformations are applied.

### Features

- Building detection
- Vehicle detection
- Infrastructure detection
- Land-use classification
- Reflective surface detection
- Semantic segmentation
- Object classification
- Context-aware rendering decisions

Supported model integrations include:

- YOLO
- Segment Anything Model (SAM)
- Semantic segmentation networks
- Custom computer vision models

---

## Privacy Rule Engine

Evaluates rendering policies for every protected region.

### Features

- Zone-specific rules
- Zoom-level policies
- User access policies
- Time-based rendering
- Conditional transformations
- Rule prioritization
- Policy inheritance
- Configurable privacy levels

---

## GIS Integration Layer

Provides interoperability with common geospatial software and standards.

### Features

- PostGIS integration
- GDAL compatibility
- Raster processing
- Vector processing
- XYZ tile services
- Spatial coordinate support
- GIS data import/export
- MapLibre compatibility
- Leaflet compatibility

---

## Audit & Monitoring

Provides operational transparency for rendering decisions.

### Features

- Tile processing logs
- Rule execution history
- Rendering statistics
- Transformation tracking
- Performance metrics
- Processing diagnostics
- Event auditing

---

## Developer API

Exposes Atlas functionality through programmable interfaces.

### Features

- REST API
- Tile rendering endpoints
- Zone management
- Rendering controls
- Rule management
- Administrative APIs
- Integration endpoints

---

# Optional Plug-in Modules

Atlas supports optional plug-ins that extend the core platform without modifying the primary codebase.

## AI Vision Plug-ins

Optional integrations for advanced computer vision.

Examples:

- Custom object detectors
- Specialized segmentation models
- Wildlife detection
- Agricultural classification
- Infrastructure recognition

---

## Synthetic Terrain Plug-ins

Additional terrain generation engines.

Examples:

- Forest generation
- Desert simulation
- Water replacement
- Seasonal terrain
- Urban replacement
- Procedural landscape packs

---

## Rendering Plug-ins

Alternative privacy transformation algorithms.

Examples:

- Adaptive blur
- Edge-preserving masking
- Fractal scrambling
- Frequency-domain obfuscation
- Dynamic pixel displacement
- Custom shader pipelines

---

## GIS Connector Plug-ins

Support for additional mapping infrastructure.

Examples:

- GeoServer
- TileServer GL
- ArcGIS
- QGIS
- MapServer
- WMTS
- WMS

---

## Storage Plug-ins

Support additional storage backends.

Examples:

- PostgreSQL extensions
- Redis
- Object storage
- Distributed caches
- Cloud storage providers

---

## Authentication Plug-ins

Optional authentication and authorization systems.

Examples:

- OAuth
- OpenID Connect
- LDAP
- SAML
- API Keys
- JWT

---

## Automation Plug-ins

Extend Atlas with automation workflows.

Examples:

- Scheduled rendering
- Batch processing
- Rule automation
- Event-driven processing
- Background workers

---

## Monitoring Plug-ins

Integrate operational monitoring.

Examples:

- Prometheus
- Grafana
- OpenTelemetry
- Custom metrics
- Alerting systems

---

## Developer Plug-ins

Extend Atlas through custom modules.

Examples:

- Custom APIs
- Rendering extensions
- Rule processors
- Data providers
- Analytics modules
- Experimental features

---

# Philosophy

Atlas Privacy Layer is built on a simple principle:

> **If you control the rendering layer, you control what is revealed.**

Atlas does not modify external satellite imagery providers or claim to remove imagery from third-party services. Instead, it provides a programmable, privacy-aware rendering layer that enables organizations and developers to control how geospatial data is presented within the systems they deploy and manage.  

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
  - [https://roxanneardary.com/atlas-urban-intelligence/](https://roxanneardary.com/atlas-urban-intelligence/)  

---

# License & Notice Requirements

Atlas Urban Intelligence is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Atlas Urban Intelligence specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
