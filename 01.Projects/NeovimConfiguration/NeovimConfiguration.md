---
status: "active"  # Options: active, planning, completed, archived
created: 2025-02-28
tags: [personal, neovim, ide,project]
---
## Remaining Tasks
> [!check] Remaining Tasks
> ```tasks
path includes 01.Projects/NeovimConfiguration/
not done
>```

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
      - [ ] Includes: `lspconfig`, `mason`, `conform`, `mason-lspconfg` setup with `lua_ls` as the single LSP bundled
  - [ ] User Interface Configuration
      - [ ] Keymap & Option overrides
      - [ ] UI/UX Utilities (gets added to global Utils class)
          - [ ] `UI` utilities class.
              - [ ] Includes: toggles (LazyVim toggles) and maybe more
      - [ ] Includes: `snacks.nvim`, `noice.nvim`, `nvchad`, etc.
  - [ ] Coding Configuration
      - [ ] Keymap & Option overrides
      - [ ] Coding Utilities (gets added to global Utils class)
          - [ ] `CODING` utilities class
              - [ ] Includes: fold management, auto-formatting, treesitter text-objects,  and more

**Milestones:**  
  **Milestone 1:** Root Configuration & 2025-03-31

## Issues & Challenges

---