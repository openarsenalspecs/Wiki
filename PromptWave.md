# PromptWave Specification

PromptWave is designed as a modular, open-source AI companion that teaches users how to create better images and videos through natural conversation. Rather than acting solely as a content generator, PromptWave functions as an interactive creative mentor, helping users understand prompt engineering while continuously refining their ideas through guided dialogue.

The platform is model-agnostic and supports both local and remote AI models through a flexible adapter architecture. Every major capability is implemented as an independent module, allowing deployments to remain lightweight while enabling organizations and developers to extend PromptWave with additional functionality through plugins.

PromptWave is designed around four guiding principles:

- Learn by creating.
- Keep humans in control.
- Support every major AI model through adapters.
- Extend functionality without modifying the core platform.

---

# Modular Design

PromptWave consists of a lightweight core platform and an extensible plugin ecosystem.

## Core Platform

The core platform provides the conversational engine, prompt coaching, workflow management, user experience, and extension framework.

### Core Modules

### Conversation Engine
- Natural language conversations
- Context-aware prompting
- Multi-turn dialogue
- Goal-oriented questioning
- Prompt refinement sessions
- Conversation history

### Prompt Intelligence
- Real-time prompt coaching
- Prompt debugger
- Prompt clarity scoring
- Contradiction detection
- Intent recognition
- Automatic prompt rewriting
- Educational prompt explanations
- Auto-refinement loops
- Experimental prompt generation
- Prompt comparison tools

### Prompt Composer
- Structured prompt building
- Modular prompt blocks
- Drag-and-drop prompt components
- Style templates
- Lighting presets
- Camera presets
- Motion templates
- Prompt version history

### Image Generation
- Image generation interface
- Side-by-side comparisons
- Sketch-to-image workflows
- Reference image analysis
- Emotional tone adjustments
- Style harmonization
- Aesthetic scoring
- Composition analysis

### Video Generation
- Storyboard generation
- Motion prompt creation
- Camera movement planning
- Scene sequencing
- Character consistency
- Frame continuity management
- Sketch-to-video workflows

### Workflow Manager
- Creative project management
- Generation timelines
- Branching prompt history
- Session management
- Undo/redo
- Saved workflows

### Collaboration
- Shared workspaces
- Live collaboration
- Prompt reviews
- Version management
- Team roles
- Shared libraries

### User Experience
- Beginner mode
- Advanced mode
- Guided tutorials
- Interactive coaching
- Accessibility features
- Voice interaction
- Multilingual support

### Prompt Library
- Prompt organization
- Automatic tagging
- Search
- Collections
- Favorites
- Prompt memory (optional user-controlled)

### Export Framework
- Export management
- JSON prompt export
- Storyboard export
- Production pipeline support
- Asset packaging

### Integration Framework
- Model adapters
- Local inference
- Cloud providers
- REST API
- CLI
- Python SDK
- JavaScript SDK
- Webhooks

### Plugin Framework
- Plugin discovery
- Plugin lifecycle management
- Extension APIs
- Module registration
- Permission management
- Configuration management

---

# Optional Plugin Modules

Deployments can enable only the capabilities they require.

### AI Model Connectors
- Stable Diffusion
- SDXL
- SD3
- FLUX
- ComfyUI
- OpenAI image models
- OpenAI video models
- Runway
- Pika
- Kling
- Future providers

### Creative Style Packs
- Photography
- Illustration
- Anime
- Watercolor
- Oil painting
- Comic
- Pixel art
- Architectural visualization
- Interior design
- Product photography

### Motion Libraries
- Cinematic camera moves
- Drone shots
- Tracking shots
- Character motion
- Animation templates
- Visual effects presets

### Storytelling Tools
- Story generators
- Scene planners
- Character development
- Dialogue planning
- Story arcs
- Narrative pacing

### Reference Analysis
- Color extraction
- Style fingerprinting
- Lighting analysis
- Lens estimation
- Perspective analysis
- Composition matching

### Collaboration Extensions
- Team management
- Organization workspaces
- Review workflows
- Creative approvals
- Asset sharing

### Learning Modules
- Prompt engineering courses
- Interactive tutorials
- Guided exercises
- Creative challenges
- Prompt explanations
- Skill assessments

### Accessibility Extensions
- Screen reader enhancements
- Voice coaching
- Alternative interfaces
- Simplified workspace modes

### Production Integrations
- Adobe Premiere Pro
- DaVinci Resolve
- Blender
- Unreal Engine
- Unity
- Creative asset management systems

### Cloud Storage Connectors
- Git repositories
- Object storage
- Self-hosted storage
- Cloud synchronization

### Analytics Extensions
- Prompt effectiveness
- Workflow analytics
- Generation statistics
- Learning progress
- Creative insights

### Enterprise Extensions
- Authentication providers
- Role-based access control
- Audit logging
- Policy enforcement
- Organization administration

### Marketplace
- Community plugins
- Prompt collections
- Workflow templates
- Style libraries
- Motion packs
- Educational content

---

# Design Goals

- Human-centered AI guidance
- Conversational learning instead of trial and error
- Privacy-first architecture
- Local-first deployment support
- Model independence
- Extensible plugin ecosystem
- Transparent prompt refinement
- Educational user experience
- Accessible to beginners while remaining powerful for professionals
- Community-driven open-source development

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
  - [https://roxanneardary.com/promptwave/](https://roxanneardary.com/promptwave/)


---

## License & Notice Requirements

PromptWave is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**. 
- PromptWave specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
