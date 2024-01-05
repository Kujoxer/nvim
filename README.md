# Nvim Config
## Steps:
### После того как 

```bash
cd ~/.config;
git clone git@github.com:Kujoxer/nvim.git;
```
### Сделать

```bash
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
```
### Затем
В nvim редакторе набрать `:PackerInstall`.

> В результате должно получиться:
- Никаких ошибок нету;
- Манеджер плагинов Packer - исправно работает;
- У нас первоначальная простая структура nvim конфигурации.

## Plugins install
### Telescope 

https://github.com/nvim-telescope/telescope.nvim

```lua
use {
  'nvim-telescope/telescope.nvim', tag = '0.1.5',
-- or                            , branch = '0.1.x',
  requires = { {'nvim-lua/plenary.nvim'} }
}
```

### Цветовая схема rose-pine

https://github.com/rose-pine/neovim

```lua
use({ 
  'rose-pine/neovim', as = 'rose-pine',
  config = function()
    vim.cmd('colorscheme rose-pine')
    end
  })
```
### Nvim-Treesitter для раскраски кода

```lua
use('nvim-treesitter/nvim-treesitter', {run = ':TSUpdate'})
use("nvim-treesitter/playground")
```

### Harpoon

https://github.com/ThePrimeagen/harpoon/tree/harpoon2

```lua
use {
    "ThePrimeagen/harpoon",
    branch = "harpoon2",
    requires = { {"nvim-lua/plenary.nvim"} }
}
```

### Дерево изменений 

https://github.com/mbbill/undotree?tab=readme-ov-file#download-and-install

```lua
use("mbbill/undotree")
```

### Плагин для Git

https://github.com/tpope/vim-fugitive

```lua
use("tpope/vim-fugitive")
```

### Lsp

```lua

```


## Source:
### По мотивам thePrimeagen
- https://youtu.be/w7i4amO_zaE?si=NT4aaByC_C-_-p0k

### Установка менеджера плагинов
- https://github.com/wbthomason/packer.nvim 

> Packer
- https://github.com/lewis6991/pckr.nvim



