# RequestStamp

**Built for systems that need answers.**

RequestStamp is a self-hosted edge request identity and decision system that provides transparent request tracing, rule evaluation, and explainable infrastructure behavior. It assigns a unique identity to every request entering your infrastructure, enabling complete visibility into how requests move through distributed systems and why edge decisions are made.

---

# Specification

## Purpose

RequestStamp provides an open, vendor-neutral request identity layer for modern infrastructure. Rather than simply generating request IDs, it establishes a standardized request lifecycle that supports observability, policy enforcement, auditing, and explainability across reverse proxies, APIs, microservices, and distributed applications.

The platform is designed to operate independently or integrate into existing infrastructure while remaining lightweight, transparent, and fully self-hosted.

---

# Design Goals

- Self-hosted
- Open architecture
- Lightweight deployment
- Vendor neutral
- Distributed system ready
- Explainable edge decisions
- Transparent request processing
- Extensible through plugins
- Privacy-first operation
- Standards-based integrations

---

# Modular Design

RequestStamp is composed of independent modules that can operate together or be extended through optional plugins.

## Core Modules

### Request Identity

Responsible for generating and maintaining a unique identity for every request.

Features:

- Unique request ID generation
- Time-ordered identifiers
- Distributed-safe request identities
- Request lifecycle initialization
- Parent-child request relationships
- Request chain propagation
- Standard request headers

---

### Edge Integration

Handles request interception at the infrastructure boundary.

Features:

- Reverse proxy integration
- Middleware support
- Edge request interception
- Minimal processing overhead
- Distributed deployment support
- Service-to-service propagation

---

### Request Enrichment

Adds contextual metadata to requests before evaluation.

Features:

- Route identification
- Service identification
- Client metadata
- User-Agent classification
- Optional IP enrichment
- Optional ASN detection
- Optional geographic information
- Custom metadata pipeline

---

### Rule Engine

Evaluates requests using deterministic policies.

Features:

- Allow/block decisions
- Rate limiting
- Header validation
- Request filtering
- Geographic policies
- Rule priorities
- Configurable rule sets
- YAML or JSON configuration
- Deterministic rule evaluation

---

### Decision Engine

Produces transparent request outcomes.

Features:

- Decision generation
- Rule match recording
- Decision reasoning
- Risk indicators
- Audit events
- Decision metadata
- Request outcome tracking

---

### Request Propagation

Maintains request identity across distributed systems.

Features:

- Cross-service propagation
- Parent request tracking
- Child request tracking
- Distributed request chains
- Correlation support
- Service relationship mapping

---

### Decision Logging

Maintains a structured record of every evaluated request.

Features:

- Structured logging
- Request history
- Rule history
- Decision history
- Audit logging
- Timeline reconstruction
- Export-ready events

---

### Explainability Engine

Converts request evaluations into understandable information.

Features:

- Human-readable explanations
- Decision summaries
- Rule breakdowns
- Evaluation timelines
- Request history analysis
- Debugging assistance
- Transparent reasoning

---

### Configuration Management

Provides centralized system configuration.

Features:

- Modular configuration
- Rule management
- Environment profiles
- Configuration validation
- Hot reload support
- Versioned settings

---

# Optional Plugin Modules

## AI Request Analysis

Provides intelligent analysis of request behavior.

Features:

- Request summaries
- Pattern recognition
- Anomaly explanations
- Operational recommendations
- Incident assistance

---

## Advanced Threat Detection

Extends request analysis with behavioral security.

Features:

- Behavioral analysis
- Threat scoring
- Suspicious activity detection
- Reputation integration
- Adaptive security rules

---

## Advanced WAF Rules

Provides enterprise-grade filtering capabilities.

Features:

- Signature rules
- Custom policies
- Rule packs
- Managed rule updates
- Advanced request inspection

---

## Analytics Dashboard

Provides visualization of request activity.

Features:

- Live request monitoring
- Request timelines
- Decision statistics
- Rule metrics
- Service metrics
- Historical reporting

---

## Replay & Investigation

Allows request lifecycle reconstruction.

Features:

- Request replay
- Timeline visualization
- Decision replay
- Service path reconstruction
- Investigation tools

---

## OpenTelemetry Integration

Exports request information to observability platforms.

Features:

- Trace export
- Metrics export
- Log export
- Correlation support
- Standards compliance

---

## External Log Exporters

Supports third-party logging systems.

Features:

- JSON export
- SIEM integration
- Log streaming
- Custom exporters
- Event forwarding

---

## Notification System

Generates operational notifications.

Features:

- Alert rules
- Email notifications
- Webhooks
- Incident notifications
- Escalation workflows

---

## REST API

Provides programmable access to RequestStamp.

Features:

- Request lookup
- Decision lookup
- Rule management
- Configuration management
- Administrative endpoints

---

## Web Management Console

Browser-based administration interface.

Features:

- Configuration management
- Rule editing
- Request search
- Decision inspection
- System monitoring
- User administration

---

## Multi-Node Coordination

Supports distributed RequestStamp deployments.

Features:

- Cluster awareness
- Shared configuration
- Request synchronization
- High availability
- Distributed coordination

---

## Plugin SDK

Allows developers to extend RequestStamp.

Features:

- Plugin interfaces
- Event hooks
- Custom enrichers
- Custom rules
- Custom exporters
- Documentation
- Version compatibility

---

# Use Cases

RequestStamp is suitable for:

- API gateways
- Reverse proxies
- Edge computing
- Microservices
- Kubernetes environments
- Enterprise applications
- Self-hosted platforms
- Private cloud infrastructure
- Security gateways
- Internal developer platforms

---

# Project Goals

RequestStamp aims to become an open standard for request identity, transparent edge decisioning, and explainable infrastructure. By combining request tracing, policy evaluation, structured logging, and human-readable explanations, it provides organizations with complete visibility into how requests move through their systems and why every edge decision is made.  

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
  - [https://roxanneardary.com/requeststamp/](https://roxanneardary.com/requeststamp/)

---

## License & Notice Requirements

RequestStamp is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- RequestStamp specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
