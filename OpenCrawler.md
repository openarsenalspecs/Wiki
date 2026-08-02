# OpenCrawler

**Open code. Honest search.**

OpenCrawler is an open-source search engine designed around transparency, fairness, and user control. Unlike traditional search systems that rely on opaque ranking systems and hidden data practices, OpenCrawler prioritizes explainable results, privacy-first design, and verifiable trust signals.

---

## Core Philosophy

OpenCrawler is built on four principles:

- **Transparency** — ranking logic is explainable and auditable  
- **Fairness** — no hidden boosting or pay-to-win ranking manipulation  
- **Privacy** — user data is encrypted and user-controlled  
- **Trust** — business and entity verification is built into search results  

---

## Core Features

### 1. FairRank™ Engine

A transparent ranking system that determines search order using measurable signals.

**Ranking factors include:**

- Relevance to query (40%)
- Trust signals (20%)
- Freshness (10%)
- Local relevance (10%)
- Content quality (10%)
- User utility (10%)

**Penalty systems:**

- Spam detection and suppression  
- Fraud risk penalties  
- Manipulation detection (link farms, fake engagement, keyword stuffing)

**Key Feature:**
- Every result can display an explanation of *why it ranked*

---

### 2. AI Business Verification Module

OpenCrawler verifies business entities using AI-assisted analysis of public records.

**Verification sources may include:**

- State business registries  
- Licensing databases  
- Address consistency checks  
- Entity name matching  
- Public compliance status signals  

**Output labels:**

- ✅ Verified Business  
- ⚠ Unverified / Needs Review  
- ❌ No Record Found  
- 🚩 Suspicious or Mismatched Entity  

---

### 3. Consent-Based Location Module

Location is never used without explicit user approval.

**Key behavior:**

- Location is OFF by default  
- Triggered only by “near me” type queries  
- Requires user confirmation before activation  

**User controls:**

- Allow once  
- Allow for session  
- Always ask  
- City-only mode  
- Manual location entry  
- Disable immediately after search  

**Precision options:**

- Exact location  
- Approximate area  
- City-level  
- State-level  

---

### 4. Fully Encrypted Data System

All stored data is encrypted by default.

**Encryption coverage:**

- User accounts  
- Preferences and settings  
- Optional search history  
- Location data (temporary or saved)  
- Business submissions  
- System logs (where applicable)  

**Security features:**

- Encryption in transit (TLS)  
- Encryption at rest (AES-class standards)  
- Optional field-level encryption  
- Secure key management  
- Automatic data deletion options  

---

### 5. Human-in-the-Loop Control System

OpenCrawler ensures users always retain control over system behavior.

**Includes:**

- Location permission prompts  
- Ranking transparency explanations  
- Business verification review flow  
- User-controlled privacy settings  
- Manual override options for all sensitive features  

---

### 6. Explainable Search Results

Every result can optionally show:

- Ranking reason breakdown  
- Trust indicators  
- Location relevance  
- Freshness score  
- Quality indicators  

---

### 7. Business Appeals & Corrections

Businesses can request review of:

- Incorrect verification status  
- Outdated information  
- Misidentified entity records  
- False fraud flags  

---

### 8. Privacy-First Architecture

OpenCrawler does not:

- Sell user data  
- Track users across sessions  
- Use hidden behavioral profiling  
- Enable silent location tracking  
- Apply undisclosed ranking boosts  

---

## Example Search Experience

**Query:** “plumber near me”

1. User is prompted for location permission  
2. User selects “Allow once”  
3. Results are shown with:

- Verified local plumbers  
- Distance-based ranking  
- Trust badges (if applicable)  
- Explanation of ranking factors  

---

## Technology Stack (Planned)

- Crawler subsystem (distributed or modular)  
- Indexing engine (inverted index / search DB)  
- FairRank™ scoring engine  
- AI verification layer  
- Privacy encryption layer  
- API backend  
- Frontend search interface  

---

## Project Structure (Suggested)

```text
opencrawler/
  crawler/
  indexer/
  fairrank/
  ai_verify/
  geochoice/
  encryption/
  api/
  frontend/
  docs/
  ```
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
  - [https://roxanneardary.com/opencrawler/](https://roxanneardary.com/opencrawler/)

---

## License & Notice Requirements

OpenCrawler is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- OpenCrawler specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
