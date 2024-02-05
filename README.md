# NVIM

A custom configuration for neovim, based on [NvChad](https://nvchat.com) and [LazyVim](https://lazyvim.org)
I tried to bring the best of both, with some of my own preferences.

Note: This is a work in progress, and I'm still learning a lot about neovim and lua. I wouldn't advise anyone to use this config on a critical system.



## Getting started

```sh
$ git clone https://github.com/tomosovich/nvim.git ~/.config/nvim
$ cd ~/.config/nvim
$ git remote add nvchad https://github.com/NvChad/NvChad.git
$ nvim
```
### Target Projects
I primarily work with the following projects:
* next.js (typescript)
* react
* node.js
* go
* rust (My newest interest)


### Vue projects

Create a file `.volar` in the root of your project to enable volar and volar "Take over mode"

## Troubleshooting

- If any issues with layout or the UI, clear your cache
-

## Changes made to nvchad core

- `init.lua`
  - import `custom/keymaps.lua`
  - prevent loading of cached defaults highlight groups
- `lua/core/init.lua`
  - fix ReloadNvChad autocmd to correctly reload modules
- `lua/plugins/configs/cmp.lua`
  - prevent loading of cached cmp highlight groups

## Requirements

Any requirement from [Mason](https://github.com/williamboman/mason.nvim#requirements), Mason will install [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig), [conform.nvim](https://github.com/stevearc/conform.nvim), [nvim-lint](https://github.com/mfussenegger/nvim-lint) and [nvim-dap](https://github.com/mfussenegger/nvim-dap) dependencies

- [neovim >= 0.9.4](https://github.com/neovim/neovim)
- [neovim-remote](https://github.com/mhinz/neovim-remote)
- [kitty](https://sw.kovidgoyal.net/kitty) (recommended)
- [tree-sitter](https://github.com/tree-sitter/tree-sitter)
- [ripgrep](https://github.com/BurntSushi/ripgrep) (required by [telescope](https://github.com/nvim-telescope/telescope.nvim)
  )
- [fd](https://github.com/sharkdp/fd) (required by [telescope](https://github.com/nvim-telescope/telescope.nvim))
- [deno](https://github.com/denoland/deno) (required by [peek](https://github.com/toppair/peek.nvim))
- [nixfmt](https://github.com/serokell/nixfmt) (required by [conform.nvim](https://github.com/stevearc/conform.nvim))
- [statix](https://github.com/nerdypepper/statix) (required by [nvim-lint](https://github.com/mfussenegger/nvim-lint))
- [ts-node](https://www.npmjs.com/package/ts-node) (required by [nvim-dap](https://github.com/mfussenegger/nvim-dap))
- [typescript](https://www.npmjs.com/package/typescript) (required by [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig))
- [@styled/typescript-styled-plugin](https://www.npmjs.com/package/@styled/typescript-styled-plugin) (required by [typescript-tools.nvim](https://github.com/pmizio/typescript-tools.nvim#-styled-components-support))
