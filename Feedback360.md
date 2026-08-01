# Feedback360

**See the Full Picture of Public Opinion**

Feedback360 is a modular civic intelligence platform that enables legislators to understand constituent sentiment on each individual line item of a bill. It uses AI to translate complex legislation into plain language, collect structured public feedback, and generate secure, aggregated insights that support informed, transparent decision-making.

---

## Overview

Modern legislation is complex and often inaccessible to the public. Feedback360 bridges this gap by breaking down bills into understandable components and allowing constituents to respond directly to each part. The system then uses AI to analyze, cluster, and summarize feedback so representatives can clearly see how each policy element is perceived by the public.

The platform is built with a **modular architecture**, enabling scalability, extensibility, and integration with government systems.

---

## Core Features

### Legislative Breakdown Engine
- Parses bills into structured line items
- Converts legal language into plain, readable summaries
- Identifies purpose, scope, and intent of each clause
- Highlights affected groups and policy domains

### Policy Impact Analysis
- Estimates cost implications per line item
- Analyzes tax increases or decreases
- Identifies budget reallocations and funding sources
- Flags high-impact or high-sensitivity provisions
- Provides short-term and long-term impact summaries

### Constituent Feedback System
- Free-text feedback per legislative line item
- Optional anonymous or verified submissions
- Mobile-friendly and accessible interface
- Structured capture of public sentiment

### AI Feedback Understanding & Clustering
- Sentiment classification (support / oppose / neutral)
- Thematic clustering of similar responses
- Extraction of key concerns and recurring themes
- Aggregated statistical summaries of public opinion
- Noise reduction across large datasets

### Representative Dashboard
- Real-time sentiment visualization per bill section
- Line-item comparison of public opinion
- Trend tracking across bill versions
- Exportable reports for caucus and committee review
- Drill-down into thematic feedback clusters

### Legislative Change Tracking
- Version control for bills and amendments
- Automatic re-analysis when legislation changes
- Comparison between bill versions
- Alerts for significant shifts in sentiment

### Security & Privacy Layer
- AES-256 encryption at rest
- TLS 1.3 encryption in transit
- Role-based access control
- Aggregated output only (no raw identity exposure by default)
- Secure separation of raw input and analytics layers

### API & Integration Layer
- Secure APIs for external government systems
- Support for legislative databases and portals
- Modular endpoints for each system component
- Extensible architecture for future civic tools

### Accessibility & Usability
- Plain-language explanations for all outputs
- Mobile-first design for broad accessibility
- Multi-device support (desktop, tablet, mobile)
- Designed for non-technical users across all education levels

### Open Governance & Transparency
- Fully open-source under AGPL-3.0+
- Network-deployed systems remain open and auditable
- Encourages civic transparency and accountability
- Supports public trust through verifiable systems

---

## Modular Architecture

Feedback360 is built as a set of independent, interoperable modules:

- Legislative Parsing Module
- Impact Analysis Module
- Constituent Input Module
- AI Aggregation Module
- Security & Privacy Module
- Analytics & Visualization Module
- Legislative Change Tracking Module
- API & Integration Layer
- Open Governance Layer

Each module can scale independently, be replaced, or be extended without affecting the core system.

---

## Tech Stack

- **Frontend:** React (responsive web interface)
- **Backend:** Node.js + Express
- **Databases:** PostgreSQL (structured data), MongoDB (feedback + AI outputs)
- **AI Layer:** GPT-based model for legislative breakdown and sentiment analysis
- **Analytics:** Python (Pandas, NumPy, Scikit-learn)
- **Security:** AES-256 encryption at rest, TLS 1.3 in transit
- **Deployment:** Cloud-agnostic (AWS / GCP / Azure), Dockerized services
- **License:** GNU Affero General Public License v3.0 or later (AGPL-3.0+)

---

## Use Cases

- Legislative committees reviewing public opinion on bills
- Congressional and state representatives gathering constituent input
- Policy analysis teams tracking sentiment trends
- Civic organizations increasing government transparency
- Public engagement platforms for municipalities and agencies

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
  - [https://roxanneardary.com/feedback360/](https://roxanneardary.com/feedback360/)

---

## License & Notice Requirements

Feedback360 is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Feedback360 specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
