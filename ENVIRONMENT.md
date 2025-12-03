# Development Environment Setup

This document tracks the reproducible setup of the development environment.

## Package Managers

- **Homebrew** - macOS package manager
- **mise** - Polyglot runtime manager (replaces asdf)
- **pnpm** - Fast, disk space efficient package manager
- **cargo** - Rust package manager
- **pipx** - Install Python applications in isolated environments

## Homebrew Packages

### Taps
```bash
brew tap chiselstrike/tap
brew tap derailed/k9s
brew tap dopplerhq/cli
brew tap edgedb/tap
brew tap hashicorp/tap
brew tap homebrew/bundle
brew tap jesseduffield/lazygit
brew tap libsql/sqld
brew tap pulumi/tap
brew tap supabase/tap
```

### CLI Tools & Utilities
```bash
# System utilities
brew install tree
brew install wget
brew install pv
brew install xz

# Monitoring & System Info
brew install bottom
brew install btop
brew install htop
brew install neofetch

# Shell & Terminal
brew install fzf
brew install tmux
brew install atuin

# Search & Navigation
brew install gping
brew install lazygit

# Network Tools
brew install nmap
brew install aircrack-ng

# Version Control
brew install git
brew install git-lfs
brew install git-filter-repo
brew install gh
```

### Development Tools
```bash
# Build Tools
brew install autoconf
brew install cmake
brew install gcc
brew install pkgconf

# Language-specific tools
brew install fnm
brew install rustup
brew install go
brew install gleam
brew install erlang
brew install elixir

# Cloud & Infrastructure
brew install awscli
brew install flyctl
brew install kubernetes-cli
brew install helm
brew install kind
brew install kompose
brew install derailed/k9s/k9s
brew install hashicorp/tap/terraform
brew install pulumi/tap/pulumi

# Databases & Data
brew install libpq
brew install edgedb/tap/gel-cli
brew install chiselstrike/tap/turso
brew install supabase/tap/supabase

# DevOps & Deployment
brew install ansible
brew install dopplerhq/cli/doppler
brew install podman

# Package Management
brew install mise
brew install chezmoi
brew install pipx
```

### Media & Processing
```bash
brew install ffmpeg
brew install imagemagick
brew install mpv
brew install yt-dlp
brew install vips
brew install tesseract
brew install ghostscript
brew install poppler
```

### Libraries
```bash
brew install libtiff
brew install little-cms2
brew install webp
brew install jpeg-xl
brew install aom
brew install libarchive
brew install openjpeg
brew install leptonica
brew install hdf5
brew install icu4c@75
brew install libheif
brew install libmatio
brew install librsvg
brew install clblas
brew install clblast
brew install openblas
brew install openslide
brew install qt@5
brew install vapoursynth
brew install gdk-pixbuf
```

### AI & LLMs
```bash
brew install ollama
brew install gemini-cli
```

### Other Tools
```bash
brew install jq
brew install gnupg
brew install synergy-core
brew install tlrc
brew install rclone
brew install rtorrent
brew install exercism
brew install node
```

## Homebrew Casks (Applications)

### Terminal Emulators
```bash
brew install --cask alacritty
brew install --cask ghostty
brew install --cask hyper
brew install --cask iterm2
brew install --cask kitty
brew install --cask warp
```

### Browsers
```bash
brew install --cask floorp
brew install --cask google-chrome
```

### IDEs & Editors
```bash
brew install --cask cursor
brew install --cask sublime-text
brew install --cask vscodium
brew install --cask windsurf
brew install --cask jetbrains-toolbox
brew install --cask thonny
```

### AI Tools
```bash
brew install --cask jan
brew install --cask lm-studio
brew install --cask msty
```

### Productivity
```bash
brew install --cask alfred
brew install --cask anytype
brew install --cask bartender
brew install --cask dash
brew install --cask joplin
brew install --cask logseq
brew install --cask notion
brew install --cask obsidian
brew install --cask raycast
brew install --cask rectangle
brew install --cask roam-research
brew install --cask scrivener
```

### Development Tools
```bash
brew install --cask docker-desktop
brew install --cask github
brew install --cask openlens
brew install --cask podman-desktop
brew install --cask godot
```

### Communication
```bash
brew install --cask discord
brew install --cask microsoft-teams
brew install --cask chatterino
brew install --cask thunderbird
brew install --cask proton-mail-bridge
```

### Media & Creative
```bash
brew install --cask blender
brew install --cask obs
brew install --cask spotify
brew install --cask vlc
brew install --cask distroav
brew install --cask libndi
brew install --cask reflector
```

### Utilities
```bash
brew install --cask authy
brew install --cask calibre
brew install --cask dropbox
brew install --cask kindle
brew install --cask linearmouse
brew install --cask parallels
brew install --cask protonvpn
brew install --cask qbittorrent
brew install --cask stats
brew install --cask steam
brew install --cask syncthing-app
brew install --cask utm
brew install --cask wireshark-app
```

### Fonts
```bash
brew install --cask font-fira-code
brew install --cask font-fira-code-nerd-font
brew install --cask font-fira-mono
brew install --cask font-fira-mono-for-powerline
brew install --cask font-fira-mono-nerd-font
brew install --cask font-fira-sans
brew install --cask font-fira-sans-condensed
brew install --cask font-jetbrains-mono
brew install --cask font-source-code-pro
brew install --cask font-source-code-pro-for-powerline
```

## mise (Runtime Manager)

mise is configured globally via `~/.config/mise/config.toml` with the following runtimes:

```bash
mise use -g bun@latest
mise use -g deno@latest
mise use -g elixir@latest
mise use -g erlang@latest
mise use -g gleam@latest
mise use -g go@latest
mise use -g jq@latest
mise use -g node@latest
mise use -g ocaml@latest
mise use -g pnpm@latest
mise use -g python@3.12
mise use -g rebar@latest
mise use -g ruby@latest
mise use -g rust@latest
mise use -g zig@latest
```

Current versions installed:
- bun: 1.2.21
- deno: 2.4.5
- elixir: 1.18.4-otp-28
- erlang: 28.0.2
- gleam: 1.12.0
- go: 1.25.0
- jq: 1.8.1
- node: 24.7.0
- ocaml: 5.3.0
- pnpm: 10.15.0
- python: 3.12.11
- rebar: 3.25.1
- ruby: 3.4.5
- rust: 1.89.0
- zig: 0.15.1

## Cargo (Rust) Packages

```bash
cargo install cargo-expand
cargo install cargo-watch
cargo install rustlings
cargo install tauri-cli
```

## pnpm Global Packages

```bash
pnpm install -g tdd-guard@latest
pnpm install -g vercel
```

## npm Global Packages

```bash
npm install -g @anthropic-ai/claude-code
npm install -g @musistudio/claude-code-router
npm install -g @sveltejs/mcp
npm install -g @wallabyjs/cli
npm install -g mcp-server-apple-reminders
```

## Shell Setup (zsh)

### Oh My Zsh
```bash
# Install Oh My Zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Install Powerlevel10k theme
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

# Install plugins
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

### Plugins enabled in .zshrc
- git
- fnm
- zsh-autosuggestions
- zsh-syntax-highlighting

### Additional Shell Tools
- **atuin** - Shell history with sync capabilities
- **fzf** - Fuzzy finder
- **mise** - Runtime version manager

## Python Environment

### Anaconda/Conda
Anaconda3 is installed at `/Users/seth/anaconda3`

Initialized in `.zshrc` via conda init

## Additional Setup Scripts

### Script-based installations found in history:
```bash
# Ash HQ Phoenix installation
sh <(curl 'https://ash-hq.org/install/blockchain_coffee?install=phoenix')
```

## VS Code Extensions

See Brewfile output for complete list of VS Code extensions. Key extensions include:
- GitHub Copilot suite
- Language support: Go, Rust, Python, Elixir, Deno, Svelte
- Docker & Kubernetes tools
- Remote development tools
- GitLens
- Prettier, ESLint
- Material themes and icons
- And many more...

## Recent Manual Installations

Recent tools installed via package managers (from shell history):
```bash
brew install chezmoi
brew install gemini-cli
brew install ghostty
brew install git-filter-repo
brew install jan
brew install node pnpm
brew install windsurf
brew install xz
```

## Notes

- This environment uses `chezmoi` for dotfiles management
- Shell history is tracked with `atuin` with cloud sync disabled for up-arrow
- Terminal emulator options: Ghostty, Warp, Kitty, iTerm2, Alacritty
- Multiple AI/LLM tools installed: Ollama, LM Studio, Jan, Msty, Gemini CLI
- Multiple IDE options: Cursor, Windsurf, VSCodium, JetBrains Toolbox

## Restoration Commands

To restore this environment on a new machine:

1. Install Homebrew
2. Clone this chezmoi repo
3. Run `brew bundle` (if Brewfile exists)
4. Install mise and configure global tools
5. Apply chezmoi: `chezmoi init && chezmoi apply`
6. Install Oh My Zsh and plugins
7. Configure shell integrations (atuin, fzf, mise)
