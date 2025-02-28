---
status: "active"  # Options: active, planning, completed, archived
created: 2025-02-28
tags: [personal, neovim, ide,project]
---
## Remaining Task
```tasks
(folder regex matches /01.Projects/NeovimConfiguration/i) AND \
(path regex does not match /NeovimConfiguration/NeovimConfiguration\.md/i)
not done
group by filename
```

## Overview
**Description:**  
    Latest Neovim configuration. This will not follow the development style of LazyVim.
    Instead it will follow this [repo]([dotfiles/nvim-fredrik/lua/fredrik/plugins/lang/lua.lua at main · fredrikaverpil/dotfiles](https://github.com/fredrikaverpil/dotfiles/blob/main/nvim-fredrik/lua/fredrik/plugins/lang/lua.lua))
**Objectives:**  
  - Per programming language LSP support
      - Install via UI similar to `LazyVim` Extras
  - Utilize `NvChad` libraries for nice UI
  - Lazy load all plugins where possible

## Setup & Installation
**Requirements:**  
  - Latest stable `neovim` or nightlight
  - Command line utilities
      - `fd`, `ripgrep`, `gcc (or some other c compiler)`, `lazygit`
**Installation Steps:**  
- TODO

## Configuration Layout
**Key Components:**  
  - Global Utils Class (like LazyVim's `LazyVim` global variable)
  - Root Configuration
      - Contains setup, utilities, and option setup that doesn't rely on plugins
  - LSP Configuration
      - Contains all plugins, utilities, and option setup for LSP. Some options set in Root Configuration will be overwritten here
  - User Interface Configuration
      - Contains all plugin, utilities, and option setup for UI/UX related items. Some options set in Root Configuration will be overwritten here
  - Coding Configuration
      - Contains all plugin, utilities, and option setup for coding related plugins. Some options set in Root Configuration will be overwritten here

## Development Tasks
**Backlog:**  
  - [[Core]]
  - [[LSP]]
  - [[UX]]
  - [[Coding]]

**Milestones:**  
  **Milestone 1:** Root Configuration & 2025-03-31

## Issues & Challenges

---