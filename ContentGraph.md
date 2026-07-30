# ContentGraph

**ContentGraph** is a WordPress-native relational content layer that transforms pages, posts, and documentation into a structured, graph-based system. It introduces Spec Containers as modular documentation units and enables Git-like navigation, while keeping WordPress as the source of truth for URLs, indexing, and content ownership.

## Overview

ContentGraph extends WordPress with a relational architecture layer over content. Instead of treating pages and posts as isolated documents, ContentGraph connects them through structured relationships, navigation graphs, and optional Spec Containers that behave like repository-style documentation units.

The system is designed to work entirely within standard WordPress hosting environments without requiring external infrastructure.

---

## Modular Design

ContentGraph is built as a modular WordPress extension where core functionality provides the foundation for relational content management, while optional plug-in modules extend capabilities without changing the underlying architecture.

The modular design allows users to deploy only the features they need while keeping WordPress as the source of truth for content, relationships, and documentation.

---

## Core Modules

### Spec Container Engine

The Spec Container Engine provides the foundation of ContentGraph.

Features:
- Creates and manages Spec Containers as structured documentation units
- Provides repository-style organization within WordPress
- Supports hierarchical file and folder structures
- Stores Markdown-based documentation nodes
- Maintains relationships between container elements
- Enables modular software specifications and knowledge systems

---

### Content Relationship Engine

The Content Relationship Engine creates the relational layer over WordPress content.

Features:
- Connects pages, posts, and Spec Containers
- Creates structured relationships between content objects
- Supports cross-linking between documentation systems
- Enables graph-based content organization
- Maintains content relationships independently from presentation layers

---

### Navigation Engine

The Navigation Engine provides automatic Git-style navigation for Spec Containers.

Features:
- Generates dynamic file-tree navigation
- Supports nested folders and document paths
- Provides breadcrumb navigation
- Tracks active document locations
- Creates repository-style browsing experiences

---

### Markdown Rendering Engine

The Markdown Rendering Engine manages documentation display.

Features:
- Native Markdown support
- Rendered documentation view
- Raw Markdown repository view
- Code-focused formatting
- Documentation-friendly layouts
- Extensible rendering pipeline

---

### WordPress Integration Module

The WordPress Integration Module connects ContentGraph with standard WordPress workflows.

Features:
- Native WordPress administration integration
- Add Spec Container workflow
- Page and post embedding support
- Gutenberg block support
- Shortcode support
- WordPress permission compatibility

---

### Theme Compatibility Module

The Theme Compatibility Module ensures Spec Containers integrate with existing WordPress designs.

Features:
- Inherits active WordPress theme styling
- Supports page-level style inheritance
- Provides scoped CSS handling
- Prevents global theme conflicts
- Allows custom container styling

---

### Search and Indexing Module

The Search and Indexing Module enables discovery across structured content.

Features:
- WordPress search compatibility
- Spec Container content indexing
- Container-level search
- Document path discovery
- Search filtering controls

---

## Optional Plug-In Modules

### Git Mirror Module

Provides optional synchronization with external Git platforms.

Features:
- Export Spec Containers as repository structures
- Import supported Git documentation formats
- Maintain external mirrors
- Support developer-selected hosting platforms
- Keep local WordPress installation as the canonical source

---

### Version Control Module

Adds revision and change tracking capabilities.

Features:
- Document revision history
- Change comparison
- Version tagging
- Release tracking
- Specification lifecycle management

---

### API Integration Module

Extends ContentGraph through external integrations.

Features:
- REST API access
- External application connections
- Automated content synchronization
- Third-party workflow integrations

---

### Advanced Graph Visualization Module

Provides visual representations of content relationships.

Features:
- Interactive content graphs
- Relationship mapping
- Dependency visualization
- Knowledge network exploration

---

### Collaboration Module

Adds team-based documentation workflows.

Features:
- Contributor permissions
- Review workflows
- Approval processes
- Documentation ownership tracking

---

### Export and Archive Module

Provides long-term portability options.

Features:
- Export Spec Containers
- Generate documentation packages
- Create offline archives
- Preserve structured content outside WordPress

---

### AI Assistance Module

Provides optional AI-powered documentation capabilities.

Features:
- Documentation generation assistance
- Content relationship suggestions
- Specification analysis
- Search enhancement
- Knowledge discovery support

---

## System Design Principles

- WordPress is the source of truth
- Spec Containers are optional structured overlays
- Navigation is scoped to containers, not global UI
- No forced layout injection into themes
- User controls embedding and placement
- Content is relational, not flat

---

## Use Cases

- Technical documentation systems
- API specification hosting
- Internal knowledge graphs
- Software architecture documentation
- Modular product specification systems
- Wiki-style structured content inside WordPress

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
  - [https://roxanneardary.com/contentgraph/](https://roxanneardary.com/contentgraph/)

---

## License & Notice Requirements

ContentGraph is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- ContentGraph specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
