---
<%*
let title = await tp.system.prompt("Project Name")
let given_tags = await tp.system.prompt("Tags (personal, web)")
let tags = given_tags.split(",")
tp.file.title = await tp.file.rename(title)
tp.file.tags = tags.includes('project') ? tags : [...tags, 'project']

_%>

status: "active"  # Options: active, planning, completed, archived
created: {{date:YYYY-MM-DD}}
tags: [<% tp.file.tags %>]
---

## Overview
**Description:**  
Provide a concise description of the project.
**Objectives:**  
  - Objective 1
  - Objective 2

## Setup & Installation
**Requirements:**  
  - Dependency 1
  - Dependency 2
**Installation Steps:**  
  1. Step 1: Brief instruction
  2. Step 2: Brief instruction
**Configuration:**  
Note any configuration details here.

## Architecture & Design
**Tech Stack:**  
  - Language/Framework 1
  - Language/Framework 2
**Architecture Diagram:**  
![Diagram]()
**Key Components:**  
  - Component A: Description
  - Component B: Description

## Development Tasks
**Backlog:**  
  - [ ] Task 1 – Brief description
  - [ ] Task 2 – Brief description
**Milestones:**  
  **Milestone 1:** Description & target date
  **Milestone 2:** Description & target date

## Code & Resources
**Repository:**  
[Link to repository](https://github.com/your-repo)
**Documentation:**  
[Link to project docs](#)
**Useful Resources:**  
  - Resource 1
  - Resource 2

## Testing & Deployment
**Testing Strategy:**  
Outline your testing approach, frameworks, or tools.
**Deployment Plan:**  
Describe your deployment workflow and environment.

## Meetings & Updates
**Meeting Notes:**  
Reference or link to meeting notes (e.g., `[[Meeting Notes]]`).
**Project Updates:**  
  - *YYYY-MM-DD:* Brief update or progress summary

## Issues & Challenges
- List current issues, roadblocks, or challenges.
- Note potential solutions or areas for further investigation.

## Future Enhancements
- Ideas for improvements or new features to consider later.

---

*Created on {{date:YYYY-MM-DD}}*