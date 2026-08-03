# PhotonForge

**Open tools for next-generation optical array control systems.**

PhotonForge is a modular open-source framework for **array-level control of distributed optical emitters** such as VCSELs, laser diodes, LED arrays, and simulated photonic systems. It enables simulation, scheduling, feedback control, calibration, real-time execution, and distributed coordination of structured light systems.

Instead of controlling single emitters independently, PhotonForge treats light as a **coordinated, programmable field** governed by system-level behavior.

---

# 🧠 Core Concept

PhotonForge is built on a simple idea:

> Optical arrays should be programmable systems, not fixed hardware behaviors.

It provides a full pipeline from:
- physical modeling
- to scheduling
- to execution
- to feedback correction
- to distributed coordination

---

# 🚀 Key Features

## 🔦 Array-Level Optical Control
- Unified abstraction for NxM emitter grids
- Control of entire optical fields instead of single emitters
- Support for structured light behaviors and coordinated emission patterns

---

## ⏱ Deterministic Scheduling Engine
- Time-slot based emitter coordination
- Constraint-aware scheduling (thermal, power, interference)
- Spatial and temporal emission pattern generation
- Predictable execution model for hardware and simulation parity

---

## 🧬 Physical & System Modeling Layer
- Optical propagation modeling
- Interference and diffusion approximations
- Thermal drift modeling
- Sensor response modeling
- Physics-consistent simulation environment

---

## 🧪 High-Fidelity Simulation Environment
- Full virtual emitter arrays
- Noise and signal distortion modeling
- Sensor feedback emulation
- Environment variability simulation
- Hardware-free development workflow

---

## 📡 Closed-Loop Feedback Control
- Real-time sensor signal analysis
- Per-emitter drift detection
- Adaptive correction signals
- Signal quality optimization loops
- Continuous calibration refinement

---

## ⚡ Real-Time Execution Engine
- Deterministic control loop execution
- Microsecond-level scheduling support (hardware dependent)
- Jitter reduction and synchronization
- Hardware-safe timing enforcement layer

---

## 🔌 Hardware Abstraction Layer
- Unified API for optical hardware systems
- Support for LED, VCSEL, laser diode drivers
- GPIO / PWM / FPGA integration layer
- Swap hardware without changing control logic

---

## 🌐 Distributed Optical Network Control
- Multi-device synchronization
- Clustered emitter array coordination
- Network-based control of distributed optical systems
- Multi-node sensor fusion support

---

## 📊 Optimization & Control Intelligence
- Emission pattern optimization under constraints
- Energy and thermal efficiency balancing
- Adaptive tuning strategies
- Optional ML/RL integration for system optimization

---

## 📈 Telemetry & Observability System
- Per-emitter usage tracking
- Thermal and performance monitoring
- Scheduler efficiency analytics
- Signal quality trend tracking
- Debugging and diagnostics framework

---

## 🧩 Developer API
- Python-first interface
- Scriptable optical behaviors
- Programmatic array control
- Extensible architecture for custom modules

---

## 🧪 Examples & Benchmarks
- 8×8 emitter simulation demo
- Feedback loop correction examples
- Scheduler performance tests
- Simulation vs hardware validation benchmarks

---

# 🧱 Modular Architecture
```text
PhotonForge/
├── core/
├── scheduler/
├── models/
├── simulation/
├── feedback/
├── realtime/
├── hardware/
├── network/
├── optimization/
├── telemetry/
├── api/
├── examples/
├── benchmarks/
├── docs/
```

---

# 🔄 System Flow

```text
User Intent
    ↓
API Layer
    ↓
Scheduler / Pattern Engine
    ↓
Physical Models
    ↓
Optimization Layer
    ↓
Realtime Execution Engine
    ↓
Core Emitter Control
    ↓
Hardware / Simulation Backend
    ↓
Feedback + Telemetry
    ↓
Optimization Loop (closed cycle)
```
# 🧭 Design Principles

- Array-first control (no single-emitter thinking)
- Hardware abstraction (simulation ↔ real systems parity)
- Deterministic execution where possible
- Feedback-driven adaptation
- Modular extensibility
- Safety-aware control architecture

---

# ⚠️ Safety Note

PhotonForge may be used with optical hardware systems, including high-intensity emitters. Users are responsible for ensuring compliance with all applicable laser and electrical safety standards. Safety constraints should be enforced at the hardware and realtime layers.

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
  - [https://roxanneardary.com/photonforge/](https://roxanneardary.com/photonforge/)

---

# 📜 License & Notice Requirements

PhotonForge is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- PhotonForge specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

# 🤝 Contributing

Contributions are welcome. Please ensure all changes align with the modular architecture and maintain compatibility with the AGPL-3.0+ licensing requirements.

---

# 🌐 Vision

PhotonForge aims to become a foundational open framework for **programmable optical systems**, enabling research and development in:

- structured light systems  
- adaptive photonic arrays  
- LiDAR and sensing systems  
- optical simulation and control theory applications  
