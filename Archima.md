# Archima

## Build What You Imagine.

Archima is an open source AI architectural intelligence specification for co-creating buildings from initial architectural vision through detailed, coordinated, and buildable design documentation. Archima enables architects, designers, engineers, builders, homeowners, and other authorized users to collaborate with an AI Large Language Model across the complete architectural design process.

Archima is designed to transform natural language, sketches, references, spatial requirements, existing plans, site information, and architectural concepts into coordinated architectural systems. The specification supports 2D drawings, 3D models, architectural renderings, building schematics, structural systems, mechanical systems, electrical systems, plumbing systems, materials, assemblies, construction details, regulatory constraints, and project documentation.

The canonical source of truth is the structured architectural model rather than an individual rendering or drawing. All generated views, documentation, schedules, analyses, and representations should remain connected to the underlying model so that changes can propagate throughout the project.

Archima is modular by design. Core modules provide the foundational intelligence required for architectural co-creation, while optional plugin modules extend the system into specialized architectural styles, engineering disciplines, regulatory jurisdictions, analysis systems, construction workflows, visualization environments, and external data sources.

## Specification Goals

Archima is designed to:

- Translate architectural vision into structured design requirements.
- Co-create designs with architects and other authorized users.
- Preserve the architect's design intent throughout the project.
- Generate and maintain parametric architectural models.
- Produce coordinated 2D architectural drawings.
- Produce editable 3D building models.
- Generate architectural renderings from the underlying building model.
- Support a comprehensive library of architectural styles.
- Design residential, commercial, institutional, industrial, agricultural, recreational, and specialized structures.
- Support unconventional structures including underground buildings, bunkers, earth-sheltered structures, rooftop structures, off-grid buildings, and disaster-resistant structures.
- Generate architectural and building system schematics.
- Coordinate architecture, structure, MEP, site systems, and construction assemblies.
- Adapt designs to geographic zoning and regulatory requirements.
- Validate designs against configurable constraints.
- Track design decisions, revisions, approvals, and provenance.
- Generate construction documentation from the coordinated model.
- Support open source, vendor-neutral interoperability.
- Allow specialized capabilities to be added through optional plugins.
- Keep humans responsible for professional review, approval, permitting, and construction decisions.

## Core Design Principles

### Architectural Intent First

Archima treats the architect's vision as a primary project artifact. The system must distinguish between explicit requirements, inferred preferences, AI-generated suggestions, accepted decisions, rejected alternatives, and unresolved questions.

The system should preserve the reasoning and intent behind major design decisions so that later modifications do not unintentionally eliminate important characteristics of the original concept.

### Model as the Source of Truth

Renderings, drawings, schedules, and documentation should be generated from a structured building model whenever technically possible.

A change to the building model should be capable of propagating to all affected representations.

### Parametric Design

Building components should be represented as structured objects with properties, relationships, dimensions, materials, constraints, and dependencies.

The system should support parametric relationships between:

- Spaces
- Walls
- Floors
- Ceilings
- Roofs
- Doors
- Windows
- Stairs
- Foundations
- Structural components
- Mechanical systems
- Electrical systems
- Plumbing systems
- Fire protection systems
- Site elements
- Materials
- Assemblies
- Fixtures
- Equipment
- Construction details

### Human Controlled Co-Creation

Archima should function as a co-creator rather than an autonomous replacement for professional architectural and engineering judgment.

Users must be able to accept, reject, modify, compare, annotate, and restore AI-generated design decisions.

### Modular Extensibility

Core architectural capabilities must remain independent from optional specialty capabilities.

Plugins should be able to add new styles, jurisdictions, analysis engines, engineering capabilities, visualization systems, data sources, and workflows without requiring changes to the fundamental Archima model.

### Open Source Interoperability

Archima should favor open standards, documented interfaces, vendor-neutral data formats, and interoperable building information models.

The specification should support integration with openBIM workflows and IFC where appropriate.

## Core Modules

## Architectural Vision & Intent Module

The Architectural Vision & Intent Module converts human architectural concepts into structured project requirements.

It accepts:

- Natural language descriptions
- Conversational instructions
- Sketches
- Images
- Reference photographs
- Existing floor plans
- Existing building models
- Site information
- Material references
- Architectural precedents
- Spatial requirements
- Functional requirements
- Aesthetic requirements
- Performance requirements

The module identifies:

- Project objectives
- Design priorities
- Required spaces
- Desired relationships
- Architectural character
- Materials
- Building scale
- Environmental preferences
- Functional requirements
- Constraints
- Preferences
- Explicit exclusions
- Unresolved decisions

The system must distinguish between user-provided requirements and AI inferences.

## Architectural Co-Creation Module

The Architectural Co-Creation Module allows users and AI to develop architectural concepts collaboratively.

The AI can propose:

- Floor-plan alternatives
- Building massing
- Circulation systems
- Room configurations
- Exterior forms
- Roof configurations
- Courtyards
- Outdoor spaces
- Material palettes
- Façade concepts
- Structural concepts
- Building system concepts
- Alternative site configurations

Each alternative should maintain its relationship to the project requirements and architectural intent.

Users must be able to compare alternatives and preserve rejected concepts for future reference.

## Design Memory Module

The Design Memory Module maintains persistent project knowledge.

It records:

- Architectural intent
- Requirements
- User preferences
- Approved decisions
- Rejected decisions
- Design alternatives
- Design rationale
- Project constraints
- Materials
- Dimensions
- Spatial relationships
- Regulatory assumptions
- Engineering assumptions
- Open questions
- Review comments
- Revision history

The system should prevent previously rejected design decisions from being silently reintroduced unless explicitly reconsidered.

## Architectural Style Intelligence Module

The Architectural Style Intelligence Module provides a structured library of architectural styles and design characteristics.

The library should support:

- Historical styles
- Classical styles
- Vernacular architecture
- Regional architecture
- Indigenous architectural traditions
- Colonial styles
- Revival styles
- Modernism
- Postmodernism
- Contemporary architecture
- Minimalism
- Brutalism
- Art Deco
- Art Nouveau
- Mediterranean architecture
- Tropical architecture
- Desert architecture
- Mountain architecture
- Coastal architecture
- Industrial architecture
- Futuristic architecture
- Experimental architecture
- Hybrid styles

Each style definition may include:

- Historical context
- Geographic context
- Form characteristics
- Massing
- Proportions
- Roof forms
- Window patterns
- Door characteristics
- Materials
- Ornamentation
- Interior characteristics
- Landscape relationships
- Structural tendencies
- Environmental strategies
- Common building typologies

Style plugins should allow additional architectural traditions to be added without modifying the core system.

## Program & Spatial Planning Module

The Program & Spatial Planning Module converts functional requirements into a structured spatial program.

It manages:

- Rooms
- Spaces
- Functions
- Occupancy
- Adjacencies
- Circulation
- Privacy
- Accessibility
- Storage
- Service areas
- Mechanical spaces
- Utility spaces
- Vertical circulation
- Outdoor spaces
- Shared spaces
- Required clearances

The system should understand relationships such as:

- Must be adjacent
- Should be adjacent
- Must be separated
- Preferably separated
- Direct access required
- Visual connection desired
- Acoustic separation required
- Service access required

## Parametric Building Model Module

The Parametric Building Model Module provides the canonical representation of the building.

The model should represent:

- Building sites
- Buildings
- Levels
- Spaces
- Building elements
- Assemblies
- Materials
- Components
- Systems
- Equipment
- Fixtures
- Structural elements
- MEP elements
- Landscape elements
- Regulatory constraints

Each object should support structured metadata, geometry, relationships, properties, and dependencies.

## Geometry & Spatial Reasoning Module

The Geometry & Spatial Reasoning Module provides geometric reasoning for architectural objects and relationships.

It should support:

- Dimensions
- Coordinates
- Planes
- Volumes
- Surfaces
- Intersections
- Clearances
- Offsets
- Angles
- Curves
- Slopes
- Levels
- Building envelopes
- Spatial boundaries
- Collision detection
- Geometric constraints

The module should identify impossible or contradictory geometry before producing construction documentation.

## 2D Documentation Module

The 2D Documentation Module generates coordinated architectural drawings from the building model.

Supported outputs should include:

- Site plans
- Floor plans
- Roof plans
- Foundation plans
- Reflected ceiling plans
- Elevations
- Sections
- Enlarged plans
- Wall sections
- Construction details
- Interior elevations
- Accessibility diagrams
- Life safety diagrams
- Architectural diagrams

The system should automatically maintain:

- Dimensions
- Tags
- Callouts
- Legends
- Sheet references
- Room names
- Room numbers
- Door tags
- Window tags
- Material references
- Drawing scales
- Drawing titles
- Revision information

## 3D Modeling Module

The 3D Modeling Module generates an editable three-dimensional representation of the architectural model.

It should support:

- Building massing
- Interior spaces
- Exterior architecture
- Structural elements
- Building systems
- Materials
- Furniture
- Fixtures
- Landscape
- Site elements
- Lighting
- Terrain

The 3D model must remain connected to the underlying parametric model.

## Rendering & Visualization Module

The Rendering & Visualization Module produces visual representations from the architectural model.

Supported visualization modes should include:

- Conceptual rendering
- Photorealistic rendering
- Interior rendering
- Exterior rendering
- Aerial views
- Street views
- Daytime views
- Nighttime views
- Material studies
- Lighting studies
- Sectional perspectives
- Exploded views
- Axonometric views
- Orthographic views
- Virtual reality environments

Rendered imagery must not be treated as evidence that a design is technically viable.

## Building Envelope Module

The Building Envelope Module manages exterior building assemblies.

It supports:

- Exterior walls
- Interior walls
- Insulation
- Air barriers
- Vapor control
- Waterproofing
- Roofing
- Windows
- Doors
- Curtain walls
- Cladding
- Exterior finishes
- Thermal breaks
- Drainage
- Flashing
- Weather protection

The module should track assembly relationships and required performance properties.

## Structural Design Module

The Structural Design Module coordinates architectural design with structural systems.

It supports conceptual modeling of:

- Foundations
- Footings
- Slabs
- Beams
- Columns
- Load-bearing walls
- Structural frames
- Roof structures
- Retaining walls
- Connections
- Bracing
- Structural assemblies

The system should identify structural conflicts and flag calculations requiring qualified structural engineering review.

## Mechanical Systems Module

The Mechanical Systems Module coordinates building mechanical systems.

It supports:

- HVAC systems
- Equipment
- Ductwork
- Mechanical rooms
- Ventilation
- Exhaust
- Air distribution
- Controls
- Service clearances
- Equipment access

## Electrical Systems Module

The Electrical Systems Module supports conceptual and coordinated electrical design.

It includes:

- Electrical service
- Distribution
- Panels
- Circuits
- Receptacles
- Lighting
- Switches
- Emergency systems
- Communications
- Low-voltage systems
- Equipment connections
- Renewable energy systems
- Energy storage systems

## Plumbing & Water Systems Module

The Plumbing & Water Systems Module supports:

- Domestic water
- Hot water
- Sanitary drainage
- Stormwater
- Fixtures
- Pumps
- Tanks
- Water treatment
- Irrigation
- Graywater systems
- Rainwater systems

## Fire & Life Safety Module

The Fire & Life Safety Module supports conceptual coordination of:

- Egress
- Exit access
- Exit systems
- Fire separations
- Fire-rated assemblies
- Fire detection
- Fire suppression
- Emergency lighting
- Fire access
- Occupancy information

The module should identify areas requiring jurisdictional or professional verification.

## Site & Environmental Module

The Site & Environmental Module integrates the building with its physical environment.

It supports:

- Site boundaries
- Topography
- Terrain
- Orientation
- Solar exposure
- Views
- Access
- Driveways
- Parking
- Landscaping
- Drainage
- Utilities
- Existing structures
- Vegetation
- Outdoor spaces
- Pools
- Patios
- Terraces
- Retaining systems

## Geographic Zoning & Regulatory Adaptation Module

The Geographic Zoning & Regulatory Adaptation Module allows architectural designs to be evaluated and modified according to geographic zoning laws and applicable regulatory requirements.

The module must support hierarchical geographic profiles including:

- Country
- State or province
- County
- Municipality
- Planning jurisdiction
- Zoning district
- Overlay district
- Special district
- Historic district
- Parcel-specific constraints

Regulatory profiles may define:

- Permitted uses
- Conditional uses
- Lot dimensions
- Setbacks
- Building envelopes
- Maximum height
- Floor-area ratio
- Lot coverage
- Density
- Dwelling-unit limits
- Parking requirements
- Accessory structures
- Accessory dwelling units
- Rooftop structures
- Pools
- Fences
- Landscaping
- Impervious surface limits
- Easements
- Environmental restrictions
- Flood requirements
- Coastal restrictions
- Historic restrictions
- Fire access
- Accessibility requirements
- Energy requirements
- Local amendments
- Other jurisdiction-specific requirements

The module must be capable of adapting an existing architectural model to a target jurisdiction.

For example, a design may be imported and evaluated against a new jurisdiction. The system can identify conflicts and propose modifications to:

- Building footprint
- Building height
- Setbacks
- Floor count
- Roof form
- Parking
- Outdoor structures
- Lot coverage
- Building envelope
- Site organization
- Circulation
- Room organization

Every regulatory modification must be traceable to the rule that caused the modification.

The module should maintain:

- Regulatory source
- Jurisdiction
- Effective date
- Version
- Rule identifier
- Applicability
- Confidence
- Verification status

Conflicting requirements must be surfaced rather than silently resolved.

The module should support regulatory change monitoring so that updated zoning requirements can be applied to existing projects.

The system should also support comparative design scenarios where one architectural concept is adapted to multiple jurisdictions.

Regulatory analysis and adaptation must not be represented as legal approval. Final zoning, permitting, code, and construction determinations remain subject to the applicable authority and qualified professionals.

## Building Code & Compliance Module

The Building Code & Compliance Module provides configurable analysis against building and safety requirements.

It should support:

- Occupancy
- Construction type
- Height
- Area
- Egress
- Accessibility
- Fire safety
- Structural requirements
- Energy requirements
- Plumbing requirements
- Mechanical requirements
- Electrical requirements
- Local amendments

Code rules should remain separate from the architectural model and be versioned independently.

## Construction Assembly Module

The Construction Assembly Module translates building components into constructible assemblies.

It supports:

- Wall assemblies
- Floor assemblies
- Roof assemblies
- Foundation assemblies
- Door assemblies
- Window assemblies
- Interior partitions
- Exterior cladding
- Waterproofing assemblies
- Insulation assemblies
- Finish assemblies
- Structural connections
- Mechanical assemblies
- Electrical assemblies
- Plumbing assemblies

Assemblies should contain component relationships, dimensions, materials, performance properties, and installation dependencies.

## Construction Detail Module

The Construction Detail Module generates detailed construction information.

It supports:

- Connections
- Fasteners
- Anchoring
- Flashing
- Waterproofing
- Sealing
- Penetrations
- Structural connections
- Material transitions
- Finish transitions
- Equipment connections
- Service access
- Tolerances

The system should be able to move from building-level design into detailed assemblies while preserving relationships to the larger building model.

## Design Validation Module

The Design Validation Module continuously evaluates the architectural model.

It should detect:

- Geometric conflicts
- Spatial conflicts
- Missing components
- Inconsistent dimensions
- Unconnected systems
- Impossible circulation
- Insufficient clearances
- System clashes
- Regulatory conflicts
- Incomplete assemblies
- Documentation inconsistencies
- Unresolved assumptions

Validation results should include:

- Issue
- Severity
- Location
- Affected objects
- Cause
- Applicable rule
- Suggested solutions
- Resolution status
- Reviewer
- Date

## Change Propagation Module

The Change Propagation Module tracks the consequences of design changes.

If a user modifies an element, the system should identify affected:

- Spaces
- Geometry
- Structure
- MEP
- Materials
- Assemblies
- Drawings
- Schedules
- Quantities
- Renderings
- Regulatory analyses
- Cost estimates
- Construction sequences

The system should present affected elements before automatically applying major cascading changes.

## Design Alternative Module

The Design Alternative Module generates controlled alternatives while preserving defined constraints.

Users should be able to request alternatives based on:

- Cost
- Size
- Style
- Materials
- Sustainability
- Construction complexity
- Performance
- Accessibility
- Regulatory limitations
- Site constraints
- Structural efficiency
- Spatial efficiency

Alternatives should be comparable using consistent project criteria.

## Materials & Components Module

The Materials & Components Module provides structured information about building materials and components.

It supports:

- Material properties
- Dimensions
- Appearance
- Finishes
- Performance
- Assembly relationships
- Compatibility
- Maintenance
- Manufacturer-neutral specifications
- Substitution options

The system should not require a specific manufacturer unless the user explicitly chooses one.

## Quantity & Cost Module

The Quantity & Cost Module derives quantities from the building model.

It supports:

- Area calculations
- Volume calculations
- Component counts
- Material quantities
- Assembly quantities
- Equipment quantities
- Labor assumptions
- Cost estimates
- Alternative cost scenarios
- Change-order impact analysis

Cost information should be geographically configurable and clearly identified as estimates unless verified by authoritative pricing data.

## Construction Sequencing Module

The Construction Sequencing Module represents the logical construction process.

It should support:

- Site preparation
- Excavation
- Foundations
- Structural construction
- Building envelope
- MEP rough-in
- Interior construction
- Finishes
- Equipment installation
- Commissioning
- Site completion

The system should identify dependencies and construction conflicts.

## Project Provenance Module

The Project Provenance Module records the history of significant project decisions.

It should track:

- User requests
- AI proposals
- Accepted decisions
- Rejected decisions
- Manual modifications
- Regulatory changes
- Model changes
- Reviews
- Approvals
- Validation results
- Exports
- Imports
- External data sources

Every significant automated change should be attributable to its originating instruction, rule, or process.

## Professional Review & Approval Module

The Professional Review & Approval Module establishes human review gates.

The system should distinguish between:

- AI generated
- User approved
- Architect reviewed
- Engineer reviewed
- Code reviewed
- Jurisdiction reviewed
- Permit submitted
- Permit approved
- Construction approved

The system must never represent AI-generated output as professionally stamped, approved, permitted, or construction-ready unless the applicable human professionals and authorities have completed those processes.

## Interoperability Module

The Interoperability Module provides interfaces to external architectural, engineering, construction, and visualization systems.

The module should prioritize:

- Open standards
- Vendor-neutral formats
- Documented APIs
- Structured data
- IFC and openBIM workflows
- Import and export
- Model synchronization

Vendor-specific integrations should be implemented as plugins rather than requirements of the core specification.

## Versioning & Collaboration Module

The Versioning & Collaboration Module manages project evolution.

It supports:

- Project versions
- Design branches
- Alternatives
- Revisions
- Change comparisons
- User comments
- Review workflows
- Approvals
- Rollbacks
- Decision history

Multiple participants should be able to work on a project without losing the history of architectural decisions.

## AI Agent Architecture

Archima should support specialized AI agents operating against a shared project model.

Possible agents include:

- Architectural Vision Agent
- Architectural Design Agent
- Spatial Planning Agent
- Style Agent
- Geometry Agent
- Structural Agent
- Mechanical Agent
- Electrical Agent
- Plumbing Agent
- Fire Safety Agent
- Site Agent
- Zoning Agent
- Code Compliance Agent
- Materials Agent
- Construction Agent
- Cost Agent
- Documentation Agent
- Visualization Agent
- Validation Agent
- Project Coordination Agent

Agents must operate through defined interfaces and must not independently overwrite authoritative project information without appropriate authorization.

## Agent Coordination

Agents should communicate through structured project objects, tasks, findings, proposals, and validation results.

Each agent response should identify:

- Agent identity
- Task
- Inputs
- Assumptions
- Proposed changes
- Affected objects
- Validation status
- Confidence
- Required human review

The Project Coordination Agent should resolve workflow dependencies and identify conflicts between specialist recommendations.

## Optional Plugin Modules

Archima should provide a plugin architecture that allows additional capabilities to be installed independently.

### Advanced Architectural Style Plugins

Optional plugins may provide specialized style libraries including:

- Regional architecture
- Historic architecture
- Vernacular architecture
- Religious architecture
- Indigenous architectural traditions
- Contemporary architecture
- Experimental architecture
- Futuristic architecture

### Regional Zoning Plugins

Regional plugins may provide jurisdiction-specific regulatory datasets and update mechanisms.

Examples include:

- Country-specific zoning
- State or provincial zoning
- County zoning
- Municipal zoning
- Special districts
- Historic districts
- Coastal zones
- Flood zones

### Building Code Plugins

Plugins may provide jurisdiction-specific building code datasets and validation engines.

### Structural Engineering Plugins

Plugins may provide specialized structural analysis and engineering workflows.

### MEP Engineering Plugins

Plugins may provide advanced mechanical, electrical, plumbing, and fire protection calculations and analysis.

### Energy Analysis Plugins

Plugins may provide:

- Energy modeling
- Solar analysis
- Thermal modeling
- Daylight analysis
- HVAC optimization
- Building performance simulation

### Environmental Analysis Plugins

Plugins may provide:

- Carbon analysis
- Water analysis
- Stormwater analysis
- Site ecology
- Environmental impact analysis
- Passive design analysis

### Landscape Architecture Plugins

Plugins may provide:

- Plant libraries
- Landscape systems
- Irrigation
- Hardscape
- Site ecology
- Garden design
- Outdoor living systems

### Interior Design Plugins

Plugins may provide:

- Furniture
- Fixtures
- Finishes
- Lighting
- Interior styles
- Space planning
- Interior rendering

### Specialized Building Plugins

Plugins may support specialized structures including:

- Underground structures
- Bunkers
- Safe rooms
- Off-grid buildings
- Tiny houses
- Modular buildings
- Floating structures
- Disaster-resistant buildings
- Agricultural structures
- Industrial structures
- Hospitality structures
- Healthcare structures
- Educational structures

### Manufacturing & Fabrication Plugins

Plugins may provide connections to:

- CNC systems
- 3D printing
- Robotic fabrication
- Prefabrication
- Modular construction
- Digital fabrication
- Automated material processing

### Visualization Plugins

Plugins may provide:

- Advanced rendering
- Virtual reality
- Augmented reality
- Interactive walkthroughs
- Real-time visualization
- Immersive design review

### Cost Database Plugins

Plugins may provide geographically specific:

- Material costs
- Labor costs
- Equipment costs
- Construction costs
- Market data

### Manufacturer Catalog Plugins

Plugins may provide manufacturer-specific components and product data while preserving manufacturer-neutral representations in the core model.

## Plugin Requirements

Plugins should:

- Use documented interfaces.
- Declare their capabilities.
- Declare required dependencies.
- Identify their data sources.
- Identify their geographic scope where applicable.
- Provide version information.
- Preserve project provenance.
- Avoid modifying unrelated project objects.
- Respect user permissions.
- Provide validation information.
- Clearly identify external dependencies.
- Remain optional unless explicitly required by a project.

## Regulatory Data Requirements

Regulatory datasets should identify:

- Jurisdiction
- Authority
- Regulation
- Rule
- Source
- Effective date
- Expiration date where applicable
- Version
- Geographic applicability
- Applicability conditions
- Data retrieval date
- Verification status

The system should distinguish between authoritative regulatory information and AI interpretation.

## Security & Privacy

Archima should support:

- Local-first deployment
- Private project storage
- Access control
- Role-based permissions
- Encryption where appropriate
- Audit logging
- Project isolation
- Secure plugin execution
- Controlled external data access
- User-controlled model providers

The core specification should not require a particular AI provider.

## Local-First Architecture

Archima should support operation using locally hosted AI models, local building models, local project databases, and local rendering systems where practical.

Cloud services may be used through optional integrations.

No cloud provider should be required by the core specification.

## Vendor Independence

Archima must not require users to adopt a particular:

- LLM provider
- BIM application
- CAD application
- Rendering engine
- Structural software
- MEP software
- Cloud platform
- Manufacturer
- Construction platform

Integrations should be implemented through documented interfaces and optional plugins.

## Design Safety & Verification

Archima must distinguish between:

- Conceptual design
- Preliminary design
- Coordinated design
- Code analysis
- Engineering analysis
- Construction documentation
- Professional approval
- Permit approval
- Construction authorization

AI-generated designs must not be represented as legally approved or professionally certified without the applicable review.

The system should prominently identify assumptions, unresolved conflicts, missing information, and required professional review.

## Output Requirements

Archima should be capable of producing:

- Architectural concepts
- Floor plans
- Site plans
- Roof plans
- Foundation plans
- Elevations
- Sections
- Details
- Schedules
- Schematics
- 3D models
- Architectural renderings
- Material studies
- Building system diagrams
- Structural concepts
- MEP concepts
- Construction assemblies
- Quantity takeoffs
- Cost estimates
- Construction sequences
- Design reports
- Regulatory reports
- Validation reports
- Project histories
- Interoperable building models

## Design Transformation Workflow

Archima should support the following conceptual workflow:

**Vision**

The user describes what they want to build.

**Requirements**

Archima converts the vision into explicit project requirements.

**Program**

The system establishes spaces, functions, adjacencies, circulation, and constraints.

**Concept**

Archima generates architectural concepts and alternatives.

**Model**

The selected concept becomes a structured parametric building model.

**Coordination**

Architecture, structure, site, MEP, materials, and assemblies are coordinated.

**Regulation**

The design is evaluated against the selected geographic and regulatory profile.

**Adaptation**

The building model is modified when required to satisfy applicable constraints.

**Validation**

The system identifies conflicts, missing information, and unresolved requirements.

**Documentation**

Coordinated drawings, schedules, schematics, and details are generated from the model.

**Review**

Architects, engineers, specialists, authorities, and other qualified reviewers perform the required professional review.

**Construction**

Approved documentation may be used as part of the applicable construction workflow.

## Multi-Jurisdiction Design

Archima should allow a single architectural concept to be evaluated against multiple jurisdictions.

For example, a user should be able to request:

> Adapt this architectural concept for multiple cities while preserving the architectural style, room program, courtyard, rooftop patio, and overall design intent.

The system should generate jurisdiction-specific design configurations while preserving a relationship to the original concept.

Each configuration should identify:

- Geographic jurisdiction
- Applicable regulatory profile
- Modified elements
- Preserved elements
- Regulatory conflicts
- Design compromises
- New opportunities
- Validation status

## Design Optimization

Archima should support constrained design optimization.

Users should be able to establish priorities such as:

- Maximize living space
- Minimize construction cost
- Preserve courtyard size
- Maximize natural light
- Preserve architectural style
- Minimize energy consumption
- Maximize accessibility
- Preserve views
- Minimize site disturbance
- Maximize usable outdoor space

The AI should optimize the design while maintaining explicitly protected requirements.

## Natural Language Design Interaction

Users should be able to interact with Archima conversationally.

Examples include:

> Make the kitchen 20 percent larger.

> Move the primary bedroom to the quieter side of the house.

> Keep the courtyard but reduce the building footprint.

> Add a rooftop patio.

> Make the house Mediterranean but use modern structural systems.

> Adapt this design to a different zoning district.

> Give me three alternatives that reduce construction cost.

> Show me what changed after the zoning adaptation.

> Generate the complete drawing set for the current approved model.

The system should translate these instructions into structured model changes rather than treating each request as an isolated image-generation prompt.

## Change Impact Analysis

Before applying significant changes, Archima should identify expected consequences.

For example:

**Requested Change**

Increase the courtyard by 20 percent.

**Potential Impacts**

- Reduced building footprint
- Modified room dimensions
- Modified structural spans
- Modified roof geometry
- Modified exterior walls
- Modified windows
- Modified HVAC distribution
- Modified electrical layouts
- Modified landscaping
- Modified quantities
- Modified drawings
- Modified cost estimate

The user should be able to approve or reject the proposed cascade.

## Schematic Integrity

All generated schematics should remain synchronized with the current architectural model.

If the model changes, affected schematics should be marked for regeneration or automatically updated according to project settings.

The system should identify outdated drawings rather than allowing obsolete documentation to appear current.

## Documentation Integrity

Generated documentation should identify:

- Project version
- Model version
- Drawing version
- Generation date
- Review status
- Validation status
- Regulatory profile
- Required professional review

## Extensibility

Future versions of Archima should be able to add capabilities without breaking existing project models.

New modules should use versioned interfaces and maintain backward compatibility wherever practical.

## Implementation Requirements

An implementation claiming Archima compatibility should provide:

- Architectural project representation
- Design intent management
- Parametric building model
- Natural language interaction
- 2D documentation
- 3D modeling
- Architectural visualization
- Design validation
- Change propagation
- Project versioning
- Provenance
- Plugin interfaces
- Geographic regulatory adaptation
- Human review controls
- Interoperability interfaces

Optional capabilities may be implemented through plugins.

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
  - [https://roxanneardary.com/archima/](https://roxanneardary.com/archima/)  

---

## License & Notice Requirements

Archima is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Archima specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
