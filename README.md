# linux-setup
My custom linux setup :)
based on Ubuntu 24.04

# GNOME as a tile manager
Using GNOME extensions to replicate the behavior and workflow of a tiling manager -at least my experience and workflow i previously had with i3- 

### But why not sticking to i3?
Tile managers can be minimal, including only window management and with the need to provide external utilities like: Network manager, lockscreen , file browser, keyboard, graphics, backgrounds... and the list goes on. Which can be painful to maintain and configure all together :(

So with this solution i see the **advantage** that GNOME comes out of the box from Ubuntu installation, and  its simple to configure, no need to worry about all the external utilities now that we are using the ones that come with Ubuntu :))

So to achieve this we only need a few GNOME extensions!

#### Gnome extensions: 
  - Space Bar: to add the workspace number in the space bar.
  - Search Light: File and app launcher.
  - Tactile: Resizing of windows on a custom grid using keyboard.
  - Just Perfection : Customization of shell animations

You can load a a saved config in this way:

```shell
dconf load /org/gnome/shell/extensions/ < some-file.txt
```

# Dotfiles 
All the dotfiles are managed in the following repo:
https://github.com/MarlonRiv/dotfiles

This repo is being mantained using [Chezmoi](https://github.com/twpayne/chezmoi) tool, that helps to manage personal configuration files (dotfiles, like ~/.gitconfig) across multiple machines.
