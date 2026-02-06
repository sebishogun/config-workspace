# Config Workspace

Umbrella repo for quickly navigating all editor configuration repos.

## Included Submodules

- `LazyVim-Config`
- `99`
- `IdeaVim-Config`
- `VSCode-Config`
- `Zed-Config`

## Usage

- Update all submodules:
  - `git submodule update --init --recursive`
- Pull latest for all configs:
  - `git submodule foreach 'git pull --ff-only'`

## Notes

- Active Neovim runtime config is still in `~/.config/nvim`.
- This workspace is for navigation and centralized management.
