# nvim-config

Ma configuration Neovim basée sur [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim), adaptée pour l'école 42.

## Plugins

### 42 / Norminette

| Plugin | Description |
|--------|-------------|
| [MoulatiMehdi/42norm.nvim](https://github.com/MoulatiMehdi/42norm.nvim) | Vérification de la norminette, formatage automatique et header 42 |
| [simrat39/symbols-outline.nvim](https://github.com/simrat39/symbols-outline.nvim) | Panel de symboles (fonctions, variables) dans un panneau latéral |

### Editeur

| Plugin | Description |
|--------|-------------|
| [folke/tokyonight.nvim](https://github.com/folke/tokyonight.nvim) | Thème de couleurs (tokyonight-night) |
| [echasnovski/mini.nvim](https://github.com/echasnovski/mini.nvim) | Suite mini : text objects (`mini.ai`), surround (`mini.surround`), statusline (`mini.statusline`) |
| [nvim-treesitter/nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter) | Coloration syntaxique avancée |
| [NMAC427/guess-indent.nvim](https://github.com/NMAC427/guess-indent.nvim) | Détection automatique de l'indentation |
| [folke/todo-comments.nvim](https://github.com/folke/todo-comments.nvim) | Met en surbrillance les TODO/NOTE/FIXME dans les commentaires |

### LSP & Complétion

| Plugin | Description |
|--------|-------------|
| [neovim/nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) | Configuration des serveurs LSP |
| [mason-org/mason.nvim](https://github.com/mason-org/mason.nvim) | Gestionnaire d'installation de LSPs et outils |
| [mason-org/mason-lspconfig.nvim](https://github.com/mason-org/mason-lspconfig.nvim) | Bridge entre Mason et lspconfig |
| [WhoIsSethDaniel/mason-tool-installer.nvim](https://github.com/WhoIsSethDaniel/mason-tool-installer.nvim) | Installation automatique d'outils via Mason |
| [saghen/blink.cmp](https://github.com/saghen/blink.cmp) | Autocomplétion rapide |
| [L3MON4D3/LuaSnip](https://github.com/L3MON4D3/LuaSnip) | Moteur de snippets |
| [folke/lazydev.nvim](https://github.com/folke/lazydev.nvim) | LSP Lua pour la config Neovim elle-même |
| [j-hui/fidget.nvim](https://github.com/j-hui/fidget.nvim) | Indicateur de progression LSP |

### Navigation & Recherche

| Plugin | Description |
|--------|-------------|
| [nvim-telescope/telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) | Fuzzy finder (fichiers, grep, LSP, etc.) |
| [nvim-telescope/telescope-fzf-native.nvim](https://github.com/nvim-telescope/telescope-fzf-native.nvim) | Extension fzf pour Telescope |
| [nvim-telescope/telescope-ui-select.nvim](https://github.com/nvim-telescope/telescope-ui-select.nvim) | UI select via Telescope |
| [folke/which-key.nvim](https://github.com/folke/which-key.nvim) | Affiche les keybinds disponibles en attente |

### Git

| Plugin | Description |
|--------|-------------|
| [lewis6991/gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim) | Signes git dans la gouttière (`+` ajout, `~` modif, `_` suppression) |

## Raccourcis clavier

### 42

| Touche | Action |
|--------|--------|
| `<F1>` | Insérer/mettre à jour le header 42 |
| `<F5>` | Lancer la norminette |
| `<leader>f` | Formater le buffer (norminette) |
| `<leader>cs` | Ouvrir le panneau de symboles |

### Terminal

| Touche | Action |
|--------|--------|
| `<leader>t` | Ouvrir un terminal vertical (100 colonnes, à gauche) |

### Telescope (Recherche)

| Touche | Action |
|--------|--------|
| `<leader>sf` | Rechercher des fichiers |
| `<leader>sg` | Live grep |
| `<leader>sw` | Chercher le mot sous le curseur |
| `<leader>sh` | Chercher dans l'aide |
| `<leader>sk` | Chercher les keymaps |
| `<leader>sd` | Chercher les diagnostics |
| `<leader>sr` | Reprendre la dernière recherche |
| `<leader>s.` | Fichiers récents |
| `<leader>sn` | Fichiers de config Neovim |
| `<leader><leader>` | Buffers ouverts |
| `<leader>/` | Fuzzy search dans le buffer courant |

### LSP

| Touche | Action |
|--------|--------|
| `grn` | Renommer |
| `gra` | Code action |
| `grr` | Références |
| `gri` | Implémentations |
| `grd` | Aller à la définition |
| `grD` | Aller à la déclaration |
| `gO` | Symboles du document |
| `gW` | Symboles du workspace |
| `grt` | Type definition |
| `<leader>th` | Toggle inlay hints |
| `<leader>q` | Quickfix diagnostics |

### Navigation fenêtres

| Touche | Action |
|--------|--------|
| `<C-h/j/k/l>` | Naviguer entre les splits |

## Installation

```sh
git clone <ton-repo> ~/.config/nvim
nvim
```

Lazy installe automatiquement tous les plugins au premier lancement.
