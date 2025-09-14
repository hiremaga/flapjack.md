# FlapJack Plan

## Vision
Create a comprehensive markdown-based project management format that bridges the gap between traditional PM tools and developer-friendly workflows. FlapJack (Fluid, Layered Agile Planning for Just-right Agile Collaboration & Knowledge-tracking) should be maintainable by both humans and LLMs, fault-tolerant, and git-friendly.

## Team
- @Claude
- @hiremaga

## Iteration 0 – Bootstrap

### Finished
1. Make initial git commit @Claude @hiremaga #medium
2. [[#Create minimal viable FlapJack format]]

### Started
1. [[#Create formal specification document]]

### Unstarted
1. [[#Create project README]]

## Iteration 1 - Core Specification & Validation
1. Set up validation/linting #small
2. [[#Create minimal working examples]]

## Iteration 2 - Tool Integration
1. [[#Add basic Obsidian support]]
2. Create story templates #xsmall
3. Basic CSS styling #small

## Iteration 3 - Advanced Features
1. Multi-file format support #xxlarge
2. Cross-file wiki-links #medium
3. Directory structure templates #small

## Iteration 4 - Documentation & Guides
1. Getting started guide
2. Migration guide between formats
3. Tool setup guides

## Stories

### Create minimal viable FlapJack format
@Claude @hiremaga #medium

As a project manager, I want a basic FlapJack format so that I can start tracking this project immediately.

- [x] PLAN.md uses FlapJack format
- [x] Basic story syntax works with metadata blocks
- [x] Simple iteration structure (Current + Backlog)
- [x] Support for both inline and detailed story formats
- [x] Wiki-links for cross-references

### Create formal specification document
#small

As a developer/LLM, I want a formal specification so that I can validate FlapJack format and build tools around it.

### Create project README
@Claude

Clear README explaining FlapJack purpose and quick start instructions.

### Create minimal working examples

As a new user, I want clear examples so that I can understand how to use FlapJack for my projects. #medium

### Add basic Obsidian support

As an Obsidian user, I want FlapJack to work seamlessly with wiki-links and graph view. #small

- [ ] Code/format changes work as specified
- [ ] Documentation is updated
- [ ] Changes are committed to git
- [ ] Format remains human and LLM readable
- [ ] No breaking changes to existing valid FlapJack files

## Guidelines

### Sizing
- #xsmall: Quick task, few minutes, definitely under an hour
- #small: Straightforward feature, few hours
- #medium: Moderate complexity, upto a day
- #large: Complex feature, 2-3 days
- #xlarge: Large feature, ~1 week
- #xxlarge: Very large feature, multiple weeks
