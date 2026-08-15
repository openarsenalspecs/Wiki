# Ralph Workflow Specification
- HTML Mirror:  [https://roxanneardary.com/ralph-workflow-specification/](https://roxanneardary.com/ralph-workflow-specification/)

---

## Overview

Ralph Workflow is a modular CLI-based AI development orchestration framework designed for long-running, unattended software engineering workflows.

The system enables developers to define a complete feature specification in `PROMPT.md`, execute Ralph Workflow, and allow autonomous AI agents to plan, implement, review, refine, and commit changes through repeatable development cycles.

Ralph Workflow is designed around deterministic automation, structured specifications, and human-defined goals. It does not function as an interactive assistant that continuously asks questions. Instead, it relies on detailed specifications, allowing AI agents to execute complex engineering tasks with minimal intervention.

The more complete and precise the project specification, architecture requirements, acceptance criteria, and implementation details are, the more effective Ralph Workflow becomes.

Ralph Workflow is inspired by the Ralph workflow concept created by Geoffrey Huntley.

---

# Design Philosophy

Ralph Workflow is built around the principle that AI development systems should maximize deterministic decisions while using AI reasoning where ambiguity or complex judgment is required.

The workflow separates:

- Specification
- Planning
- Implementation
- Validation
- Review
- Correction
- Delivery

This creates repeatable development cycles where every change can be tracked, reviewed, and improved.

Ralph Workflow is optimized for:

- Large feature development
- Long-running coding tasks
- Multi-agent development pipelines
- Automated refactoring
- Repository maintenance
- Structured software evolution

It is designed for developers who approach AI-assisted development like product managers by defining clear requirements, expected behavior, and implementation constraints.

---

# Modular Architecture

Ralph Workflow is organized into a modular architecture consisting of:

- Core Modules
- Optional Plugin Modules
- External AI Agent Integrations
- Repository Intelligence Services

The core system provides the complete autonomous workflow engine. Optional plugins extend Ralph Workflow with additional capabilities without changing the underlying workflow architecture.

---

# Core Modules

## Workflow Orchestration Module

The Workflow Orchestration Module manages the complete autonomous development lifecycle.

Capabilities:

- Execute long-running development workflows
- Manage workflow states
- Coordinate planning, implementation, review, and correction cycles
- Maintain workflow history
- Resume interrupted workflows
- Support unattended execution

---

## Specification Input Module

The Specification Input Module converts human-defined requirements into structured development objectives.

Capabilities:

- Read `PROMPT.md` specifications
- Define feature goals
- Capture implementation requirements
- Maintain project context
- Provide structured instructions to AI agents

The quality of the specification directly affects workflow success.

Detailed specifications reduce ambiguity and allow autonomous agents to make consistent decisions.

---

## Planning Engine Module

The Planning Engine creates structured implementation plans before code changes begin.

Capabilities:

- Analyze feature requirements
- Generate implementation strategies
- Identify required files and components
- Create development plans
- Produce structured planning documents

Planning output becomes the foundation for the implementation cycle.

---

## AI Development Agent Module

The AI Development Agent Module manages coding agents responsible for implementing planned changes.

Capabilities:

- Modify source code
- Create new files
- Refactor existing components
- Execute development tasks
- Run validation commands
- Track implementation progress
- Generate commits

Supported agent integrations include:

- Claude Code
- OpenAI Codex CLI
- OpenCode

Additional AI providers can be integrated through plugin modules.

---

## Review Agent Module

The Review Agent Module provides automated code review and quality analysis.

Capabilities:

- Analyze code changes
- Review Git diffs
- Identify potential issues
- Detect architectural problems
- Generate review reports
- Provide corrective recommendations

The review phase allows a separate AI agent to evaluate implementation quality.

---

## Correction Cycle Module

The Correction Cycle Module manages iterative improvement after reviews.

Capabilities:

- Process review findings
- Assign corrections to development agents
- Repeat implementation and review cycles
- Track unresolved issues
- Stop when quality requirements are satisfied

Workflows continue until:

- Review issues are resolved
- Maximum cycle limits are reached
- Completion criteria are satisfied

---

## Git Integration Module

The Git Integration Module manages repository operations.

Capabilities:

- Track modifications
- Create commits
- Generate commit messages
- Manage development branches
- Support Git worktree workflows

Ralph Workflow is designed to work effectively with separate Git worktrees, allowing multiple autonomous development tasks to run simultaneously.

---

## Repository Intelligence Module

The Repository Intelligence Module provides codebase understanding capabilities.

Capabilities:

- Scan repositories
- Extract source symbols
- Generate structured indexes
- Build project metadata
- Support future semantic search systems
- Improve AI context retrieval

Example output:

.agent/index/symbols.json

The repository index provides structured information about:

- Files
- Programming languages
- Classes
- Functions
- Structures
- Symbols
- Code relationships

---

## Configuration Module

The Configuration Module manages system behavior and integrations.

Capabilities:

- Configure AI providers
- Define workflow settings
- Manage execution preferences
- Configure repository behavior
- Store user environment settings

Default configuration location:

$HOME/.config/ralph-workflow.toml

---

# Optional Plugin Modules

## Semantic Search Plugin

Provides advanced code understanding capabilities.

Features:

- Semantic source search
- AI-powered context retrieval
- Code relationship mapping
- Dependency discovery
- Architecture exploration

---

## Additional AI Provider Plugin

Extends Ralph Workflow with additional AI agent providers.

Features:

- Custom model integrations
- Local AI model support
- Enterprise AI services
- Private AI deployments

---

## Enterprise Governance Plugin

Adds organizational controls for large deployments.

Features:

- Approval workflows
- Audit logging
- Team permissions
- Policy enforcement
- Compliance reporting

---

## Continuous Integration Plugin

Connects Ralph Workflow with automated build systems.

Features:

- Automated testing
- Build validation
- Deployment checks
- CI/CD pipeline integration

---

## Project Management Plugin

Connects specifications with project management systems.

Features:

- Issue tracking integration
- Sprint planning support
- Task synchronization
- Feature tracking

---

## Knowledge Base Plugin

Provides persistent project knowledge storage.

Features:

- Architecture documentation
- Development history
- Engineering decisions
- Agent memory storage

---

# Workflow Architecture

The Ralph Workflow lifecycle:

Specification Input

PROMPT.md

↓

Planning Phase

Creates structured implementation plan

↓

Development Phase

AI agents:

- Modify code
- Execute tasks
- Run validations
- Commit progress

↓

Review Phase

AI reviewer analyzes:

- Git changes
- Current implementation
- Project requirements

↓

Correction Phase

Development agents resolve identified issues

↓

Final Commit

Creates completed repository update

↓

Updated Project  

---
# Workflow Diagram
```
                         RALPH WORKFLOW ARCHITECTURE

                              ┌─────────────────────┐
                              │      Developer       │
                              │ Product Requirements │
                              │ Architecture Goals   │
                              │ Acceptance Criteria  │
                              └──────────┬──────────┘
                                         │
                                         ▼
                              ┌─────────────────────┐
                              │   Specification     │
                              │      Module         │
                              │                     │
                              │  PROMPT.md          │
                              │  Feature Goals      │
                              │  Requirements       │
                              │  Constraints       │
                              └──────────┬──────────┘
                                         │
                                         ▼
                    ┌────────────────────────────────────────┐
                    │          Workflow Orchestration       │
                    │              Core Module              │
                    │                                        │
                    │  • Workflow State Management          │
                    │  • Execution Control                  │
                    │  • Cycle Management                   │
                    │  • Agent Coordination                │
                    └───────────────┬────────────────────────┘
                                    │
                                    ▼

                         ┌─────────────────────┐
                         │   Planning Engine    │
                         │     Core Module      │
                         │                      │
                         │ • Analyze Request    │
                         │ • Create Plan        │
                         │ • Identify Changes   │
                         │ • Generate PLAN.md   │
                         └──────────┬──────────┘
                                    │
                                    ▼

                    ┌────────────────────────────────┐
                    │       AI Agent Runtime         │
                    │          Core Module           │
                    │                                │
                    │ ┌────────────────────────────┐ │
                    │ │ Development Agent          │ │
                    │ │                            │ │
                    │ │ • Write Code              │ │
                    │ │ • Refactor Components     │ │
                    │ │ • Add Features            │ │
                    │ │ • Run Commands            │ │
                    │ └─────────────┬──────────────┘ │
                    │               │                │
                    │               ▼                │
                    │ ┌────────────────────────────┐ │
                    │ │ External AI Providers     │ │
                    │ │                            │ │
                    │ │ • Claude Code              │ │
                    │ │ • OpenAI Codex CLI         │ │
                    │ │ • OpenCode                 │ │
                    │ │ • Custom Providers         │ │
                    │ └────────────────────────────┘ │
                    └───────────────┬────────────────┘
                                    │
                                    ▼

                    ┌────────────────────────────────┐
                    │       Repository Engine         │
                    │          Core Module            │
                    │                                │
                    │ • File Operations              │
                    │ • Git Integration              │
                    │ • Branch Management            │
                    │ • Commit Creation              │
                    │ • Worktree Support             │
                    └───────────────┬────────────────┘
                                    │
                                    ▼

                         ┌─────────────────────┐
                         │   Validation Phase  │
                         │    Core Module      │
                         │                     │
                         │ • Run Tests         │
                         │ • Check Builds      │
                         │ • Verify Changes    │
                         │ • Measure Progress  │
                         └──────────┬──────────┘
                                    │
                                    ▼

                    ┌────────────────────────────────┐
                    │        Review Engine            │
                    │          Core Module            │
                    │                                │
                    │ Independent Review Agent        │
                    │                                │
                    │ Reviews:                        │
                    │ • Git Diff                      │
                    │ • Source Code                   │
                    │ • Architecture                  │
                    │ • Requirements                  │
                    │                                │
                    │ Produces:                       │
                    │ • ISSUES.md                     │
                    └───────────────┬────────────────┘
                                    │
                                    ▼

                         ┌─────────────────────┐
                         │   Correction Cycle  │
                         │    Core Module      │
                         │                     │
                         │ • Process Issues    │
                         │ • Request Fixes     │
                         │ • Repeat Workflow   │
                         │ • Track Completion  │
                         └──────────┬──────────┘
                                    │
                       ┌────────────┴────────────┐
                       │                         │
                       ▼                         ▼

            ┌───────────────────┐       ┌───────────────────┐
            │ Issues Remaining  │       │  Quality Passed   │
            │                   │       │                   │
            │ Return to Agent   │       │ Continue Release  │
            └─────────┬─────────┘       └─────────┬─────────┘
                      │                           │
                      └───────────────┐           │
                                      │           ▼
                                      │  ┌────────────────────┐
                                      │  │  Final Commit      │
                                      │  │  Core Module       │
                                      │  │                    │
                                      │  │ • Commit Message   │
                                      │  │ • Repository Save  │
                                      │  └─────────┬──────────┘
                                      │            │
                                      │            ▼
                                      │  ┌────────────────────┐
                                      │  │ Updated Repository │
                                      │  │                    │
                                      │  │ Completed Feature  │
                                      │  │ Version History    │
                                      │  └────────────────────┘
                                      │
                                      └───────────────┐
                                                      │
                                                      ▼
                                             New Workflow Cycle



                 OPTIONAL PLUGIN EXTENSION ARCHITECTURE


                         ┌──────────────────────┐
                         │   Ralph Workflow     │
                         │     Core System      │
                         └──────────┬───────────┘
                                    │
              ┌─────────────────────┼─────────────────────┐
              │                     │                     │
              ▼                     ▼                     ▼

 ┌────────────────────┐  ┌────────────────────┐  ┌────────────────────┐
 │ Semantic Search    │  │ Enterprise         │  │ CI/CD Integration  │
 │ Plugin             │  │ Governance Plugin  │  │ Plugin             │
 │                    │  │                    │  │                    │
 │ • Code Search      │  │ • Approvals        │  │ • Build Checks     │
 │ • Context Engine   │  │ • Auditing         │  │ • Deployments      │
 │ • Dependencies     │  │ • Policies        │  │ • Automation       │
 └────────────────────┘  └────────────────────┘  └────────────────────┘


 ┌────────────────────┐  ┌────────────────────┐  ┌────────────────────┐
 │ AI Provider        │  │ Project Management │  │ Knowledge Base     │
 │ Plugin             │  │ Plugin             │  │ Plugin             │
 │                    │  │                    │  │                    │
 │ • Local Models     │  │ • Issues           │  │ • Decisions        │
 │ • Private Models   │  │ • Tasks            │  │ • Documentation    │
 │ • Custom Agents    │  │ • Planning         │  │ • History          │
 └────────────────────┘  └────────────────────┘  └────────────────────┘



                 AGENT CONTEXT FLOW


        PROMPT.md
            │
            ▼
     ┌───────────────┐
     │ Specification │
     └───────┬───────┘
             │
             ▼
     ┌───────────────┐
     │ Planning Data │
     └───────┬───────┘
             │
             ▼
     ┌───────────────┐
     │ Agent Context │
     │ Construction  │
     └───────┬───────┘
             │
             ▼
     ┌───────────────┐
     │ Code Changes  │
     └───────┬───────┘
             │
             ▼
     ┌───────────────┐
     │ Review Context│
     └───────┬───────┘
             │
             ▼
     ┌───────────────┐
     │ Improvements  │
     └───────────────┘

```

Ralph Workflow Core Principles:

1. Humans define intent.
2. Specifications define requirements.
3. AI agents execute implementation.
4. Independent agents review changes.
5. Automation manages repetition.
6. Humans retain control over critical decisions.

---

# Recommended Usage

Ralph Workflow works best when:

- Features are fully specified before execution
- Development tasks are isolated
- Git worktrees are used for parallel development
- Review agents are separated from implementation agents
- Human engineers review final output

Recommended workflow:

1. Create a detailed feature specification
2. Run Ralph Workflow in an isolated worktree
3. Allow autonomous implementation
4. Review generated changes
5. Merge completed work

---

# Human-in-the-Loop Development

Although Ralph Workflow supports unattended execution, human oversight remains an important part of professional software development.

Recommended human checkpoints:

- Architecture decisions
- Security-sensitive changes
- Database modifications
- Production deployments
- Final feature approval

Ralph Workflow automates execution while keeping humans responsible for product direction and critical decisions.

---

# Supported AI Clients

Currently supported integrations:

Claude Code

OpenAI Codex CLI

OpenCode

Additional providers may be added through plugin modules.


---

## 🆕 Recent Additions

The features below are released under **AGPL 3.0+** and require attribution to **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
Please see `notice.md` for full contributor details.

- **Architecture Diagram** – Added a detailed ASCII diagram showing Ralph's multi-phase workflow, agent context isolation, and internal workspace structure. Helps new users understand the orchestration pipeline clearly.

- **Semantic Code Search (Context Engine)** – Proposed and designed the initial indexing module for semantic code search, including symbol extraction and CLI integration (`ralph index`) to improve context retrieval for AI agents.

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
  - [https://roxanneardary.com/ralph-workflow/](https://roxanneardary.com/ralph-workflow/)

---

## License & Notice Requirements

Ralph Workflow is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Open Arsenal Ralph Workflow specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request. [https://roxanneardary.com/ralph-workflow/](https://roxanneardary.com/ralph-workflow/)
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
