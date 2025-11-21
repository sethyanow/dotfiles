This file provides guidance to agents when working with code in this repository.

## Project Overview

This is a **dotfiles repository** managed by [chezmoi](https://chezmoi.io), a dotfile manager for version-controlling and deploying user configuration files. The repository contains configuration and scripts for the user's development environment.

**Key Guidelines:**
- This is a dotfiles repository, not a software project
- Do not write code or make changes unprompted
- Always ask before making modifications if you're unsure about what's needed

## Chezmoi Deployment Model

- **Source directory:** `home/`
- **Target directory:** User's home (`~/`)
- **File naming convention:** Files prefixed with `dot_` are deployed as dotfiles (e.g., `dot_zshrc` → `~/.zshrc`)

### Deploying dotfiles
```bash
chezmoi apply           # Deploy all dotfiles to home directory
chezmoi diff            # Preview what would be deployed
chezmoi edit dot_zshrc  # Edit zshrc with chezmoi (manages the dotfile)
```

### Viewing current state
```bash
chezmoi status          # Show status of tracked dotfiles
chezmoi managed         # List all managed files
```

### Adding new dotfiles
```bash
chezmoi add ~/.some_config_file    # Start managing a file
# Edit in home/ directory with dot_ prefix
chezmoi apply                       # Deploy changes
```