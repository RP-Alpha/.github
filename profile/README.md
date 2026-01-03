# RP-Alpha

**RP-Alpha** is a modern development collective dedicated to engineering high-quality, open-source resources for the FiveM roleplay community. We bridge the gap between complex functionality and ease of use, ensuring compatibility across major frameworks (QB-Core, QBOX, OX_CORE).

### Mission Statement
To empower server owners and developers with robust, modern, and accessible tools that elevate the standard of FiveM roleplay cities.

### Core Values
1.  **Open Source First**: Transparency, collaboration, and knowledge sharing.
2.  **Modern Standards**: Utilizing contemporary Lua/JS practices and performance optimization.
3.  **Simplicity & Flexibility**: Plug-and-play resources with deep customization.
4.  **Community Driven**: Building *with* the community, not just for them.

---

## Organizational Structure

### Core Team Roles
The organization operates with a flat hierarchy that emphasizes responsibility over rank.

#### **Project Lead(s)**
*   **Responsibilities**: Strategic vision, high-level roadmap planning, final decision on architectural standards, conflict resolution.
*   **Focus**: Maintaining the "RP-Alpha Mindset" and ensuring project cohesion.

#### **Core Developers**
*   **Responsibilities**: Implementation of core resources, code review, maintaining framework compatibility layers, security auditing.
*   **Focus**: Writing clean, performant, and secure code (Lua/JS/SQL).

#### **Documentation & Support Specialists**
*   **Responsibilities**: Maintaining READMEs, creating Wikis, managing community support channels (Discord/GitHub), writing tutorials.
*   **Focus**: Reducing the barrier to entry for end-users.

#### **Community Managers**
*   **Responsibilities**: Gathering feedback, managing release announcements, fostering the developer ecosystem.
*   **Focus**: Bridge between the user base and the dev team.

---

## Operational Workflow

### Development Lifecycle
We follow a strict **Plan -> Develop -> Test -> Document -> Release** cycle.

1.  **Ideation & RFCs (Request for Comments)**
    *   New features or resources start as an Issue or RFC in GitHub.
    *   Must define: Problem to solve, Framework impact, Config needs.

2.  **Development Standards**
    *   **Naming**: Resources prefixed with `rpa-` (e.g., `rpa-banking`).
    *   **Code**: Adherence to the RP-Alpha Style Guide (CamelCase, specific event naming conventions).
    *   **Compatibility**: All core logic must be abstracted to support QB/QBOX/OX via a unified bridge.

3.  **Quality Assurance (QA)**
    *   **Automated**: Linting (LuaCheck) and rigid syntax verification.
    *   **Manual**: Tested on "Clean" server instances of **QB-Core** and **QBOX**. We do not perform direct manual testing on OX_CORE, though we maintain code-level compatibility where possible.
    *   **Performance**: 0.00ms idle requirement for client scripts; optimized database queries (batching).

4.  **Release Protocol**
    *   Semantic Versioning (1.0.0).
    *   Changelog generation.
    *   Release tags on GitHub.

### Repository Management
*   **GitHub Organization**: All repositories are hosted under the **RP-Alpha** GitHub Organization.
*   **Monorepo vs Polyrepo**: We utilize individual repositories for major resources to allow modular adoption, with a central "manifest" or "pack" repo for full-suite users.
*   **Branching**: `main` is stable. Feature branches (`feat/xyz`) for development.

---

## Product Strategy & Roadmap

### Phase 1: Core Essentials & UI
*   **Goal**: Establish the base infrastructure and visual language.
*   **Deliverables**:
    *   `rpa-lib`: Shared bridge for Frameworks, Notify, TextUI, and target systems.
    *   `rpa-notify` / `rpa-textui`: Standalone options (with support for external resources like Brutal/RTX).
    *   `rpa-blips`: Centralized blip management configuration.
    *   `rpa-spawn` & `rpa-appearance`: Modern entry-points for players.

### Phase 2: Economy & Assets
*   **Goal**: Robustness for the server's financial and asset backbone.
*   **Deliverables**:
    *   `rpa-fuel`: Legacy and target-based fueling systems.
    *   `rpa-banking`: Clean UI banking, society management, and logs.
    *   `rpa-shops`: Unified system for Player-owned and AI-run shops.
    *   `rpa-consumables`: Food, drink, and item usability handler.
    *   `rpa-garages`: Vehicle storage and management.
    *   `rpa-housing`: Instanced and shell-based property systems.

### Phase 3: Gameplay Loop & Services
*   **Goal**: Specialized jobs and government systems.
*   **Deliverables**:
    *   `rpa-dispatch` & `rpa-mdt`: Integrated emergency services suite.
    *   `rpa-police` & `rpa-ambulance`: Full-featured service jobs including AI Medic options.
    *   `rpa-cityhall`: Licensing and government jobs.
    *   `rpa-trucking` & `rpa-jobs`: Generic and specialized civ jobs.

---

## Community & Contribution

### Contribution Model
*   **"Good First Issues"**: Tagged for new contributors to get involved.
*   **Pull Request Policy**:
    *   Must pass CI checks.
    *   Requires 1 Core Dev review.
    *   Must update relevant documentation.

### Support Channels
*   **GitHub Issues**: For bug reports and technical feature requests.
*   **Discord**: For general support, showcases, and community discussion.

---

## Technology Stack
*   **Backend**: Lua 5.4 (FiveM), NodeJS (where necessary for heavy IO).
*   **Frontend**: React/Vue/Svelte (built to static HTML/JS) or standard NUI.
*   **Data**: SQL (OxMySQL wrapper).
*   **UI Library**: Mantine or similar for consistent, modern aesthetics.
*   **Integrations**: Native compatibility with popular community tools (e.g., BrutalNotify, BrutalTextUI, rtx_notify, etc.) via `rpa-lib` bridges.
