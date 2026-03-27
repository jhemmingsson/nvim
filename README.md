# Neovim Configuration

Personal Neovim configuration managed with [Packer](https://github.com/wbthomason/packer.nvim).

## Plugins

- **LSP** - [lsp-zero.nvim](https://github.com/VonHeikemen/lsp-zero.nvim) (v3.x) with Mason, nvim-cmp
- **Treesitter** - Syntax highlighting and code analysis
- **Telescope** - Fuzzy finder for files, grep, and more
- **nvim-tree** - File explorer
- **onedark** - Color scheme
- **lualine** - Status line
- **trouble.nvim** - Diagnostics list
- **todo-comments** - Highlight and search TODO/FIXME comments
- **ssr.nvim** - Structural search and replace
- **claudecode.nvim** - Claude Code integration

## Key Mappings

Leader key: `<Space>`

| Key | Mode | Action |
|-----|------|--------|
| `<leader>ff` | Normal | Find files |
| `<C-p>` | Normal | Git files |
| `<leader>ps` | Normal | Grep string |
| `<leader>lg` | Normal | Live grep |
| `<leader>t` | Normal | Toggle file tree |
| `<leader>pv` | Normal | Open netrw |
| `<leader>y` | Normal/Visual | Yank to system clipboard |
| `<leader>w` | Normal | Switch window |
| `<leader>h/j/k/l` | Normal | Navigate windows |
| `<leader>cc` | Normal | Toggle Claude Code |
| `<leader>cs` | Visual | Send selection to Claude Code |
| `J/K` | Visual | Move selected lines |

## Structure

```
init.lua                    # Entry point, loads lua/voi/
lua/voi/
  init.lua                  # Module loader
  packer.lua                # Plugin definitions
  remap.lua                 # Key mappings
  set.lua                   # Vim options
after/plugin/               # Plugin-specific configuration
```
