# VectorMeter

**Compliance Begins With Measurement.**

VectorMeter is an open, modular resource accounting and metering system designed to make compute, time, energy, and digital infrastructure fully measurable, auditable, and verifiable. It serves as the reference implementation for the Open Metering Specification (OMS), enabling deterministic billing, immutable audit trails, and multi-agent compute accountability across AI systems, cloud infrastructure, and physical-world services.

VectorMeter is designed as a foundational layer for any system that requires transparent usage tracking, including AI workloads, internet cafés, coworking spaces, cloud providers, data centers, EV charging networks, and future machine-driven economies.

---

## Core Principles

- Everything measurable is a resource
- Every resource event is recorded
- Every event is immutable
- Every invoice is reproducible
- Every cost is traceable to origin
- Every system action is auditable
- No billing without measurement
- No measurement without verification

---

## Full Feature Specification

### Open Metering Specification (OMS) Compliance
- Full OMS Core compatibility
- OMS event schema implementation
- OMS ledger specification compliance
- OMS billing specification support
- OMS compliance framework integration
- OMS plugin architecture support
- OMS API specification alignment
- OMS governance model support

---

### Immutable Ledger System
- Append-only event ledger
- Cryptographic hash chaining
- Merkle tree verification support
- Digital signature enforcement
- Tamper-evident storage
- Dual-host logging (provider + customer)
- Cross-host reconciliation
- Deterministic replay capability
- Ledger snapshot verification
- Time-synchronized event ordering

---

### Resource Metering Engine
- CPU usage tracking
- GPU usage tracking
- RAM and memory tracking
- Storage usage tracking
- Network bandwidth tracking
- API call tracking
- Tool invocation tracking
- Energy usage estimation
- Time-based resource tracking
- Composite resource aggregation
- Custom resource plugin support

---

### AI Compute Accounting
- Token-level tracking (input/output)
- Reasoning compute tracking
- Hidden reasoning cost accounting
- Context window utilization tracking
- Model invocation logging
- Model version tracking
- RAG pipeline tracking
- Vector database query tracking
- Embedding generation tracking
- Multi-model routing accounting
- Cache hit/miss accounting

---

### Multi-Agent System Accounting
- Per-agent resource breakdown
- Agent hierarchy tracking
- Parent-child agent attribution
- Delegation accounting
- Swarm execution tracking
- Agent lifecycle logging
- Shared resource attribution
- Agent performance metrics
- Parallel execution tracking
- Orchestration cost breakdown

---

### Industry Modules

#### AI / Machine Intelligence
- Full LLM usage metering
- Autonomous workflow tracking
- Tool execution accounting
- Prompt-to-output traceability

#### Internet Café Module
- Seat-based time tracking
- Device usage tracking
- Printing/scanning usage
- Game station usage
- Download/upload tracking
- POS integration support

#### Coworking Module
- Desk and room usage tracking
- Meeting room billing
- Subscription + usage hybrid billing
- Resource reservation tracking

#### Data Center Module
- VM and container usage tracking
- GPU cluster billing
- Storage cluster accounting
- Cooling and power tracking

#### EV Charging Module
- kWh consumption tracking
- Charging time tracking
- Idle fee tracking
- Charger utilization tracking

---

### Billing Engine
- Time-based billing
- Usage-based billing
- Hybrid billing models
- Tiered pricing support
- Dynamic pricing rules
- Peak/off-peak pricing
- Subscription billing integration
- Discount and credit tracking
- Refund and adjustment handling
- Multi-currency support

---

### Pricing Engine
- Rule-based pricing system
- Versioned pricing models
- Resource-weighted billing
- AI cost weighting
- Energy cost weighting
- Customer-specific pricing rules
- Organizational pricing policies
- Market-based pricing plugins

---

### Digital Receipts System
- Cryptographically signed receipts
- Immutable invoice generation
- Full billing breakdown
- Per-agent cost attribution
- Resource provenance in receipts
- QR-based verification
- Public verification endpoints
- Machine-readable receipts (JSON, XML)
- Human-readable receipts (PDF, HTML)
- Ledger-linked invoice reconstruction
- Audit-ready export packages

---

### Audit & Compliance Layer
- Full audit trail generation
- Regulatory compliance profiles
- FTC disclosure support
- State and local compliance modules
- Billing transparency enforcement
- Dispute resolution support
- Evidence package generation
- Legal hold support
- Retention policy enforcement
- Independent verification support

---

### Security Model
- End-to-end encryption
- At-rest encryption
- In-transit encryption
- HSM and TPM support
- Role-based access control
- Multi-tenant isolation
- API authentication layers
- Secure plugin sandboxing
- Signed plugin execution
- Integrity verification checks

---

### Plugin Architecture
- Resource plugins
- Industry-specific plugins
- Billing plugins
- Compliance plugins
- Reporting plugins
- Export plugins
- Authentication plugins
- Marketplace plugin system
- Versioned plugin system
- Signed plugin verification

---

### API System
- REST API support
- Streaming event API
- WebSocket event ingestion
- gRPC compatibility layer
- Batch ingestion API
- Audit query API
- Invoice reconstruction API
- Ledger verification API
- Reconciliation API

---

### Reporting & Analytics
- Usage dashboards
- Cost breakdown reports
- Agent-level analytics
- Resource efficiency metrics
- Predictive cost modeling
- Capacity planning tools
- Compliance reporting exports
- Executive dashboards

---

### Storage Support
- PostgreSQL backend
- SQLite local mode
- MongoDB support
- Redis caching layer
- S3-compatible object storage
- Immutable archive storage
- Distributed ledger storage options

---

### OMS Governance Compliance
- OMS Enhancement Proposal support (OMEP)
- Specification version tracking
- Conformance certification model
- Extension registry support
- Namespace governance rules
- Backward compatibility enforcement
- Deprecation lifecycle management
- Security advisory integration
- Community governance alignment
- Reference implementation validation

---

### Enterprise Features
- Horizontal scalability
- Multi-region deployments
- High availability mode
- Disaster recovery support
- Backup verification system
- Observability integration
- Infrastructure-as-code support
- Kubernetes deployment ready

---

## Philosophy

VectorMeter is built on the belief that:

> If a system cannot measure its own behavior, it cannot be trusted to bill for it.

Every compute event, agent decision, and resource allocation becomes part of a verifiable, reproducible ledger.

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
  - [https://roxanneardary.com/vectormeter/](https://roxanneardary.com/vectormeter/)


---

## License & Notice Requirements

VectorMeter is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Open Arsenal VectorMeter specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
