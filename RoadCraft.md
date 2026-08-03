# RoadCraft
### The AI Copilot for Every Rider

RoadCraft is an open-source AI-assisted motorcycle intelligence system that integrates helmet-based computing, vehicle control systems, real-time sensor fusion, and optional emergency AI intervention to improve rider safety without removing rider control.

It is designed as a modular, extensible platform combining **embedded hardware systems, edge AI, V2X communication, and stabilization technologies**.

---

## Core Philosophy

RoadCraft is built on three principles:

- **Rider First:** The human always retains primary control.
- **Safety Only Intervention:** AI intervenes only in verified emergency conditions.
- **Open Systems:** Fully open-source hardware and software under AGPL-3.0+.

---

## Full Feature List

### 1. AI Copilot & Riding Intelligence
- Real-time AI riding assistance with optional manual control mode
- Emergency-only AI override for collision prevention and stability correction
- Predictive hazard detection using multi-sensor fusion (camera, radar, lidar, IMU)
- Lane tracking, object detection, and trajectory risk forecasting
- Adaptive rider modeling based on behavior, braking style, and lean patterns
- Personalized AI tuning over time per rider profile

---

### 2. Helmet AI System
- Embedded edge AI compute unit integrated into helmet shell
- Heads-Up Display (HUD) for navigation, alerts, and system status
- Bone conduction audio system for non-intrusive voice feedback
- Real-time voice assistant for navigation and system control
- Haptic feedback system:
  - Blind spot alerts
  - Collision warnings
  - Stability correction cues
- Multi-level alert system (informational, caution, critical)

---

### 3. Motorcycle Control System (Drive-by-Wire)
- Electronic throttle control (throttle-by-wire)
- Electronic braking control (brake-by-wire)
- Steering assist input for stability correction
- AI-assisted emergency braking system (safety-only activation)
- CAN-FD real-time communication between subsystems
- Manual override prioritization at hardware level

---

### 4. Stabilization Hardware System
- Active gyroscopic stabilization module integrated into motorcycle frame
- IMU-driven balance correction system
- Low-speed stability support (stop-and-go traffic assistance)
- Electronic suspension adjustment system:
  - Real-time damping control
  - Terrain-based adaptive stiffness
- Optional retractable micro-stabilizer arms for stationary balance

---

### 5. Sensor Fusion System
- Front and rear HD wide-angle cameras
- Radar-based motion and speed detection
- Lidar-based 3D environmental mapping
- High-precision IMU (acceleration, rotation, tilt)
- RTK GPS for centimeter-level positioning
- Rider biometric sensors (optional):
  - Eye tracking
  - Fatigue and attention monitoring

---

### 6. Navigation & GPS Intelligence
- Satellite-enhanced RTK navigation system
- Dynamic rerouting based on traffic and hazard detection
- Offline navigation support
- AI-based route prediction based on rider habits
- Real-time road condition analysis

---

### 7. Vehicle-to-Vehicle (V2V) & Network Communication
- Helmet-to-helmet encrypted mesh communication
- AI-to-AI hazard broadcasting between RoadCraft systems
- Vehicle-to-infrastructure (V2X) compatibility
- Real-time hazard alerts from nearby vehicles
- Secure, anonymized safety data exchange

---

### 8. Helmet Hardware Architecture
- Embedded AI processor (Jetson / Snapdragon-class edge compute)
- Modular PCB architecture for sensor and compute expansion
- Thermal management system for enclosed helmet environment
- Dual redundant battery system
- Secure wireless communication module (helmet ↔ motorcycle)

---

### 9. Motorcycle Embedded Hardware System
- Central vehicle ECU for AI integration
- CAN-FD bus for real-time system communication
- Electronic stability controller integration
- Power distribution unit with AI load management
- Modular sensor mounting framework

---

### 10. Safety & Override System
- Hardware-level emergency override circuit
- Watchdog microcontroller for system integrity monitoring
- Multi-sensor validation before AI intervention
- Physical kill switch for full rider control restoration
- Fail-safe default behavior: immediate return to manual control

---

### 11. Simulation & Testing Framework
- Hardware-in-the-loop (HIL) testing support
- Digital twin simulation of motorcycle dynamics
- Scenario-based AI testing:
  - Emergency braking
  - Collision avoidance
  - Loss of traction recovery
- Integration with CARLA / LGSVL simulation environments
- Reinforcement learning training pipeline for AI models

---

### 12. Open-Source Architecture
- Fully modular ROS-based system design
- Plug-and-play hardware and software modules
- Dockerized development and testing environments
- Open API for third-party AI modules
- Community-driven hardware expansion support

---

## Tech Stack Overview

- **AI Frameworks:** PyTorch, TensorFlow, RLlib
- **Computer Vision:** YOLOv9, Detectron2, OpenCV
- **Middleware:** ROS 3.0, gRPC, MQTT
- **Embedded Systems:** C++, Rust, STM32, Jetson Orin / Snapdragon Ride
- **Simulation:** CARLA, LGSVL
- **Networking:** 5G mmWave, DSRC, V2X mesh networking
- **Navigation:** RTK GPS, GNSS multi-band systems

---

## Project Structure (Planned)
- `helmet_ai/` – Edge AI and sensor fusion
- `vehicle_control/` – Motorcycle drive-by-wire system
- `stabilization/` – Gyroscopic and balance control systems
- `communication/` – V2V, V2X, and networking layer
- `simulation/` – Testing and digital twin environment
- `hardware/` – Schematics, PCB layouts, and BOM
- `docs/` – Architecture, design, and development guides

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
  - [https://roxanneardary.com/roadcraft/](https://roxanneardary.com/roadcraft/)

---

## License & Notice Requirements

RoadCraft is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- RoadCraft specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the project’s `notice.md` file.

---

## Status

RoadCraft is currently in early development. Core focus areas include:
- Sensor fusion prototype
- Helmet AI edge compute system
- Simulation-first safety validation
- Drive-by-wire motorcycle integration layer
