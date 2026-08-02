# No Lock-In Compliance Standard (NLCS v1.0)

**_Freedom by design, not permission._**

NLCS v1.0 is an open architecture and governance standard designed to eliminate vendor lock-in across AI systems, software infrastructure, and deployment environments. It enforces modular design, full interchangeability, and legal-technical alignment through machine-verifiable compliance rules.

---

## Overview

The No Lock-In Compliance Standard (NLCS v1.0) defines a complete system architecture where every component is:

- Modular
- Replaceable
- Portable across environments
- Independent of vendor ecosystems
- Legally aligned with AGPL 3.0+ distribution requirements

NLCS extends beyond traditional software architecture by integrating:
- AI model abstraction
- Infrastructure independence
- Data portability standards
- Automated compliance validation
- Terms of Service (TOS) governance via AI review systems

---

## Core Principles

- **No Vendor Lock-In:** No dependency on a single provider for system operation
- **Full Modularity:** Every system layer is independently swappable
- **Interface-First Design:** Systems communicate through stable contracts, not implementations
- **Data Sovereignty:** All data must be exportable in open formats
- **Execution Portability:** Systems must run across local, cloud, and edge environments
- **Legal Alignment:** Terms of Service must not contradict architectural independence

---

## Seven-Layer Architecture

NLCS systems are composed of seven interchangeable layers:

### 1. AI / Model Layer
- Swappable AI backends (local, cloud, hybrid)
- Standard inference interface
- Multi-model routing support
- No provider-locked logic

### 2. Orchestration Layer
- Workflow and agent execution engine
- Graph-based or rule-based systems
- Fully replaceable logic layer

### 3. Data Layer
- Database-agnostic design (SQL, NoSQL, file-based)
- Open format enforcement (JSON, CSV, Parquet)
- Schema versioning and migration required

### 4. API / Interface Layer
- Multi-protocol support (REST, GraphQL, CLI, gRPC, events)
- Functional parity across interfaces
- No logic tied to transport layer

### 5. Execution Layer
- Runs in local, cloud, or edge environments
- Docker/Kubernetes compatibility required
- Infrastructure independence enforced

### 6. Identity & Policy Layer
- OAuth2 / OIDC support
- API key fallback systems
- Externalized policy engine
- Optional decentralized identity support

### 7. TOS Governance Layer
- AI-driven Terms of Service evaluation system
- Ensures alignment with NLCS principles
- Detects legal lock-in or restrictive clauses
- Prevents policy-layer vendor dependency

---

## Interchangeability System

NLCS enforces a **Hot Swap Rule**:

Every module must be replaceable without requiring changes to other system layers.

Requirements:
- No cascading refactors
- Interface-only coupling
- No hardcoded external dependencies
- Independent versioning per module

---

## Module Interface Contract

All modules must implement a standard interface:
```text
{
  "module_name": "string",
  "version": "semver",
  "inputs_schema": {},
  "outputs_schema": {},
  "dependencies": [],
  "swap_compatibility": true,
  "fallback_supported": true
}
```
---

## Fallback System Requirement

Every module must include:

- Primary implementation
- Secondary fallback implementation
- Offline/local fallback implementation

No module is considered compliant without graceful degradation support.

---

## Dependency Rules

### Allowed
- Open protocols
- Interface-based services
- Local libraries

### Restricted
- Cloud APIs (must be abstracted)
- Vendor SDKs (cannot be core-dependent)

### Forbidden
- Proprietary-only execution logic
- Non-exportable formats
- Closed ecosystem dependencies

---

## Compliance Tiers

### Level 0 — Non-Compliant
- Vendor lock-in present
- No export capability

### Level 1 — Basic Compliance
- Partial export support
- Limited modular separation

### Level 2 — Portable Systems
- Full export/import support
- Multi-environment execution

### Level 3 — Fully Compliant
- No proprietary dependencies required
- Fully modular architecture
- Offline-capable system
- Complete interchangeability

---

## Machine-Readable Compliance

NLCS systems must expose:

- nlcs.schema.json → structural compliance rules
- nlcs.meta.json → runtime compliance metadata
- nlcs.check → validation tooling interface

---

## TOS AI Governance System

NLCS includes an AI-driven Terms of Service evaluation module that:

- Parses system TOS documents
- Evaluates alignment with NLCS architecture rules
- Detects vendor lock-in clauses
- Flags legal conflicts with modularity or portability
- Produces structured compliance reports

TOS violations may block deployment in Level 3 systems.

---

## Validator System (nlcs-check)

A compliance validation tool that detects:

- Vendor lock-in dependencies
- Missing fallback layers
- Hardcoded external services
- Non-exportable formats
- TOS violations

Integrates with CI/CD pipelines and pre-commit hooks.

---

## Interchangeability Test Suite

Ensures system resilience by validating:

- AI model swapping without breaking functionality
- Database replacement without code changes
- Infrastructure migration without refactoring
- Orchestrator replacement without workflow loss
- TOS changes without compliance violations

---

## Portability Score System

NLCS systems are optionally scored (0–100) based on:

- Module independence
- Vendor neutrality
- Offline capability
- Export completeness
- Runtime flexibility
- Legal/TOS alignment

---

## Deployment Profiles

- NLCS-Lite → Local-only systems
- NLCS-Hybrid → Local + cloud fallback
- NLCS-Distributed → Multi-node systems
- NLCS-Airgap → Fully offline environments

---

## Ecosystem Structure

Recommended repository layout:

/nlcs-project  
  /modules  
  /contracts  
  /adapters  
  /data  
  /policy  
  /tos  
  /tests  
  nlcs.schema.json  
  nlcs.meta.json  
  nlcs.check  
  NLCS_SCORE.md  

---

## Key Feature Summary

- Fully modular AI architecture standard
- Vendor-neutral system design rules
- Swappable AI, storage, and orchestration layers
- Multi-environment portability (local, cloud, edge)
- Machine-readable compliance schema
- Automated CI/CD compliance validation
- AI-driven Terms of Service governance system
- Interchangeability test suite
- Dependency classification system
- Portability scoring framework
- Deployment profile standardization
- AGPL 3.0+ enforced attribution compliance alignment

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
  - [https://roxanneardary.com/no-lock-in-compliance-standard/](https://roxanneardary.com/no-lock-in-compliance-standard/)


---

## License & Notice Requirements

No Lock-In Compliance Standard (NLCS v1.0) is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- No Lock-In Compliance Standard specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.
- Any implementation of the **NLCS v1.0 standard**, including optional compliance modules (such as TOS governance, interchangeability validation, or portability scoring), must preserve the core principles of vendor neutrality, modular replaceability, and exportability unless explicitly disabled in a non-compliant derivative.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
