# Oneiros

**Decode the dream. Become the man you’re meant to be.**

---

## 🌙 Overview

Oneiros is an **open-source dream interpretation and psychological development platform** designed specifically for men.  
It transforms recurring subconscious dreams about a mysterious feminine figure into **actionable insights, emotional growth, and relational readiness**.  

Oneiros is **not a dating app** — it is a tool for **inner alignment, emotional intelligence, and relational maturity**.  

---

## 🔑 Philosophy & Understanding

- Dreams reflect **subconscious simulations** of emotional, relational, and psychological patterns.  
- Recurring dream figures often symbolize aspects of **emotional capacity, attachment style, and inner feminine (anima) integration**.  
- The app focuses on **interpreting dreams, identifying patterns, and guiding users to actionable personal growth**.  
- All interpretations are probabilistic, psychologically grounded, and symbolic.  
- The system avoids claims of literal or supernatural visions and prevents obsessive thinking.  

---

## 🧩 Core Modules

### 1. Dream Intake Processor
- Logs dreams via text or voice  
- Extracts symbols, emotions, dreamer roles, tone, and recurrence  
- Outputs structured data for AI processing  

### 2. Symbolic Interpretation Engine
- Maps dream elements to psychological and archetypal meanings  
- Multi-layer analysis:  
  - Emotional Mirror  
  - Relational Blueprint  
  - Nervous System Indicator  
  - Inner Feminine Integration  

### 3. Emotional State & Trend Module
- Tracks emotional evolution across dreams  
- Metrics include emotional regulation, suppression index, anxiety likelihood, and openness trend  

### 4. Attachment & Relational Blueprint Module
- Infers attachment style and relational readiness  
- Provides trends over time and conflict response patterns  

### 5. Growth Path Recommendation Engine
- Generates personalized growth tasks:  
  - Emotional processing exercises  
  - Nervous system regulation  
  - Journaling prompts  
  - Communication and boundary training  
  - Masculine grounding routines  

### 6. Psychological Safety & Grounding Module
- Detects obsession or delusional thinking  
- Reframes dream interpretations as symbolic  
- Provides grounding guidance  

### 7. Dashboard & Visualization Module
- Visualizes emotional, attachment, and dream trends  
- Tracks growth task completion  

### 8. User Profile & Data Management Module
- Secure encrypted storage of dream history, insights, and growth progress  
- Supports self-hosting and data export  

### 9. [AI Model Training & Serving Module](https://gitlab.com/Roxanne_Ardary/oneiros/-/blob/b97ee636f33ff8b23d9a03a6602f92a270f99e40/AI%20Model%20Training%20and%20Serving.md)
- NLP entity extraction, emotion classification, archetype mapping, pattern recognition  
- Risk detection for unhealthy patterns  
- Continuous retraining on anonymized data  

### 10. Open-Source & Community Integration Module
- Fully open-source under AGPL-3.0  
- Community-editable symbol database and growth library  
- Documentation and contribution guides in `/documentation`  

---

## 💻 Tech Stack

**Backend:** FastAPI / Django  
**Database:** PostgreSQL + Weaviate / Milvus (semantic embeddings)  
**Task Queue:** Celery + Redis  
**AI Models:** LLaMA / Mistral / BERT / PyTorch / HuggingFace  
**Frontend:** React / React Native / Flutter  
**Charts / Dashboard:** Chart.js / D3.js  
**Voice Input:** Whisper / Vosk  
**Security:** AES-256 encryption, user-owned data, audit logs  

---

## 📈 User Experience

1. Log dream via text or voice  
2. AI parses symbols, emotions, and interactions  
3. Symbolic Interpretation Engine generates insights  
4. Emotional & attachment profiles update  
5. Growth Path Engine assigns personalized tasks  
6. Safety Monitor checks for unhealthy patterns  
7. Dashboard visualizes trends and progress  

---

## 🔓 Open Source Principles

- License: **AGPL-3.0**  
- Fully auditable AI logic  
- Community contributions encouraged for:  
  - Symbolic interpretations  
  - Growth exercises  
  - AI model improvements  
  - UI/UX enhancements  
  - Security and privacy  

---

## ⚠️ Safety & Ethical Guidelines

- Dreams are **symbolic, not literal**  
- Never encourage fixation on imagined figures  
- Promote **real-world grounding** and relational responsibility  

---

## 📚 Contribution

We welcome contributions to improve:

- Symbol database and archetype coverage  
- Growth exercises and journaling prompts  
- AI model interpretability and accuracy  
- UI/UX and accessibility  
- Security, privacy, and ethical compliance  

Please see **CONTRIBUTING.md** for guidelines.  

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
  - [https://roxanneardary.com/oneiros/](https://roxanneardary.com/oneiros/)

---

## License & Notice Requirements

Oneiros is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Oneiros is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
 specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution must also update `notice.md`.  
- When submitting a merge request (MR) or pull request (PR), ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
