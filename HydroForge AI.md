# HydroForge AI
**The Open Specification for Generative Hydraulic Engineering**
- HTML Mirror:  [https://roxanneardary.com/hydroforge-ai-specification/](https://roxanneardary.com/hydroforge-ai-specification/)  

---

HydroForge AI is the open specification for generative hydraulic engineering. It defines a modular system for formulating, generating, analyzing, simulating, comparing, and refining water infrastructure designs including aqueducts, canals, underground channels, settling systems, reservoirs, pipelines, and complex hydraulic networks.

## Purpose

HydroForge AI is designed to move beyond isolated hydraulic calculations and support the formulation of complete water infrastructure systems. It interprets user-defined objectives and constraints, evaluates terrain and hydraulic conditions, generates multiple design alternatives, models their behavior, identifies tradeoffs, and helps users refine designs according to priorities such as efficiency, economy, functionality, aesthetics, historical character, environmental impact, resilience, maintenance, and energy use.

The specification is intended to support conceptual and analytical engineering workflows while maintaining a clear distinction between AI-generated designs and independently verified, code-compliant, permitted, construction-ready, and professionally approved engineering.

## Core Principles

- Modular design
- Open specification
- Local-first operation
- Vendor independence
- Solver independence
- AI-model independence
- Human-controlled design
- Human-in-the-loop engineering
- Explainable engineering decisions
- Reproducible calculations
- Explicit assumptions
- Transparent optimization
- Multiple design alternatives
- Gravity-first analysis
- Safety-conscious design
- Interoperable representations
- Long-term maintainability
- Future-proof architecture
- Clear separation between conceptual and verified engineering

---

## Core Modules

### Requirements & Constraint Module

The Requirements & Constraint Module translates natural-language requests into structured hydraulic engineering requirements.

Features include:

- Natural-language design requirements
- Required, preferred, and optional requirement classification
- Functional and performance requirements
- Flow requirements
- Capacity requirements
- Pressure requirements
- Velocity requirements
- Elevation requirements
- Storage requirements
- Geographic constraints
- Terrain constraints
- Construction constraints
- Material constraints
- Budget constraints
- Energy constraints
- Maintenance constraints
- Environmental constraints
- Historical constraints
- Aesthetic constraints
- Regulatory considerations
- Land-use constraints
- Access requirements
- User-defined optimization priorities
- Constraint conflict detection
- Missing-information detection
- Constraint relaxation analysis

### Water Source Module

The Water Source Module evaluates potential water sources and their relationship to the proposed hydraulic system.

Features include:

- Surface water sources
- Groundwater sources
- Springs
- Rainwater
- Reservoir sources
- Seawater
- Brackish water
- Recycled water
- Multiple-source systems
- Source reliability analysis
- Seasonal availability
- Source elevation analysis
- Intake considerations
- Source quality requirements
- Source-to-system compatibility
- Source redundancy

### Water Treatment & Desalination Module

The Water Treatment & Desalination Module determines how water quality requirements affect hydraulic system architecture.

Features include:

- Treatment requirement assessment
- Water-quality requirements
- Treatment capacity analysis
- Desalination requirement assessment
- Seawater desalination
- Brackish-water desalination
- Pretreatment
- Post-treatment
- Treatment placement optimization
- Treatment and storage integration
- Treatment and distribution integration
- Desalination energy analysis
- Concentrate and brine management considerations
- Treatment architecture comparison
- Modular treatment systems
- Treatment redundancy

### Terrain & Geographic Analysis Module

The Terrain & Geographic Analysis Module evaluates physical geography and identifies potential hydraulic corridors.

Features include:

- Terrain analysis
- Elevation profiles
- Longitudinal route profiles
- Slope analysis
- Watershed awareness
- Ridge and valley identification
- Natural drainage analysis
- Surface route generation
- Underground route generation
- Crossing identification
- Excavation depth analysis
- High-point identification
- Low-point identification
- Gravity corridor identification
- Route alternatives
- Terrain-based route optimization

### Gravity Optimization Module

The Gravity Optimization Module prioritizes gravity-assisted conveyance wherever hydraulic and geographic conditions make it practical.

Features include:

- Gravity feasibility analysis
- Available-head analysis
- Hydraulic grade line analysis
- Gravity route generation
- Gravity-only system generation
- Gravity-plus-pump system generation
- Staged gravity systems
- Cascading reservoirs
- Elevated storage
- Gravity-fed distribution
- Elevation-based pressure management
- Gravity-driven settling
- Gravity-driven treatment concepts
- Pump elimination analysis
- Pump reduction analysis
- Energy minimization
- Gravity versus pumping comparison

### Open-Channel Module

The Open-Channel Module generates and evaluates channels and other free-surface hydraulic systems.

Features include:

- Canals
- Aqueduct channels
- Flumes
- Drainage channels
- Lined channels
- Unlined channels
- Rectangular channels
- Trapezoidal channels
- Circular channels
- Custom channel geometries
- Hydraulic radius calculations
- Wetted perimeter calculations
- Freeboard analysis
- Velocity analysis
- Slope optimization
- Capacity analysis
- Transitions
- Drop structures
- Weirs
- Spillways
- Cascades
- Flow-control structures
- Erosion-risk analysis

### Aqueduct Module

The Aqueduct Module generates long-distance water conveyance systems with particular attention to elevation, architecture, and gravity flow.

Features include:

- Long-distance aqueduct routing
- Gravity aqueducts
- Elevated aqueducts
- Surface aqueducts
- Underground aqueducts
- Hybrid aqueducts
- Arch-supported concepts
- Masonry-inspired designs
- Modern structural integration
- Hydraulic slope optimization
- Channel sizing
- Freeboard analysis
- Valley crossings
- Tunnel transitions
- Pipeline transitions
- Historical-inspired aqueducts
- Modernized historical designs
- Maintenance access
- Inspection access
- Overflow routing
- Emergency routing

### Underground Conveyance Module

The Underground Conveyance Module generates and analyzes concealed hydraulic infrastructure.

Features include:

- Buried pipelines
- Underground channels
- Tunnel concepts
- Hydraulic galleries
- Utility corridors
- Vertical shafts
- Access chambers
- Inspection chambers
- Maintenance access
- Burial-depth analysis
- Excavation-volume analysis
- Terrain-following routes
- High-point analysis
- Low-point analysis
- Air-management considerations
- Drainage considerations
- Groundwater considerations
- Underground storage
- Underground settling systems
- Surface-to-underground transitions

### Pipe Engineering Module

The Pipe Engineering Module evaluates individual hydraulic conveyance segments and their physical properties.

Features include:

- Pipe material selection
- Pipe diameter selection
- Pipe length
- Pipe roughness
- Pressure analysis
- Velocity analysis
- Flow analysis
- Headloss analysis
- Minor-loss analysis
- Elevation effects
- Gravity-flow analysis
- Pressurized-flow analysis
- Partially full pipe analysis
- Series configurations
- Parallel configurations
- Tapered systems
- Variable-diameter systems
- Pipe transitions
- Material lifecycle comparisons

### Pipe Network Synthesis Module

The Pipe Network Synthesis Module generates complete interconnected pipe systems.

Features include:

- Network topology generation
- Branching networks
- Looped networks
- Ring networks
- Radial networks
- Manifold networks
- Header systems
- Multi-zone systems
- Parallel conveyance
- Redundant conveyance
- Isolation zones
- Distribution zones
- Pressure zones
- Flow zones
- Junction generation
- Valve placement
- Bypass routing
- Emergency routing
- Network balancing
- Failure-path analysis
- Topology optimization

### Long-Distance Conveyance Module

The Long-Distance Conveyance Module analyzes systems extending across substantial distances or complex terrain.

Features include:

- Long-distance route generation
- Multi-segment conveyance
- Cumulative headloss analysis
- Friction-loss analysis
- Intermediate storage
- Pressure management
- Pressure-zone segmentation
- Staged pumping
- Staged gravity conveyance
- Hybrid conveyance
- Elevation-break analysis
- Velocity management
- Energy optimization
- Route comparison
- Pipe and channel sizing optimization
- Pump placement
- Reservoir placement
- Surge considerations

### Hydraulic Calculation Module

The Hydraulic Calculation Module provides the mathematical foundation for hydraulic analysis and design evaluation.

Features include:

- Continuity analysis
- Energy analysis
- Bernoulli analysis
- Static head
- Dynamic head
- Hydraulic head
- Friction losses
- Minor losses
- Darcy-Weisbach calculations
- Hazen-Williams calculations
- Manning calculations
- Chezy calculations
- Open-conduit analysis
- Closed-conduit analysis
- Hydraulic radius
- Reynolds number
- Flow-regime analysis
- Pressure calculations
- Velocity calculations
- Flow-rate calculations
- Pump-head calculations
- System curves
- Equation-selection logic
- Unit conversion
- Dimensional consistency checks
- Calculation traceability
- Independent verification

### Settling & Sedimentation Module

The Settling & Sedimentation Module generates systems for removing suspended material before or during conveyance and storage.

Features include:

- Settling tanks
- Sedimentation basins
- Forebays
- Grit chambers
- Sediment traps
- Settling ponds
- Flow-distribution analysis
- Residence-time analysis
- Sediment accumulation analysis
- Cleaning access
- Sludge-management considerations
- Flushing systems
- Gravity sedimentation
- Multi-stage settling
- Settling-system optimization
- Hydraulic short-circuit detection

### Storage Module

The Storage Module designs hydraulic storage and balancing systems.

Features include:

- Reservoirs
- Cisterns
- Tanks
- Elevated storage
- Underground storage
- Balancing storage
- Intermediate storage
- Surge storage
- Seasonal storage
- Storage-volume optimization
- Inflow analysis
- Outflow analysis
- Overflow routing
- Emergency storage
- Storage and distribution integration
- Gravity-head optimization

### Hydraulic Control Module

The Hydraulic Control Module designs structures and operating strategies for controlling water movement.

Features include:

- Valves
- Gates
- Check valves
- Pressure-reducing systems
- Flow-control systems
- Orifices
- Weirs
- Bypasses
- Overflows
- Isolation systems
- Pressure zones
- Automated control concepts
- Manual control concepts
- Fail-safe concepts
- Emergency shutoff concepts

### Pumping Module

The Pumping Module evaluates when pumping is necessary and how it can be integrated efficiently.

Features include:

- Pump necessity assessment
- Pump selection logic
- Pump head analysis
- Pump flow analysis
- Operating-point analysis
- Pump-system interaction
- Pump energy analysis
- Variable-speed operation
- Pump redundancy
- Pump-station placement
- Pump staging
- Pump scheduling
- Gravity versus pumping analysis
- Lifecycle energy analysis
- Power-loss scenarios
- Emergency operation

### Hydraulic Transient & Stability Module

The Hydraulic Transient & Stability Module evaluates dynamic hydraulic conditions that may affect system stability and integrity.

Features include:

- Hydraulic transient analysis
- Pressure surge analysis
- Water hammer analysis
- Valve-operation effects
- Pump start effects
- Pump stop effects
- Flow reversal analysis
- Air accumulation analysis
- High-point analysis
- Low-point analysis
- Surge-control concepts
- Hydraulic stability analysis
- Emergency shutdown analysis

### Artistic & Architectural Layout Module

The Artistic & Architectural Layout Module allows aesthetic objectives to influence hydraulic architecture without replacing engineering requirements.

Features include:

- Artistic hydraulic systems
- Landscape integration
- Monumental designs
- Classical designs
- Roman-inspired designs
- Medieval-inspired designs
- Industrial designs
- Naturalistic designs
- Minimalist designs
- Futuristic designs
- Sculptural designs
- Decorative aqueducts
- Architectural channels
- Visible pipework
- Cascades
- Fountains
- Bridges
- Arches
- Terraces
- Garden water systems
- Concealed infrastructure
- Architectural integration
- Visual-axis planning
- Proportion-based layouts
- User-defined aesthetic priorities

### Historical Design Module

The Historical Design Module incorporates historical engineering concepts and visual characteristics into design alternatives.

Features include:

- Historical engineering references
- Historical aqueduct concepts
- Historical canal concepts
- Historical cistern concepts
- Roman-inspired systems
- Medieval-inspired systems
- Ancient engineering concepts
- Industrial-era concepts
- Historical materials
- Historical geometries
- Historical construction concepts
- Historical versus modern comparisons
- Modern safety integration
- Historical appearance with modern infrastructure
- Historical authenticity assessment

### Economic Optimization Module

The Economic Optimization Module evaluates financial implications throughout the design lifecycle.

Features include:

- Construction-cost analysis
- Material-cost analysis
- Excavation-cost analysis
- Pumping-cost analysis
- Energy-cost analysis
- Maintenance-cost analysis
- Replacement-cost analysis
- Lifecycle-cost analysis
- Capital-cost analysis
- Operating-cost analysis
- Total-cost analysis
- Budget-constrained generation
- Cost-performance comparison
- Longevity comparison

### Environmental Module

The Environmental Module incorporates environmental considerations into hydraulic design.

Features include:

- Environmental constraint analysis
- Surface-disturbance analysis
- Excavation-impact analysis
- Erosion analysis
- Sediment-impact analysis
- Groundwater considerations
- Wetland considerations
- Habitat considerations
- Water-loss analysis
- Evaporation analysis
- Energy-impact analysis
- Ecological-flow considerations
- Intake-impact considerations
- Discharge-impact considerations
- Brine-impact considerations
- Environmental alternative generation

### Materials & Construction Module

The Materials & Construction Module evaluates physical materials and construction approaches.

Features include:

- Material selection
- Material comparison
- Pipe materials
- Channel materials
- Channel lining
- Masonry concepts
- Concrete concepts
- Steel concepts
- Polymer concepts
- Composite concepts
- Local-material considerations
- Constructability analysis
- Installation methods
- Excavation methods
- Prefabrication concepts
- Maintenance access
- Construction alternatives

### Resilience & Redundancy Module

The Resilience & Redundancy Module evaluates how systems behave when components or operating conditions fail.

Features include:

- Failure-mode analysis
- Single-point-of-failure detection
- Pipe failure scenarios
- Valve failure scenarios
- Pump failure scenarios
- Storage failure scenarios
- Power-loss scenarios
- Blockage scenarios
- Sediment scenarios
- Extreme-flow scenarios
- Low-flow scenarios
- Drought scenarios
- Emergency routing
- Redundant conveyance
- Isolation strategies
- Degraded operating modes
- Emergency operating modes
- Recovery modes

### Multi-Objective Optimization Module

The Multi-Objective Optimization Module balances competing design objectives.

Features include:

- Efficiency optimization
- Economic optimization
- Gravity optimization
- Energy optimization
- Aesthetic optimization
- Historical optimization
- Functional optimization
- Environmental optimization
- Resilience optimization
- Maintenance optimization
- Constructability optimization
- User-defined objective weights
- Weighted optimization
- Constraint prioritization
- Pareto-style alternative generation
- Tradeoff analysis
- Objective-conflict detection

### Design Alternative Module

The Design Alternative Module generates distinct architectures for comparison rather than forcing a single solution.

Features include:

- Automatic alternative generation
- Conservative alternatives
- Economic alternatives
- High-efficiency alternatives
- Gravity-first alternatives
- Low-maintenance alternatives
- High-resilience alternatives
- Historical alternatives
- Artistic alternatives
- Minimal-footprint alternatives
- Underground alternatives
- Above-ground alternatives
- Hybrid alternatives
- User-defined design archetypes
- Alternative comparison
- Alternative scoring
- Alternative ranking
- Alternative refinement

### Simulation & Verification Module

The Simulation & Verification Module evaluates generated designs against hydraulic behavior and defined constraints.

Features include:

- Hydraulic model generation
- Hydraulic solver integration
- Steady-state analysis
- Dynamic analysis
- Scenario analysis
- Sensitivity analysis
- Failure simulation
- Demand variation
- Seasonal variation
- Flow variation
- Pressure variation
- Storage variation
- Pumping scenarios
- Gravity scenarios
- Constraint verification
- Calculation verification
- Model-consistency checks
- Simulation interpretation

### GIS & Spatial Integration Module

The GIS & Spatial Integration Module represents hydraulic designs in geographic context.

Features include:

- GIS-compatible design representation
- Coordinate-aware routing
- Terrain data integration
- Elevation data integration
- Property-boundary considerations
- Land-use analysis
- Infrastructure-crossing analysis
- Route corridors
- Spatial constraint mapping
- Surface and subsurface comparison

### Visualization Module

The Visualization Module represents hydraulic designs in forms suitable for analysis, comparison, and communication.

Features include:

- Network diagrams
- Elevation profiles
- Longitudinal profiles
- Hydraulic-grade-line visualization
- Flow visualization
- Pressure visualization
- Cross-sections
- Channel visualization
- Pipe-network visualization
- Underground-system visualization
- Aqueduct visualization
- Reservoir visualization
- Alternative-design visualization
- Artistic concept visualization
- Construction concept visualization

### AI Reasoning Module

The AI Reasoning Module coordinates interpretation, design generation, engineering reasoning, and iterative refinement.

Features include:

- Requirements interpretation
- Engineering reasoning
- Design-space exploration
- Constraint reasoning
- Equation selection
- Alternative generation
- Tradeoff reasoning
- Design critique
- Failure reasoning
- Optimization reasoning
- Iterative refinement
- Human-in-the-loop interaction
- Explainable reasoning
- Assumption reporting
- Confidence reporting
- Uncertainty reporting
- Professional-verification flags

### Provenance & Audit Module

The Provenance & Audit Module maintains traceability throughout the design process.

Features include:

- Input provenance
- Data provenance
- Equation provenance
- Parameter provenance
- Calculation provenance
- Design-decision provenance
- Version history
- AI-generated-content identification
- User-modification tracking
- Simulation provenance
- External-model provenance
- Source-data tracking
- Assumption registry
- Engineering-review registry
- Reproducibility records

### Safety & Engineering Review Module

The Safety & Engineering Review Module establishes boundaries between generated concepts and verified engineering.

Features include:

- Safety-critical parameter identification
- Engineering-review flags
- Unverified-design warnings
- Regulatory-risk flags
- Structural-risk flags
- Hydraulic-risk flags
- Environmental-risk flags
- Construction-risk flags
- Operational-risk flags
- Failure-consequence assessment
- Human-approval checkpoints
- Professional-review checkpoints
- Construction-readiness classification
- Conceptual-model classification
- Verified-model classification
- Review-status tracking

### Interoperability Module

The Interoperability Module allows HydroForge AI designs to interact with independent engineering, geographic, simulation, and design systems.

Features include:

- Vendor-independent design representations
- Hydraulic-solver interoperability
- GIS interoperability
- CAD interoperability
- Simulation interoperability
- Structured data exchange
- Machine-readable representations
- Human-readable representations
- Design import
- Design export
- External solver integration
- AI-model integration
- Local deployment support

### Scenario & What-If Module

The Scenario & What-If Module allows users to test how designs respond to changing conditions.

Features include:

- Increased-flow scenarios
- Reduced-flow scenarios
- Increased-demand scenarios
- Reduced-demand scenarios
- Elevation changes
- Route changes
- Material changes
- Diameter changes
- Budget changes
- Energy-price changes
- Pump failures
- Power failures
- Storage failures
- Seasonal scenarios
- Climate-condition scenarios
- Treatment-capacity changes
- Desalination-capacity changes
- Future expansion scenarios

### Expansion & Future-Proofing Module

The Expansion & Future-Proofing Module ensures that designs can accommodate changing requirements.

Features include:

- Capacity expansion
- Modular expansion
- Future branches
- Future reservoirs
- Future treatment systems
- Future desalination systems
- Future pumping systems
- Reserved network capacity
- Reserved hydraulic corridors
- Upgrade planning
- Replacement planning
- Technology-independent compatibility

### Documentation Module

The Documentation Module generates human-readable and machine-readable records of the design process.

Features include:

- Design reports
- Hydraulic calculation reports
- Design rationale
- Assumption reports
- Constraint reports
- Alternative reports
- Optimization reports
- Cost reports
- Energy reports
- Risk reports
- Simulation reports
- Provenance reports
- Engineering-review reports
- Machine-readable specifications
- Human-readable specifications

---

## Optional Plugin Modules

HydroForge AI supports optional plugin modules that extend the core specification without requiring every deployment to implement every capability.

### Advanced Surveying Plugin

Provides enhanced terrain, elevation, survey, route, and field-measurement analysis.

### Structural Engineering Plugin

Provides structural evaluation of aqueduct supports, bridges, tunnels, channels, tanks, reservoirs, and related infrastructure.

### Sediment Transport Plugin

Extends sediment analysis beyond settling systems to include transport, deposition, scour, and sediment-management scenarios.

### Water Quality Plugin

Provides expanded analysis of water-quality parameters and their interaction with conveyance, storage, treatment, and distribution.

### Climate Resilience Plugin

Provides expanded analysis of drought, flooding, extreme precipitation, temperature, evaporation, changing demand, and long-term environmental scenarios.

### Construction Planning Plugin

Generates construction sequencing concepts, access requirements, excavation phases, installation stages, material logistics, and construction alternatives.

### Cost Modeling Plugin

Provides detailed regional, lifecycle, material, labor, energy, excavation, and maintenance cost modeling.

### Advanced Optimization Plugin

Provides additional optimization strategies for complex multi-objective hydraulic systems.

### Advanced Simulation Plugin

Provides expanded dynamic, transient, sensitivity, uncertainty, and failure simulations.

### Monitoring & Operations Plugin

Provides operational monitoring concepts, sensor integration, condition assessment, anomaly detection, maintenance triggers, and system-status analysis.

### Historical Engineering Plugin

Provides expanded historical research and reconstruction capabilities for historically inspired hydraulic systems.

### Landscape & Architecture Plugin

Provides advanced integration of hydraulic infrastructure with landscape architecture, public spaces, gardens, monuments, and architectural environments.

### Desalination Plugin

Provides expanded seawater and brackish-water desalination system generation, energy analysis, treatment integration, concentrate management, and lifecycle comparison.

### Water Reuse Plugin

Provides expanded analysis and design of reclaimed-water systems, treatment integration, storage, conveyance, and reuse networks.

---

## Design Generation Workflow

HydroForge AI follows a structured generative workflow:

- Interpret the user's objectives
- Identify requirements and constraints
- Classify requirements by priority
- Identify missing information
- Analyze available water sources
- Analyze terrain and elevation
- Determine gravity opportunities
- Establish hydraulic requirements
- Formulate candidate system architectures
- Generate multiple design alternatives
- Calculate hydraulic behavior
- Simulate candidate systems
- Evaluate constraints
- Analyze cost, energy, environment, resilience, aesthetics, and maintenance
- Identify tradeoffs
- Rank or compare alternatives
- Present assumptions and uncertainties
- Allow human selection and refinement
- Recalculate modified designs
- Record design provenance
- Identify required professional review

## Design Objectives

HydroForge AI must allow users to define one or more objectives and assign relative importance to them.

Supported objectives include:

- Hydraulic efficiency
- Gravity utilization
- Energy reduction
- Economic efficiency
- Functional performance
- Reliability
- Resilience
- Low maintenance
- Constructability
- Environmental compatibility
- Historical character
- Artistic character
- Landscape integration
- Minimal surface disturbance
- Minimal excavation
- Future expansion
- Operational simplicity

The system should identify conflicts between objectives rather than concealing them. When objectives cannot be simultaneously maximized, HydroForge AI should expose the tradeoff and provide alternative designs representing different priorities.

## Gravity-First Design Requirement

HydroForge AI should evaluate gravity-assisted conveyance before recommending pumping where terrain, available head, flow requirements, and hydraulic losses permit a viable gravity-based configuration.

Gravity-first analysis may include:

- Natural elevation differences
- Gravity corridors
- Cascading systems
- Elevated storage
- Staged conveyance
- Gravity-fed treatment
- Gravity-fed settling
- Gravity-fed distribution
- Pressure management through elevation
- Pump elimination
- Pump reduction

Gravity should remain an optimization preference rather than an absolute requirement. Where gravity alone cannot satisfy the defined requirements, the system should evaluate pumped and hybrid alternatives.

## Generative Design Requirement

HydroForge AI should not prematurely converge on a single hydraulic architecture.

For suitable design problems, the system should generate multiple technically reasoned alternatives representing different combinations of:

- Conveyance type
- Route
- Elevation strategy
- Pipe or channel dimensions
- Materials
- Storage configuration
- Treatment configuration
- Pumping strategy
- Gravity utilization
- Network topology
- Construction approach
- Cost
- Energy use
- Maintenance requirements
- Environmental impact
- Aesthetic character
- Historical character
- Resilience

Each alternative should include its assumptions, relevant calculations, constraints, advantages, disadvantages, uncertainties, and major tradeoffs.

## Human Control

HydroForge AI is intended to assist human decision-making rather than replace professional engineering judgment.

Users should be able to:

- Modify requirements
- Modify constraints
- Change priorities
- Reject alternatives
- Select alternatives
- Combine design concepts
- Override non-safety-critical recommendations
- Request new alternatives
- Request design critique
- Request what-if scenarios
- Review calculations
- Review assumptions
- Review provenance
- Iterate designs

Safety-critical or professionally regulated decisions should remain subject to appropriate human and professional review.

## Engineering Status

HydroForge AI generated designs must clearly identify their engineering status.

Possible classifications include:

- Conceptual
- Preliminary
- Simulated
- Computationally verified
- Professionally reviewed
- Code-compliant
- Permitted
- Construction-ready

The system must not represent an AI-generated design as professionally stamped, legally approved, permitted, code-compliant, or construction-ready unless those conditions have been independently established by appropriately qualified professionals and authorities.

## Provenance Requirements

HydroForge AI should preserve sufficient information to reproduce and audit important design decisions.

Provenance should include, where applicable:

- User requirements
- Source data
- Terrain data
- Hydraulic parameters
- Material parameters
- Equations used
- Calculation inputs
- Calculation outputs
- Simulation configurations
- Solver results
- Design alternatives
- Optimization objectives
- User modifications
- AI-generated recommendations
- Human decisions
- Engineering reviews
- Verification status
- Version history

## Interoperability Requirements

HydroForge AI should maintain representations that are independent of any particular vendor, AI model, hydraulic solver, geographic platform, or design environment.

Design information should be capable of being represented in structured forms suitable for:

- Hydraulic analysis
- Geographic analysis
- Engineering review
- Simulation
- Design exchange
- Documentation
- Archival
- Human inspection
- Machine processing

## Open Specification Requirements

HydroForge AI is designed as an extensible open specification. Implementations should be able to adopt core capabilities independently and extend functionality through optional modules and plugins.

Implementations should prioritize:

- Transparency
- Modularity
- Interoperability
- Reproducibility
- Human control
- Explicit assumptions
- Traceable calculations
- Independent verification
- Vendor independence
- Long-term accessibility

## Scope

HydroForge AI applies to conceptual and analytical hydraulic engineering involving water conveyance, storage, treatment, distribution, control, and related infrastructure.

Potential applications include:

- Aqueduct design
- Canal design
- Water-supply planning
- Gravity-fed water systems
- Pipeline systems
- Underground water infrastructure
- Reservoir systems
- Settling systems
- Hydraulic networks
- Treatment integration
- Desalination integration
- Landscape water systems
- Historical hydraulic reconstruction
- Infrastructure planning
- Hydraulic optimization
- Water-system scenario analysis

HydroForge AI does not replace licensed engineering, surveying, geotechnical investigation, structural analysis, environmental review, permitting, construction inspection, or other professional services required for real-world infrastructure.

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
  - [https://roxanneardary.com/hydroforge-ai/](https://roxanneardary.com/hydroforge-ai/)

---

## License & Notice Requirements

HydroForge AI is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- HydroForge AI specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
