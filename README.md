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

## New Machine Bootstrap

```bash
mkdir -p ~/neovim-configs
cd ~/neovim-configs
git clone https://github.com/sebishogun/config-workspace.git config-workspace
cd config-workspace
git submodule update --init --recursive
cd LazyVim-Config
./install.sh --dry-run
./install.sh
```

After install, verify in Neovim:

```vim
:NNStatus
:lua require("99").doctor()
:NNProvider <Tab>
:NNModel <Tab>
```

## Notes

- Active Neovim runtime config is still in `~/.config/nvim`.
- This workspace is for navigation and centralized management.
