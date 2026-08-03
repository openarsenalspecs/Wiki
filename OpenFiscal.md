# OpenFiscal – From Deficit to Accountability

**OpenFiscal** is an open-source platform designed to track, analyze, and audit government budgets at every level—town, city, state, and federal. The project provides **full fiscal transparency**, AI-driven insights, and accountability for officials involved in budget approval. It is designed to flag deficits, line-item anomalies, and potential misuse of public funds, promoting responsible governance.

---

## Key Features

### Core Budget Tracking
- Track **budgets for all jurisdictions** (town, city, state, federal)  
- Store **actual revenue, expenditure, and deficit** per fiscal year  
- Link budgets to **jurisdiction GDP** for context  
- Map **officials involved** in drafting, reviewing, and approving budgets  
- Calculate **deficit % relative to GDP**  
- Automatic **flagging for deficits >3% of GDP**  

### Line Item AI Auditing
- Track **individual budget line items** with category, amount, vendor, and notes  
- AI analyzes line items vs **national/state averages**  
- **Flag line items >10% above average** for investigation  
- Provide **recommendations** for flagged items (fraud, no-bid contracts, cronyism)  
- Assign **risk scores** and maintain historical trends per vendor  
- Human-in-the-loop verification required before final recommendation  

### Officials & Accountability
- Maintain **official profiles** with position, party, and term info  
- Track **role in budget process** (drafter, committee member, approver)  
- Maintain **vote history per budget**  
- Calculate **re-election risk scoring** based on budget approval behavior  
- Publicly viewable **official budget track record**

### AI-Driven Insights
- **Anomaly detection** for unusual spikes in revenue or expenditure  
- **Predictive deficit alerts** for upcoming fiscal years  
- **Budget optimization suggestions**  
- **Natural language parsing** for PDF and document budgets  
- **Machine learning forecasting** for fiscal stress or potential crises  

### Public Transparency & Engagement
- Interactive **dashboards** for citizens, journalists, and researchers  
- **API access** for querying budgets, GDPs, officials, and line items  
- **Notifications** for flagged budgets, officials, or line items  
- **Citizen feedback module** for flagged items or budgets  

### Comparative Analytics
- **Cross-jurisdiction comparison** of budgets  
- **Peer benchmarking** for towns/states of similar size  
- **Historical ranking** of jurisdictions by fiscal responsibility  

### Governance & Compliance
- **Immutable audit trail** for all budgets, line items, flags, and human reviews  
- Support for **multi-level approvals** (local → state → federal)  
- **Legal compliance checks** against balanced budget rules  
- **Human-in-the-loop verification** for AI-generated recommendations  

### Advanced / Experimental Features
- **Interactive “what-if” simulation** for revenues/expenditures  
- **Election overlay** linking officials’ budget votes to election outcomes  
- Optional **blockchain logging** for tamper-proof budget records  
- Predictive **line-item risk modeling** for fraud or cronyism  

---

## Data Sources
- Federal: US Treasury, Census Bureau  
- State: State budget offices, open-data portals  
- Local: Municipal finance departments, open budgets  

All budgets are normalized for consistent tracking, analysis, and reporting.

---

## Workflow Overview
1. **Data Ingestion:** Pull budget datasets or PDFs and normalize into the database  
2. **Line-Item & Budget Analysis:** AI calculates deficit %, compares line items to national averages, and flags anomalies  
3. **Human Review:** Human-in-the-loop verifies flagged items and updates the audit log  
4. **Reporting & Dashboard:** Generate reports and interactive dashboards for public transparency  
5. **Notifications:** Alerts for overspending, flagged line items, and high-risk officials  

---

## Installation & Setup
- Clone the repository  
- Set up the database (PostgreSQL recommended)  
- Run data ingestion scripts to import budgets and officials  
- Configure AI flagging and anomaly detection modules  
- Deploy dashboards and API endpoints  

*(Detailed setup scripts and examples are included in the `docs` directory)*

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
  - [https://roxanneardary.com/openfiscal/](https://roxanneardary.com/openfiscal/)

---

## License & Notice Requirements

OpenFiscal is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- OpenFiscal specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

**OpenFiscal – From Deficit to Accountability** empowers citizens, auditors, and governments to make budgets transparent, accountable, and fair.
