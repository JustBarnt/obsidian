---
status: "active"  # Options: active, planning, completed, archived
created: 2025-02-28
tags: [personal, neovim, ide,project]
---

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
- [ ] TODO

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
  - [ ] Root Configuration
      - [ ] Global Utils Variable
          - [ ] `Core` utilities class
      - [ ] `vim.g` variable setup
      - [ ] Keymap & Option setup
      - [ ] Root Utilities
          - [ ] TODO
      - [ ] `lazy.nvim` bootstrap
      - [ ] `health` check
  - [ ] LSP Configuration
      - [ ] Keymap & Option overrides
      - [ ] LSP Utilities (gets added to global Utils class)
          - [ ] `LSP` utilities class
      - [ ] `lspconfig`, `mason`, `conform`, `mason-lspconfg` setup with `lua_ls` as the single LSP bundled
      - [ ] `health.lsp` check to ensure things like `node.js`, `python`, `php`, `dotnet`, et
**Milestones:**  
  **Milestone 1:** Description & target date
  **Milestone 2:** Description & target date

## Issues & Challenges
- List current issues, roadblocks, or challenges.
- Note potential solutions or areas for further investigation.

## Future Enhancements
- Ideas for improvements or new features to consider later.

---