# License Guardian Network

Connecting usage, provenance, and compliance.

## Overview

License Guardian Network is a semantic licensing and attribution compliance system designed to track specification usage across distributed systems, verify attribution requirements, and generate structured compliance evidence and notices. The system combines semantic similarity detection, provenance tracking, and modular enforcement workflows to support AGPL-3.0+ ecosystems and optional Specification Branding License (SBL) deployments.

The platform is built as a modular AI infrastructure layer for detecting reuse, mapping specification lineage, and maintaining attribution integrity across networks.

---

## Core Features

### 1. Spec Registry System
- Central registry for licensed specifications
- Stores canonical spec definitions
- Maintains attribution requirements per specification
- Versioned spec tracking and history
- Embeddable metadata for semantic matching

---

### 2. Semantic Similarity Engine
- Vector-based embedding comparison for specifications
- Detects paraphrased, modified, or derivative usage
- Similarity scoring for matched content
- Supports multi-model embedding pipelines
- Configurable threshold-based matching rules

---

### 3. Crawling & Discovery Layer
- Public web content ingestion
- User-submitted URL scanning
- Repository-based ingestion (GitLab, Codeberg, GitHub APIs)
- RSS and structured feed parsing
- Scope-limited crawling (no cross-domain identity tracking)

---

### 4. Attribution Validation Engine
- Detects presence or absence of required attribution
- Validates author name inclusion
- Validates required links and licensing references
- Checks SBL compliance markers
- Generates structured compliance status outputs

---

### 5. Provenance & Evidence Builder
- Creates immutable-style audit records
- Captures source URLs and timestamps
- Stores matched spec IDs and similarity scores
- Generates structured evidence packets
- Exportable for legal and compliance workflows

---

### 6. Legal Notice Generation System
- Automated attribution request notices
- License compliance escalation notices
- Commercial licensing conversion notices (SBL)
- Configurable grace periods and response windows
- Structured legal templates with dynamic variables  

---

### 7. Compliance Intelligence Layer
- Aggregates detection + validation results
- Assigns compliance risk levels
- Tracks unresolved attribution cases
- Maintains enforcement-ready case records
- Supports batch analysis workflows

---

### 8. API & Integration Layer
- RESTful API for spec queries and validation
- Webhook support for compliance alerts
- Export endpoints for audit reports
- Integration-ready JSON schemas
- Modular plugin architecture

---

### 9. Modular Architecture Design
- Fully decoupled microservice-compatible modules
- Independent scaling of crawler, semantic, and legal layers
- Event-driven compliance pipeline
- Pluggable embedding and LLM backends
- AGPL-3.0+ network deployment compliance enforced

---

## System Workflow

1. Specifications are registered in the Spec Registry  
2. Crawling layer discovers potential usage instances  
3. Semantic engine compares content to spec embeddings  
4. Attribution engine validates required credit presence  
5. Evidence builder generates compliance report  
6. Legal module produces structured notice if required  
7. Optional SBL module handles commercial licensing pathway  

---

## Output Types

- Compliance Reports (JSON)
- Evidence Packs (Audit-ready bundles)
- Attribution Notices (Legal templates)
- Similarity Scores (semantic matching output)
- Spec lineage graphs (provenance mapping)

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
  - [https://roxanneardary.com/license-guardian-network/](https://roxanneardary.com/license-guardian-network/)  

---

## License & Notice Requirements

License Guardian Network is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Open Arsenal License Guardian Network specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
