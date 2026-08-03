# ThreadGraph

**Swarm logic, graph-structured.**

ThreadGraph is an open-source, AGPL-3.0+ modular agent swarm runtime that transforms complex tasks into executable, graph-based workflows. It replaces linear AI chains with structured, parallel, and observable execution graphs composed of modular agents, tools, memory systems, and schedulers.

---

## Overview

Modern agent systems are often fragile, linear, and difficult to debug. ThreadGraph introduces a fundamentally different approach: **execution as a graph of interconnected threads**, where every task is decomposed into modular, parallelizable components.

Instead of relying on single-agent reasoning or rigid pipelines, ThreadGraph orchestrates swarms of specialized agents through a deterministic graph runtime.

---

## Core Philosophy

- Intelligence should be composable
- Execution should be graph-structured
- Agents should be modular
- Workflows should be observable
- Systems should be reproducible

---

## Key Features

### 1. Swarm-Based Execution Runtime
- Multi-agent swarm orchestration per task
- Planner, worker, and critic role separation
- Dynamic agent spawning based on task complexity
- Parallel execution of reasoning branches
- Swarm coordination with conflict resolution
- Confidence scoring and output arbitration

---

### 2. Graph-Structured Execution Engine
- All tasks compiled into executable graphs (DAG-based)
- Dynamic graph expansion at runtime
- Node types:
  - Agent nodes
  - Tool nodes
  - Memory nodes
  - Router nodes
- Dependency-aware scheduling
- Parallel branch execution by default
- Graph pruning and optimization
- Fully replayable execution graphs

---

### 3. Modular Agent System
- Plugin-based agent architecture
- Standardized agent input/output interfaces
- Role-based agent definitions (planner, researcher, coder, critic, analyzer)
- Hot-swappable agents at runtime
- Per-agent model selection (small vs large models)
- Capability-based agent permissions
- Versioned agent modules

---

### 4. Tool Plugin Framework
- External tool registry system
- JSON schema-based tool contracts
- Secure tool execution sandboxing
- Built-in tool support:
  - Web search
  - File system access
  - Code execution
  - API requests
  - Database queries
- Tool routing via kernel, not agents directly
- Retry and fallback execution logic
- Community extensible tool SDK

---

### 5. Scheduler & Orchestration Layer
- Pluggable execution strategies
- Supported modes:
  - Sequential execution
  - Parallel swarm execution
  - Map-reduce execution
  - Debate-based reasoning
  - Critic-loop validation
- Runtime scheduler switching
- Cost-aware execution planning
- Adaptive execution depth control
- Priority-based task scheduling

---

### 6. Memory System
- Multi-layer memory architecture:
  - Episodic memory (task history)
  - Semantic memory (facts and knowledge)
  - Procedural memory (execution patterns)
- Pluggable storage backends:
  - In-memory (development mode)
  - Persistent storage (SQLite/file-based)
  - Vector database support
- Memory retrieval APIs:
  - Contextual search
  - Graph-linked retrieval
  - Summarization and compression
- Cross-task memory linking
- Memory versioning and audit trail

---

### 7. Execution Graph Observability
- Full execution graph visualization
- Node-level tracing and inspection
- Live execution monitoring dashboard
- Step-by-step replay mode
- Branch comparison tools
- Token and cost tracking per node
- Performance profiling per agent/tool
- Failure inspection and debugging tools

---

### 8. Dynamic Task Decomposition
- Automatic task breakdown into subgraphs
- Recursive decomposition engine
- Complexity-based branching logic
- Dynamic stopping condition detection
- Redundancy elimination between branches
- Graph merging and synthesis of subtasks

---

### 9. Result Synthesis Engine
- Multi-agent output aggregation
- Conflict resolution between outputs
- Confidence-weighted merging
- Deduplication of redundant results
- Multi-perspective synthesis
- Final validation and critique pass

---

### 10. Developer API & SDK
- Simple API surface:
  - swarm.run(task)
  - swarm.define_graph()
  - swarm.add_agent()
  - swarm.add_tool()
- Python and TypeScript SDK support
- Plugin Development Kit (PDK)
- CLI interface for local execution
- Docker-based deployment support
- Headless server mode

---

### 11. Performance Optimization
- Token-aware execution planning
- Lightweight routing layer for task delegation
- Lazy agent instantiation
- Parallel execution throttling
- Execution caching for repeated subgraphs
- Adaptive model selection per node

---

### 12. Security & Control Layer
- Sandboxed tool execution environment
- Permission-based agent capabilities
- Execution isolation per task graph
- Full audit logging
- Deterministic execution mode for verification
- Replayable workflows for compliance

---

### 13. Plugin Ecosystem
- Open plugin registry
- Community-built agent modules
- Tool ecosystem extensibility
- Scheduler plugins
- Memory backend plugins
- Shareable swarm templates

---

### 14. Built-in Swarm Templates
- Research swarm (multi-source synthesis)
- Coding swarm (debugging and refactoring)
- Analysis swarm (data breakdown and reporting)
- OSINT swarm (structured information gathering)
- Planning swarm (decision graph exploration)
- Document processing swarm (summarization and extraction)

---

## Architecture Summary

ThreadGraph is composed of:

- A **Swarm Runtime Kernel**
- A **Graph Execution Engine**
- A **Modular Agent System**
- A **Tool Plugin Framework**
- A **Memory Abstraction Layer**
- A **Scheduler Orchestration System**

All components are independently swappable and extensible.

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
  - [https://roxanneardary.com/threadgraph/](https://roxanneardary.com/threadgraph/)

---

## License & Notice Requirements

ThreadGraph is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- ThreadGraph specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
