# HotSide Collective

**An Open Standard for Useful Energy.**

HotSide Collective is an open-source thermal infrastructure project that defines a reproducible, safe, and modular system for recovering waste heat from liquid-cooled compute environments and redirecting it into usable hydronic energy for buildings, campuses, and district heating networks.

It treats data centers not only as compute infrastructure, but as **distributed thermal assets**.

---

## Overview

Modern compute systems—especially AI and high-density workloads—generate large amounts of waste heat. Today, that heat is typically discarded. HotSide Collective provides an open mechanical, electrical, and software standard to capture and reuse it safely.

The system sits between:
```text
Liquid-Cooled Compute Systems → HotSide Collective → Building / District Heating Systems
```


It does not modify server operation. It interfaces only through thermal exchange layers.

---

## Core Features

### 🔥 Modular Heat Recovery Skid Architecture
- Standardized, scalable heat-exchange skid design
- Cartridge-based plate heat exchanger modules
- Deployable from small lab systems (~10–25 kW) to multi-MW installations
- Plug-and-play integration with liquid-cooled racks and CDUs
- Physical isolation between IT cooling and building hydronic loops

---

### 🔁 Dual-Loop Thermal Isolation System
- Fully separated primary (compute) and secondary (building) fluid loops
- No fluid mixing under any condition
- Optional double-wall or vented exchanger configurations
- Leak containment and isolation design patterns
- Safe decoupling from IT cooling infrastructure

---

### 🌡️ Intelligent Thermal Transfer Control
- Adaptive flow balancing based on real-time ΔT optimization
- Dynamic pump modulation for variable thermal loads
- Buffer-aware heat distribution logic
- Load prioritization: compute stability over heat export
- Autonomous fallback behavior during demand imbalance

---

### 🧠 Open Control System Stack
- Edge-first control architecture (no cloud dependency required)
- Deterministic control firmware (Rust / C reference implementations)
- Supervisory layer (Python / Go reference implementations)
- Local-first operation with optional remote telemetry
- Modular control logic for pumps, valves, and exchangers

---

### 📡 Industrial Sensor Integration Layer
- Temperature sensors (primary/secondary loop monitoring)
- Flow meters for real-time heat transfer measurement
- Differential pressure monitoring across heat exchangers
- Leak detection inputs with hardware-level safety triggers
- Standard industrial interfaces (4–20 mA, RTD, Modbus)

---

### 🏠 Hydronic Output Standardization
- Radiant floor heating compatibility
- Domestic hot water preheating support
- Greenhouse and agricultural heating integration
- District heating network compatibility
- Configurable output temperature ranges (low to high-grade heat)

---

### 🧯 Thermal Buffering & Load Management
- Integrated buffer tank control system
- Thermal storage smoothing for demand fluctuations
- Overflow routing to auxiliary cooling or rejection systems
- Demand balancing between compute and building systems
- Stable output delivery under variable compute loads

---

### 🛡️ Safety-First Mechanical Design Framework
- Hard mechanical fail-safes independent of software
- ASME-aligned pressure and piping design standards
- Expansion tanks and pressure relief systems
- Emergency bypass routing for full system isolation
- Defined safe operating envelopes for all system states

---

### 📐 Open Mechanical Reference Designs
- Published P&ID diagrams and system schematics
- Standardized skid layout templates
- BOMs using commercially available components
- Fabrication guides for modular heat exchanger assemblies
- Retrofit pathways for existing data centers

---

### ⚡ Electrical & Control Panel Standards
- UL 508A-aligned control panel architecture guidance
- Hardwired safety interlocks independent of software state
- Emergency stop and full power cutoff capability
- Industrial relay/contact-based safety systems
- Structured wiring and terminal documentation

---

### 🌐 Communications & Integration Layer
- Modbus TCP/RTU support
- BACnet compatibility for building systems
- MQTT telemetry for open monitoring
- REST API for system control and integration
- Optional OPC-UA bridge for industrial deployments

---

### 📊 Monitoring, Logging & Transparency
- Real-time thermal performance dashboards
- Historical heat recovery efficiency tracking
- Flow, ΔT, and energy transfer analytics
- Fault detection and diagnostic reporting
- Long-term data retention reference architecture

---

### 🧪 Thermal Modeling & Simulation Toolkit
- Open-source heat transfer simulation tools
- LMTD-based exchanger sizing calculators
- Pump and flow rate sizing models
- System efficiency prediction under variable load
- Digital twin support for pre-deployment validation

---

### 🏗️ Deployment & Commissioning Framework
- Step-by-step installation and commissioning guides
- Calibration procedures for sensors and control systems
- Startup and shutdown safety protocols
- Maintenance schedules and inspection workflows
- Standard operating envelopes for certified deployments

---

### 🧯 Fault Tolerance & Fail-Safe Architecture
- Automatic fallback to original cooling systems
- Pump fail-safe states (default OFF behavior)
- Thermal runaway prevention logic
- Independent mechanical safety overrides
- Isolation during exchanger failure or system fault

---

### 🔓 Open Standard Definition Layer
- Vendor-neutral thermal interface specification
- Interoperable design rules for compute-to-heat systems
- Multi-vendor ecosystem compatibility framework
- Publicly auditable energy recovery architecture
- Designed for municipal and institutional adoption

---

### 📜 AGPL 3.0+ Open Source Compliance Model
- All software components licensed under AGPL 3.0+
- Network-deployed modifications must remain open
- Attribution required under Section 7 to project maintainers
- Prevents proprietary enclosure of thermal infrastructure
- Encourages public and institutional transparency

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
  - [https://roxanneardary.com/hotside-collective/](https://roxanneardary.com/hotside-collective/)

---

## License & Notice Requirements

HotSide Collective is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- HotSide Collective specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Project Goal

HotSide Collective aims to turn waste heat from computing infrastructure into a **standardized, shareable utility layer for society**.

Instead of discarding energy, we design systems that **route it back into human environments where it has value**.

---

## Contributing

Contributions are welcome from:
- Mechanical engineers
- HVAC designers
- Data center operators
- Control systems engineers
- Open hardware developers
- Municipal infrastructure planners

All contributions must follow the licensing and notice requirements above.
