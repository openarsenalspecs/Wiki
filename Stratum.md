# Stratum  
**Before execution, Stratum.**

Stratum is an AI governance layer for MCP (Model Context Protocol) systems. It sits between model-driven intent and tool execution, enforcing policy, permissions, context controls, approvals, sandboxing, and full auditability before any action is executed.

It is designed as a control plane for autonomous and semi-autonomous AI systems.

---

## Core Features

### 🔐 Permission System
- Role-Based Access Control (RBAC)
- Attribute-Based Access Control (ABAC)
- Fine-grained MCP tool permissions
- Capability-based execution control
- Role + context-aware authorization

---

### ⚖️ Policy Enforcement Engine
- Central Policy Decision Point (PDP)
- Allow / Deny / Modify / Require Approval actions
- Risk-based execution gating
- Dynamic policy evaluation
- Versioned policy definitions

---

### 👁 Context Filtering Layer
- Sensitive data detection and redaction
- Prompt injection filtering
- Context window governance
- Field-level data masking
- Role-based context shaping

---

### 🧑‍⚖️ Approval Workflows
- Human-in-the-loop approval chains
- Multi-stage approvals (L1 / L2 / compliance)
- Time-limited approvals
- Escalation rules for high-risk actions
- Delegated approval authority

---

### 🧪 Execution Sandboxing
- Isolated execution environments for MCP tools
- Container-based sandboxing (Docker)
- Optional microVM support (Firecracker)
- WebAssembly execution option
- Network and filesystem isolation
- Resource limits (CPU, memory, timeout)

---

### 📜 AI Audit Logging
- Append-only audit event stream
- Full traceability of:
  - Prompts
  - Context snapshots (hashed or redacted)
  - Policy decisions
  - Tool invocations
  - Execution results
- Tamper-evident log design (optional hash chaining)
- Queryable audit history API

---

### 📊 Risk Scoring Engine
- Real-time request risk scoring
- Prompt injection risk detection
- Tool risk classification
- Behavioral anomaly detection
- Adaptive enforcement escalation

---

### 🔄 MCP Integration Layer
- Native MCP protocol compatibility
- Middleware layer between agent and MCP tools
- Request interception and transformation
- Execution gating before MCP calls

---

### 🧠 Optional Intelligence Layer
- LLM-assisted context classification
- Semantic policy interpretation
- Adaptive policy suggestions
- Intelligent escalation recommendations

---

## System Architecture

Stratum operates as a layered governance pipeline:

MCP Agent Request  
→ Context Filtering  
→ Identity & Permissions  
→ Policy Decision Engine  
→ Approval Orchestrator (if required)  
→ Execution Sandbox  
→ MCP Tool Execution  
→ Audit Logging Layer  

---

## Suggested Tech Stack

### Core Backend
- TypeScript (Node.js) or Go
- gRPC or REST API layer
- Event-driven architecture

---

### Policy Engine
- Open Policy Agent (OPA)
- Rego policy language
- Optional JSON/YAML DSL abstraction layer

---

### Sandboxing
- Docker for container isolation
- Firecracker for microVM isolation
- WebAssembly runtime for lightweight execution

---

### Data Layer
- PostgreSQL for core state
- Redis for caching and sessions
- Kafka or Redpanda for event streaming (optional)

---

### Observability & Audit
- OpenTelemetry for tracing
- Structured logging system
- Object storage (S3-compatible) for audit logs

---

### Security & Identity
- OAuth2 / OpenID Connect
- JWT authentication
- Vault or cloud KMS for secrets management

---

## Use Cases

- Enterprise AI governance platforms
- MCP tool execution control systems
- Regulated industry AI workflows (finance, healthcare, legal)
- Autonomous agent safety layers
- Multi-agent orchestration systems

---

## Philosophy

Stratum is built on a simple principle:

Intelligence should not act without structure, permission, and traceability.

It defines the boundary between what an AI can decide and what it is allowed to do.

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
  - [https://roxanneardary.com/stratum/](https://roxanneardary.com/stratum/)


---

## License & Notice Requirements

Stratum is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Stratum specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
