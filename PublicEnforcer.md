# PublicEnforcer

**Enforce Accountability, Transparently.**

PublicEnforcer is an open-source intelligence and transparency platform that tracks publicly available federal enforcement data from investigation to final resolution. The platform aggregates, organizes, and visualizes enforcement actions, court proceedings, financial penalties, restitution orders, forfeitures, and organizational outcomes using publicly released records.

The goal is to provide researchers, journalists, watchdog organizations, developers, and the public with a transparent and verifiable view of federal enforcement activity while preserving source attribution and auditability.

## Mission

PublicEnforcer transforms fragmented public records into searchable timelines, relationship graphs, and financial accountability reports.

Every record is linked to publicly available source material, allowing users to independently verify information and understand the full lifecycle of a case.

## Core Principles

- Transparency
- Public accountability
- Source verification
- Open data
- Open-source development
- Self-hosting support
- Reproducibility
- Auditability

## Features

### Case Lifecycle Tracking

Track cases through every publicly available stage:

- Investigation announcements
- Search warrant disclosures
- Arrest records
- Criminal complaints
- Indictments
- Superseding indictments
- Initial appearances
- Detention hearings
- Bail decisions
- Plea agreements
- Trial proceedings
- Convictions
- Acquittals
- Sentencing
- Appeals
- Dismissals
- Releases
- Post-conviction actions

### Investigation Monitoring

- Federal investigation tracking
- Case announcement aggregation
- Public records ingestion
- Multi-agency case linking
- Investigation timeline generation
- Event chronology reconstruction

### Court Tracking

- Court docket monitoring
- Filing history tracking
- Motion tracking
- Hearing schedules
- Judicial assignment tracking
- Case outcome monitoring
- Appeal monitoring
- Final disposition tracking

### Financial Accountability

- Restitution tracking
- Fine tracking
- Civil penalty tracking
- Settlement monitoring
- Asset forfeiture tracking
- Seizure reporting
- Corporate penalty reporting
- Financial recovery analysis
- Collection status monitoring
- Compliance reporting

### Solvency Analysis

- Organizational survival tracking
- Bankruptcy monitoring
- Receivership tracking
- Dissolution tracking
- Corporate restructuring monitoring
- Post-enforcement financial analysis
- Long-term organizational outcome tracking

### Entity Resolution

- Individual matching
- Organization matching
- Alias detection
- Subsidiary mapping
- Parent company mapping
- Relationship discovery
- Duplicate resolution
- Cross-case entity linking

### Relationship Mapping

- Person-to-case relationships
- Organization-to-case relationships
- Organization ownership structures
- Individual affiliations
- Case networks
- Financial relationships
- Enforcement networks
- Historical relationship tracking

### Timeline Engine

- Automatic timeline generation
- Case milestone visualization
- Historical event reconstruction
- Cross-case timelines
- Organization timelines
- Individual timelines
- Financial event timelines

### Geographic Intelligence

- Enforcement heat maps
- Jurisdiction analysis
- Geographic trend analysis
- Regional enforcement comparisons
- District-level statistics
- State-level reporting
- National enforcement visualization

### Search and Discovery

- Full-text search
- Semantic search
- Advanced filtering
- Date range filtering
- Jurisdiction filtering
- Statute filtering
- Agency filtering
- Organization filtering
- Financial threshold filtering

### Analytics and Reporting

- Enforcement trend analysis
- Statistical reporting
- Outcome analysis
- Financial impact analysis
- Agency activity reporting
- Jurisdiction comparisons
- Historical comparisons
- Exportable reports

### Data Verification

- Source attribution
- Citation tracking
- Record provenance
- Change history
- Audit logs
- Verification workflows
- Public source references
- Transparency reporting

### Open Data Tools

- Public API
- GraphQL API
- JSON exports
- CSV exports
- Parquet exports
- Bulk downloads
- Developer integrations
- Data federation support

### Dashboard System

- Case dashboards
- Organization dashboards
- Financial dashboards
- Geographic dashboards
- Agency dashboards
- Enforcement dashboards
- Trend dashboards
- Custom dashboard creation

### Document Processing

- OCR processing
- PDF extraction
- Structured data extraction
- Entity extraction
- Metadata extraction
- Document indexing
- Document classification
- Archive management

### Alerts and Monitoring

- New case alerts
- Filing alerts
- Outcome alerts
- Financial event alerts
- Organization alerts
- Agency alerts
- Custom watchlists
- Notification management

### Self-Hosting

- Docker deployment
- Docker Compose support
- Podman support
- Linux deployment support
- On-premise deployment
- Air-gapped deployment options
- Backup and recovery tools
- Scalable architecture

## Technology Stack

### Data Collection

- Python
- Scrapy
- Feedparser
- Requests
- OCRmyPDF
- Tesseract OCR

### Processing

- Apache Tika
- spaCy
- Hugging Face Transformers
- Legal-BERT Models

### Storage

- PostgreSQL
- Neo4j
- OpenSearch
- MinIO

### Backend

- FastAPI
- GraphQL
- SQLAlchemy
- Alembic

### Frontend

- React
- TypeScript
- Vite
- Leaflet
- Apache ECharts

### Infrastructure

- Docker
- Docker Compose
- Podman
- Nginx

### Authentication

- Keycloak

### Monitoring

- Prometheus
- Grafana
- Loki

## Use Cases

- Investigative journalism
- Academic research
- Public accountability initiatives
- Government transparency projects
- Policy analysis
- Legal research
- Historical analysis
- Civic technology projects
- Compliance research
- Open data initiatives

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
  - [https://roxanneardary.com/publicenforcer/](https://roxanneardary.com/publicenforcer/)

---

## License & Notice Requirements

PublicEnforcer is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- PublicEnforcer specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
