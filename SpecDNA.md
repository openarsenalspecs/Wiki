# SpecDNA
**Human Directed Evolution for AI Specifications**
- HTML Mirror:  [https://roxanneardary.com/specdna-specification/](https://roxanneardary.com/specdna-specification/)  

---

SpecDNA is a specification for AI agents that evolve, fork, modify, and extend existing specifications under human direction while preserving provenance, licensing, attribution, intellectual property analysis, and human intent.

SpecDNA establishes a controlled evolution process in which an AI agent treats an existing specification as inherited source material rather than an independent creation. Every modification must remain traceable to its source specification, applicable licenses, previous creators, human instructions, AI transformations, and resulting changes.

## Purpose

SpecDNA provides a framework for responsible AI assisted evolution of specifications.

The system is designed to:

- Preserve specification lineage across forks and derivative versions.
- Preserve licensing and attribution requirements.
- Record human instructions that direct specification changes.
- Distinguish inherited, modified, human generated, AI generated, third party, removed, and unknown content.
- Analyze potential copyright conflicts.
- Analyze potential patent conflicts.
- Analyze license compatibility and attribution requirements.
- Assign risk scores to identified intellectual property concerns.
- Recommend modifications and design arounds intended to reduce identified risks.
- Preserve human authority over consequential changes.
- Generate and maintain a complete `notice.md` record.
- Maintain an auditable provenance chain for every evolved specification.
- Support modular extensions through optional plugins.

---

## Core Principles

### Human Directed

The human in the loop remains the authority over the intended evolution of a specification.

AI agents may analyze, recommend, transform, and generate content, but they must operate within the instructions, constraints, and approvals established by the human.

### Provenance Preservation

Every evolved specification must retain a traceable relationship to its known source specifications, creators, versions, licenses, and transformation history.

Provenance must not be intentionally removed, concealed, falsified, or materially altered in a manner that obscures lineage.

### License Preservation

The AI agent must identify applicable licenses before modifying an inherited specification and must preserve compatible licensing and attribution requirements throughout the evolution process.

### Intellectual Property Awareness

Copyright and patent analysis must be performed as risk assessment and evidence gathering rather than as a definitive legal determination.

The system must identify potentially relevant concerns and provide information that can support human or qualified legal review.

### Transparent Evolution

Material changes must be identifiable and attributable to their source, human direction, AI transformation, or third party contribution.

### Modular Design

Core functionality must remain independently understandable and replaceable.

Optional capabilities must be implemented as modules or plugins without requiring the core system to depend on any particular external service, database, model, or provider.

### Auditability

Significant transformation events, risk assessments, human decisions, provenance changes, and output versions must be capable of being recorded and independently reviewed.

---

## Core Modules

### Specification Intake Module

The Specification Intake Module receives and analyzes the specification selected for evolution.

It must identify, where available:

- Specification name.
- Creator information.
- Version.
- Source location.
- Repository information.
- Commit or content identifier.
- License.
- Attribution requirements.
- Existing notices.
- Existing provenance records.
- Existing contributor information.
- Existing intellectual property notices.
- Existing third party materials.
- Existing modification history.

The module must preserve the original specification as an immutable reference for the transformation process.

### Human Instruction Module

The Human Instruction Module captures the human's intended modification.

It must support:

- Modification requests.
- New requirements.
- Removed requirements.
- Design constraints.
- Functional objectives.
- Prohibited changes.
- Preferred changes.
- Explicit approvals.
- Explicit rejections.
- Requests for design alternatives.
- Requests for risk reduction.

Human instructions must be associated with the resulting transformation whenever practical.

### Fork and Transformation Module

The Fork and Transformation Module creates the new specification from the inherited specification and the human instructions.

The module must:

- Preserve inherited content where unchanged.
- Identify modified content.
- Identify removed content.
- Identify newly generated content.
- Associate material changes with their transformation source.
- Preserve inherited licensing and attribution information.
- Prevent the AI agent from representing inherited material as independently originated.
- Produce a transformation record.

The transformation process must not intentionally erase provenance in order to make the resulting specification appear independently created.

### Provenance Module

The Provenance Module maintains the lineage of the specification.

A provenance record should include, when available:

- Original specification.
- Original creator.
- Original version.
- Original source.
- Original commit or content hash.
- Previous versions.
- Previous creators.
- Applicable licenses.
- Attribution requirements.
- Human instructions.
- Human decisions.
- AI agent identity.
- AI model identity when available.
- Transformation identifier.
- Transformation timestamp.
- Content classifications.
- Material changes.
- Risk assessments.
- Review decisions.
- Resulting version.
- Resulting content hash.

The provenance chain must remain associated with every subsequent generation.

### License Compliance Module

The License Compliance Module evaluates the license governing the inherited specification and identifies obligations relevant to the proposed transformation.

It must evaluate, where applicable:

- License compatibility.
- Copyleft requirements.
- Attribution requirements.
- Notice requirements.
- Source availability requirements.
- Modification requirements.
- Distribution requirements.
- Network deployment requirements.
- Third party license obligations.
- Additional licensing conditions.

The module must identify conflicts before finalizing a transformation whenever sufficient information is available.

### Notice Generation Module

The Notice Generation Module creates or updates `notice.md` whenever a fork, derivative version, substantial modification, or other traceable evolution event occurs.

The generated notice must preserve known:

- Previous creators.
- Previous versions.
- Source specifications.
- Source repositories.
- Source identifiers.
- Licenses.
- Attribution requirements.
- Contributor acknowledgments.
- Material modifications.
- Human instructions.
- AI transformations.
- Current creator.
- Current version.
- Current creation date.
- Description of the new creation or modification.

The notice must not be removed or materially modified in a manner that conceals specification lineage, licensing history, attribution requirements, or contributor history.

### Copyright Analysis Module

The Copyright Analysis Module evaluates the resulting specification for potential copyright concerns.

It should analyze:

- Similarity to inherited material.
- Substantial retained expression.
- Potentially protected expressive material.
- Third party material.
- Reused text.
- Reused examples.
- Reused documentation.
- Reused creative content.
- Transformation characteristics.

The module must distinguish factual similarity, functional similarity, conceptual similarity, and potentially protectable expressive similarity where the available analysis permits.

The module must produce evidence and explain the basis for its assessment.

The module must not represent its analysis as a definitive legal determination.

### Patent Analysis Module

The Patent Analysis Module evaluates the specification for potential patent conflict indicators.

It should analyze:

- Functional requirements.
- Technical mechanisms.
- Claimed methods.
- Described processes.
- Potentially relevant patent documents.
- Patent status information where available.
- Patent families where available.
- Jurisdictional information where available.
- Relevant prior art indicators.

The module should identify potentially relevant patents or patent claims and explain why they may warrant further review.

The module must not represent an automated patent analysis as a definitive infringement or freedom to operate determination.

### Intellectual Property Risk Scoring Module

The Intellectual Property Risk Scoring Module converts identified concerns into structured risk assessments.

The system should support separate scores for:

- Copyright Risk.
- Patent Risk.
- License Risk.
- Attribution Risk.
- Provenance Risk.
- Third Party Material Risk.
- Derivative Work Risk.
- Overall Intellectual Property Risk.

Risk scores should use a consistent scale from 0 to 100.

Suggested classifications:

- 0 to 19: Minimal.
- 20 to 39: Low.
- 40 to 59: Moderate.
- 60 to 79: Elevated.
- 80 to 100: Critical.

Each score should include:

- Score.
- Classification.
- Evidence.
- Reasoning.
- Affected material.
- Confidence level.
- Recommended action.

A critical license or provenance violation must not be obscured by averaging it with lower risk scores.

### Modification Recommendation Module

The Modification Recommendation Module generates alternatives intended to reduce identified risks while preserving the human's intended objectives.

Recommendations may include:

- Rewriting expressive material.
- Replacing examples.
- Removing unnecessary inherited language.
- Replacing potentially conflicting mechanisms.
- Separating functional requirements from expressive implementation details.
- Creating alternative technical approaches.
- Replacing third party material.
- Adding appropriate attribution.
- Preserving required notices.
- Seeking human or legal review.

Recommendations must explain the tradeoff between risk reduction and preservation of human intent.

The AI agent must not silently implement a risk reducing recommendation that materially changes the human's intended outcome.

### Human Review Module

The Human Review Module provides the human in the loop with the information necessary to approve or reject consequential transformations.

Review records should support:

- Accepted.
- Rejected.
- Modified.
- Deferred.
- Escalated for legal review.

Human review should be required when:

- Provenance is uncertain.
- License compatibility is uncertain.
- Attribution requirements are unclear.
- Copyright risk is elevated.
- Patent risk is elevated.
- A proposed design around materially changes functionality.
- The AI cannot reliably determine whether inherited content may be retained.
- A request conflicts with an inherited provenance or licensing requirement.

### Integrity and Audit Module

The Integrity and Audit Module records significant events in the specification evolution process.

Audit records should include:

- Source specification.
- Human instruction.
- AI transformation.
- Content changes.
- Risk analysis.
- Recommendations.
- Human decisions.
- License assessment.
- Notice generation.
- Output version.
- Content integrity information.

The system should support content hashes or equivalent integrity mechanisms to help establish that recorded versions correspond to the analyzed specifications.

### Export Module

The Export Module produces the resulting specification and associated records.

A completed evolution should be capable of producing:

- Modified specification.
- Provenance record.
- Updated `notice.md`.
- License information.
- Copyright assessment.
- Patent assessment.
- License assessment.
- Risk scores.
- Recommendations.
- Human review record.
- Transformation record.

---

## Content Lineage

SpecDNA should classify specification content using standardized lineage categories.

### INHERITED

Content retained from an earlier specification without material modification.

### MODIFIED

Content derived from inherited material and materially changed during evolution.

### HUMAN GENERATED

Content directly supplied or authored by the human in the loop.

### AI GENERATED

Content generated by the AI agent without direct reuse of an identified source passage.

### THIRD PARTY

Content originating from a source outside the specification's established lineage.

### REMOVED

Content present in an earlier version that was intentionally removed during evolution.

### UNKNOWN

Content whose origin cannot currently be established with sufficient confidence.

Unknown lineage must trigger a provenance warning when the material is significant to the resulting specification.

## Provenance Requirements

Every transformation must attempt to establish the source lineage before generating the resulting specification.

The system must not intentionally:

- Remove known creator information.
- Remove known license information.
- Remove required attribution.
- Conceal inherited material.
- Falsify authorship.
- Falsify origin.
- Represent an inherited specification as independently created.
- Delete material provenance solely to reduce apparent intellectual property risk.

If the human requests removal of required provenance or attribution, the request must be identified as a provenance or licensing conflict and presented for explicit review.

## License Requirements

The AI agent must inspect the inherited license before transformation.

If the inherited license is incompatible with the intended transformation or distribution, the system must identify the conflict before finalization.

The resulting specification must preserve applicable license and attribution requirements unless a lawful and documented licensing change is established.

Where multiple licenses apply, the system must maintain records identifying the source and scope of each applicable license.

## Copyright Risk Requirements

Copyright analysis must consider both retained inherited expression and newly generated material that may resemble third party material.

The system should identify:

- Source material.
- Similar material.
- Similarity basis.
- Degree of transformation.
- Potentially protected expression.
- Applicable license information.
- Confidence in the analysis.

Copyright risk scoring must remain advisory.

## Patent Risk Requirements

Patent analysis must consider the jurisdiction, available patent information, relevant claims, patent status, and technical scope when such information is available.

The system should distinguish:

- Potentially relevant patent.
- Potentially relevant claim.
- Technical overlap.
- Jurisdictional relevance.
- Status uncertainty.
- Evidence confidence.

Patent risk scoring must remain advisory and must not be presented as a legal conclusion.

## Design Around Requirements

When elevated intellectual property risk is identified, SpecDNA should attempt to produce alternative designs that preserve the human's intended objectives.

A design around should document:

- Original requirement.
- Identified risk.
- Proposed alternative.
- Function preserved.
- Function changed.
- Risk potentially reduced.
- New tradeoffs.
- Human approval status.

The AI agent must not prioritize risk reduction by silently eliminating essential human requirements.

## Notice Requirements

Every evolved specification must contain or reference a current `notice.md` record.

The notice should establish:

- Current specification.
- Current version.
- Current creator.
- Current creation date.
- Current modification description.
- Original specification.
- Original creator.
- Original source.
- Original version.
- Original license.
- Version lineage.
- Contributor history.
- Human instructions.
- AI transformation.
- Current licensing.
- Attribution requirements.
- Intellectual property review.
- Provenance status.

Each subsequent generation must extend the existing lineage rather than replace it with only the most recent version.

## Human Intent Preservation

The system must maintain a distinction between:

- What the human requested.
- What the AI interpreted.
- What the AI recommended.
- What the AI changed.
- What the human approved.
- What the final specification contains.

Material differences between human intent and the resulting specification must be identified before finalization.

## Conflict Handling

The system must halt or escalate a transformation when it cannot safely establish required provenance or licensing information.

Potential conflict states include:

- Unknown Source.
- Unknown License.
- Missing Attribution.
- License Conflict.
- Provenance Conflict.
- Copyright Concern.
- Patent Concern.
- Third Party Material Concern.
- Human Intent Conflict.
- Insufficient Evidence.
- Legal Review Required.

The system must preserve the conflict record even if the human chooses to continue.

---

## Optional Plugin Modules

### Repository Integration Plugin

Provides integration with source repositories for retrieving versions, commits, branches, contributors, and historical changes.

### Git Integration Plugin

Provides commit history, content hashes, branch lineage, change tracking, and automated provenance records.

### Copyright Database Plugin

Connects to external copyright records and related databases for expanded analysis.

### Patent Database Plugin

Connects to patent databases for patent document, claim, family, status, and jurisdiction analysis.

### Prior Art Search Plugin

Provides expanded prior art discovery for patent risk analysis.

### Patent Family Analysis Plugin

Identifies related patent family members and jurisdictional relationships.

### Similarity Analysis Plugin

Provides textual, semantic, structural, or other similarity analysis for copyright and provenance assessment.

### Semantic Diff Plugin

Provides detailed comparison between specification versions, including changes in meaning and structure.

### SPDX License Plugin

Provides standardized license identification and compatibility analysis.

### Legal Review Plugin

Routes elevated copyright, patent, licensing, or attribution concerns to a qualified legal review process.

### Cryptographic Signing Plugin

Provides cryptographic signatures for specifications, provenance records, transformation events, and review decisions.

### Transparency Ledger Plugin

Provides an append only record of specification evolution events.

### Multi Agent Review Plugin

Allows multiple AI agents to independently analyze provenance, licensing, copyright, patent, or transformation concerns.

### Organization Policy Plugin

Applies organization specific rules for intellectual property thresholds, human approval, prohibited transformations, and deployment requirements.

## Plugin Requirements

Optional plugins must not silently modify provenance records or override core licensing requirements.

Plugins must identify:

- Plugin name.
- Plugin version.
- Provider or creator.
- Input sources.
- Analysis performed.
- Output produced.
- Timestamp.
- Relevant confidence information.

Plugin results must remain distinguishable from core SpecDNA records.

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
  - [https://roxanneardary.com/specdna/](https://roxanneardary.com/specdna/)  

---

## License & Notice Requirements

SpecDNA is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- SpecDNA specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
