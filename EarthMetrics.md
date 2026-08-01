# EarthMetrics
### Observation Without Interpretation.

**EarthMetrics** is an open-source global database dedicated to preserving **measured environmental observations of Earth’s systems**.

It aggregates **historical and real-time measurements** across atmospheric, oceanic, geological, hydrological, and cryospheric domains—starting from the **earliest recorded observations to the present day**.

EarthMetrics records **what was measured**, not what it means.

---

# 🌍 Mission

To create the **most complete, transparent, and verifiable open record of Earth's environmental measurements in history**.

EarthMetrics ensures that all data is:

- factual and measurement-based  
- fully traceable to its source  
- reproducible by anyone  
- permanently preserved  
- openly accessible  

---

# 🧭 Core Principle

## Observation Without Interpretation

EarthMetrics strictly separates:

- **Observation (data)**  
from  
- **Interpretation (meaning)**  

The system does **not store**:

- causes  
- conclusions  
- predictions  
- models  

---

# 🔬 Scientific Philosophy

Observation ≠ Explanation
Measurement ≠ Conclusion
Correlation ≠ Causation


EarthMetrics provides the **raw foundation for science**, not the conclusions.

---

# ⚙️ Key Features

## 🌐 Global Historical Record
- Integrates environmental measurements from **1600s → present**
- Includes weather stations, ship logs, satellites, buoys, seismic data, and more

---

## 🧱 Immutable Raw Data Layer
- Append-only database  
- No overwrites or silent edits  
- Original measurements preserved exactly  

---

## 🔗 Full Data Provenance
Every record includes:

- source archive  
- station or sensor ID  
- instrument ID  
- timestamp  
- geographic location  
- measurement method  

---

## 🧪 Instrument Registry
Global catalog of measurement devices:

- thermometers  
- satellites  
- ocean buoys  
- seismographs  

Includes accuracy, method, and manufacturer data.

---

## 🛠 Calibration Logs
Tracks when and how instruments were calibrated to ensure transparency in measurement accuracy.

---

## 📊 Data Confidence Layer
Provides context without interpretation:

- sensor accuracy  
- completeness  
- anomaly flags  

---

## 🔄 Multi-Source Parallel Observations
Multiple measurements are stored side-by-side:

- no averaging  
- no merging  
- no “corrected truth”  

---

## ⚖️ Raw vs Adjusted Data Separation
Both raw and adjusted values are stored (when applicable), clearly labeled.

---

## 🧬 Data Lineage Tracking
Every data point can be traced back to its original source and instrument.

---

## 🔐 Immutable Ledger System
- cryptographic hashing  
- append-only records  
- distributed mirrors  
- full version history  

---

## 📦 Versioned Datasets
All dataset imports are versioned and preserved.

---

## 🗺 Data Gaps Mapping
Highlights missing or sparse data regions and time periods.

---

## 🌪 Event Indexing
Data is indexed by observed events:

- hurricanes  
- earthquakes  
- floods  
- droughts  

(No causal interpretation included)

---

## ⏳ Historical Replay (“Time Machine”)
View Earth’s recorded state at any point in history.

---

## 🔎 Open Query Engine
Custom queries across time and space:

```sql
SELECT *
FROM observations
WHERE location_radius(50km, Miami)
AND date BETWEEN 1900 AND 1950;
```

## 📏 Unit Preservation

Stores both:

original measurement units
standardized units

## 🌐 Citizen Sensor Network

Supports public data contributions with verification layers.

## 🌍 Distributed Mirror Network

Global redundancy through:

universities
independent hosts
public nodes

## 💾 Offline Archive Access

Full dataset downloads for long-term preservation and independent research.

## 🔌 API & Developer Ecosystem

Open APIs for:

data access
third-party tools
independent analysis

## 📜 Historical Document Archive

Digitized:

handwritten logs
ship journals
early scientific records

## 📡 Planetary Dashboard

Live global visualization of:

temperature
pressure
ocean conditions
seismic activity

## 🧱 Architecture Overview

Data Sources
    ↓
Ingestion Pipeline
    ↓
Raw Observation Store (Immutable)
    ↓
Metadata & Provenance
    ↓
Integrity Layer
    ↓
API & Query Engine
    ↓
Visualization / External Analysis

## 📊 Data Categories

Atmosphere
Oceans
Cryosphere
Hydrology
Geology

## 🔍 Transparency Rules

Raw data is never modified
All changes are logged
Every record is traceable
No interpretation is stored
Data remains publicly accessible

## 🧑‍🤝‍🧑 Contributing

We welcome:

developers
researchers
data scientists
historians
citizen scientists
Ways to contribute:
digitize historical records
integrate public datasets
build ingestion pipelines
improve documentation
develop tools and visualizations

## 🛣 Roadmap

Phase 1
core database
historical data ingestion
metadata schema

Phase 2
API and query engine
automated ingestion

Phase 3
dashboards
citizen sensor network
distributed mirrors

Phase 4
global completeness

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
  - [https://roxanneardary.com/earthmetrics/](https://roxanneardary.com/earthmetrics/)

---

## 📜 License & Notice Requirements

EarthMetrics is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**
- EarthMetrics specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

## 🌎 Vision

EarthMetrics aims to become:

The permanent, open, and verifiable record of Earth's environmental measurements.

EarthMetrics
Observation Without Interpretation.

Measuring the planet. Recording the facts.
