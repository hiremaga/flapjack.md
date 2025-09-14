---
project: FlapJack
created: 2025-09-14
last_updated: 2025-09-14
current_iteration: MVP Bootstrap
team_capacity: 1 developer + 1 LLM
---

# FlapJack Project Plan

## Project Vision
Create a comprehensive markdown-based project management format that bridges the gap between traditional PM tools and developer-friendly workflows. FlapJack (Fluid, Layered Agile Planning for Just-right Agile Collaboration & Knowledge-tracking) should be maintainable by both humans and LLMs, fault-tolerant, and git-friendly.

---
iteration: MVP Bootstrap
focus: Get basic FlapJack format working by dogfooding it
---

### Started

---
type: FEATURE
title: Create minimal viable FlapJack format
points: 3
owner: Claude + Human
labels: #mvp, #core
---

As a project manager, I want a basic FlapJack format so that I can start tracking this project immediately.

**Acceptance Criteria:**
- [ ] PLAN.md uses FlapJack format
- [ ] Basic story syntax works with metadata blocks
- [ ] Simple iteration structure (Current + Backlog)
- [ ] Support for both inline and detailed story formats
- [ ] Wiki-links for cross-references

### Unstarted

---
type: CHORE
title: Create project README
points: 1
owner: Claude
labels: #docs, #setup
---

Clear README explaining FlapJack purpose and quick start instructions.

- CHORE: Make initial git commit #setup

## Backlog

---
iteration: Phase 1 - Core Specification
focus: Document the format we're using and make it type-safe
---

1. [[#Create formal specification document]]
2. CHORE: Set up validation/linting #tools, #quality
3. [[#Create minimal working examples]]

---
iteration: Phase 2 - Tool Integration
focus: Basic Obsidian compatibility and templates
---

1. [[#Add basic Obsidian support]]
2. CHORE: Create story templates #tools, #obsidian
3. CHORE: Basic CSS styling #tools, #obsidian

---
iteration: Phase 3 - Advanced Features
focus: Multi-file support and scalability
---

1. FEATURE(8pt): Multi-file format support #advanced, #scalability
2. FEATURE(3pt): Cross-file wiki-links #advanced, #obsidian
3. CHORE: Directory structure templates #advanced, #scalability

---
type: FEATURE
title: Create formal specification document
points: 5
labels: #spec, #core
---

As a developer/LLM, I want a formal specification so that I can validate FlapJack format and build tools around it.

---
type: FEATURE
title: Create minimal working examples
points: 3
labels: #examples, #docs
---

As a new user, I want clear examples so that I can understand how to use FlapJack for my projects.

---
type: FEATURE
title: Add basic Obsidian support
points: 2
labels: #tools, #obsidian
---

As an Obsidian user, I want FlapJack to work seamlessly with wiki-links and graph view.

## Definition of Done
- [ ] Code/format changes work as specified
- [ ] Documentation is updated
- [ ] Changes are committed to git
- [ ] Format remains human and LLM readable
- [ ] No breaking changes to existing valid FlapJack files

## Story Point Guidelines
- **1pt:** Simple task, < 1 hour
- **2pt:** Straightforward feature, few hours
- **3pt:** Moderate complexity, half day
- **5pt:** Complex feature, full day
- **8pt:** Large feature, multiple days