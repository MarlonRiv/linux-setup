# linux-setup
My custom linux setup :)
based on Ubuntu 24.04

# GNOME as a tile manager
Using GNOME extensions to replicate the behavior and workflow of a tiling manager -at least my experience and workflow i previously had with i3- 

### But why not sticking to i3?
Tile managers can be minimal, they include only window management, with the need of the user to provide external utilities like: Network manager, lockscreen , file browser, keyboard, graphics, backgrounds... and the list goes on. Which can be painful to maintain and configure all together. :(

So with this solution i see the **advantage** that GNOME comes out of the box from Ubuntu installation, and  it's simple to configure with no need to worry about all the external utilities, now that we are using the ones that come with our Ubuntu installation. :))

We can get close to the workflow of a tile manager with only a few GNOME extensions!

#### Gnome extensions: 
  - **Space Bar**: to add the workspace number in the space bar.
  - **Search Light**: File and app launcher.
  - **Tactile**: Resizing of windows on a custom grid using keyboard.
  - **Just Perfection** : Customization of shell animations

You can save your extensions config in this way:

```shell
dconf load /org/gnome/shell/extensions/ > some-file.txt
```

You can load a a saved config in this way:

```shell
dconf load /org/gnome/shell/extensions/ < some-file.txt
```

# Dotfiles 
All the dotfiles are managed in the following repo:
https://github.com/MarlonRiv/dotfiles

This repo is being mantained using [Chezmoi](https://github.com/twpayne/chezmoi) tool, that helps to manage personal configuration files (dotfiles, like ~/.gitconfig) across multiple machines.

# HomeBrew: Package manager
[Homebrew](https://github.com/homebrew) - a package manager for macOS and Linux.

When i started with this ricing journey i quickly noticed APT falls short for what i wanted, the versions that are released for most of the development tools where not available or had older versions. Thanks to HomeBrew, we can have the latest stable versions of most of the dev tools :D

You can have a clean way of installing packages with HomeBrew, as it installs packages to their own directory and then symlinks their files into _/opt/homebrew_. 

# Neovim 
> [!WARNING]
> At least version 0.10, as most plugins requires Nvim version 0.10, (APT has 0.9.5, and the latest stable version of noevim is 0.11.2)

- **Lua**: It's a scripting language that has a runtime built-in to Neovim, thanks to it we can add plugins in a modular way, having a configuration file for each plugin under the **plugins** folder.  
- [LazyVim](https://github.com/LazyVim/LazyVim): Package manager  to get an IDE-level status that lazily load packages.

- [Neotree](https://github.com/nvim-neo-tree/neo-tree.nvim): Neovim plugin to manage the file system and other tree like structures. 

- [Telescope](https://github.com/nvim-telescope/telescope.nvim): Powerful file searching capabilities.

- [Treesitter](https://github.com/nvim-treesitter/nvim-treesitter): Coloring different parts of your code differently. Treesitter takes code and generates an Abstract Syntax Tree (AST): helping tools understand the structure of the code,

- [Mason](https://github.com/mason-org/mason.nvim): A package that downloads and installs binaries for your neovim instance.
    
- [Mason lsp config](https://github.com/mason-org/mason-lspconfig.nvim): A package that will close the gap between the installed binaries from Mason, and the actual communication to neovim's LSP client.
    
- [Nvim LSP Config](https://github.com/neovim/nvim-lspconfig): A package that contains configs for LSP servers and neovim. It essentially handles the communication between Neovim's LSP client and LSP servers

- [LazyGit](https://github.com/jesseduffield/lazygit): A simple terminal UI for git.

# Tmux
- Tmux plugin manager [TPM](https://github.com/tmux-plugins/tpm)

# Other tools

- [Ghostty](https://github.com/ghostty-org/ghostty): 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.
- [Batcat](https://github.com/sharkdp/bat): A cat with wings.
- [Fzf](https://github.com/junegunn/fzf):  A command line fuzzy finder.
- [Yazi](https://github.com/sxyazi/yazi): A terminal file manager.





