# FlapJack Format Specification v1.0

## Overview

FlapJack (Fluid, Layered Agile Planning for Just-right Agile Collaboration & Knowledge-tracking) is a markdown-based project management format designed to be:
- Human and LLM maintainable
- Git-friendly with clear diffs
- Fault-tolerant and flexible
- Compatible with existing markdown tools

## File Structure

A FlapJack file consists of the following sections in order:

1. **Project Header** (required)
2. **Team** (optional)
3. **Iterations** (required)
4. **Stories** (optional)
5. **Guidelines** (optional)

## Project Header

The project header consists of a level 1 heading followed by a vision section:

```
# Project Name Plan

## Vision
Project vision statement describing goals and purpose.
```

## Team Section

Lists project team members using @ mentions:

```
## Team
- @username1
- @username2
```

## Iterations

Iterations are the core organizational unit. Each iteration has a name and three status sections:

```
## Iteration 0 – Bootstrap

### Finished
1. Story title @assignee #size
2. Cross-reference to detailed story

### Started
1. Cross-reference to detailed story

### Unstarted
1. Story title @assignee #size
```

### Iteration Rules
- Iteration numbers start at 0 for bootstrap/setup
- Each iteration has exactly three subsections: Finished, Started, Unstarted
- Items can be inline stories or story references using double-bracket wiki-link syntax

## Stories

Stories can be defined in two formats:

### Inline Stories
Stories defined directly within iteration numbered lists with title, optional assignment, and optional size.

### Detailed Stories
Stories with full descriptions in a dedicated Stories section using level 3 headings. These stories can contain:
- Assignment and sizing metadata on separate lines
- User story format: "As a user type, I want goal so that benefit."
- Acceptance criteria using checkbox task lists

Example detailed story structure:
```
### Story Title
@assignee #size

As a project manager, I want clear examples so that I can understand the format.

- [ ] Acceptance criterion 1
- [ ] Acceptance criterion 2
```

## Metadata

### Assignments
- Format: @username
- Can appear after story titles or on dedicated lines in detailed stories
- Multiple assignments allowed: @dev1 @dev2

### Sizing
- Format: #size
- Standard sizes: #xsmall, #small, #medium, #large, #xlarge, #xxlarge
- Custom sizes allowed but should be defined in Guidelines section

### Cross-References
- Format: Double brackets around hash and story title
- Links to detailed stories in the Stories section
- Case-sensitive exact match to story headers
- Example: Reference to "Create formal specification document" story

## Task Lists

Within detailed stories, use standard markdown checkboxes:
- Empty checkbox for incomplete tasks
- Checked checkbox for complete tasks

## Guidelines Section

Optional section for project-specific rules such as sizing definitions, workflow conventions, or team agreements.

## Syntax Rules

1. **Headers**: Use standard markdown headers (single #, double ##, triple ###)
2. **Lists**: Use numbered lists for iterations, bullet lists for teams
3. **Whitespace**: Flexible - extra blank lines are ignored
4. **Case Sensitivity**: Story references are case-sensitive
5. **Order**: Sections can appear in any order after the project header

## Compatibility

- Standard markdown parsers can render FlapJack files
- Wiki-link syntax compatible with Obsidian and other tools
- Git diffs clearly show story status changes
- Fault-tolerant: malformed sections don't break the entire file

## Examples

### Minimal FlapJack File
```
# My Project Plan

## Iteration 0 – Setup

### Finished
1. Initial planning #small

### Started

### Unstarted
1. Reference to detailed "Create user login" story

## Stories

### Create user login
#medium

Basic user authentication system.
```

### Full FlapJack File
See PLAN.md in this repository for a complete example.