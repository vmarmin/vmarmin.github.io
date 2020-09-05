---
layout: post
title:  "My dev environment"
tags: linux env neovim vscode manjaro i3
---

## Introduction

The purpose of this article is to mutualize information regarding my dev setup
so as to facilitate an installation from scratch.

## Linux installation

### Distribution

I am currently working on Manjaro with the i3 window manager.
[Download manjaro i3 Community
edition](https://manjaro.org/downloads/community/i3/)
[Manjaro installation
guide](https://wiki.manjaro.org/index.php/Installation_Guides)

Other potential candidates:
* [arch linux](https://www.archlinux.org/)

### i3wm

```sh
$ sudo pacman -S i3-gaps i3status i3lock yay blurlock
```

**Note:** will have to activate AUR in pamac/pacman

### Bonus desktop environment

Maybe get an additional more traditional desktop environment just in case.
XFCE seems to be worth a try.

### launcher

For now still hesitating between `rofi` and `dmenu` so get both. Personal config
now uses `rofi`.

```sh
$ sudo pacman -S rofi dmenu
```

### terminal

```sh
$ sudo pacman -S alacritty
```

### File manager

Get one graphical and one CLI file manager:

```sh
$ sudo pacman -S vifm nemo
```

Also get dropbox for file sharing.

### polybar

Default bar is replaced with polybar (config files needed). Polybar is part of
the AUR so it'll have to be installed with `yay`.

### Fonts

We will need the usual nerd fonts / ligatured fonts for the setup:
* Source Code Pro
* MesloLGS NF
* Fira / Fura
* Cascadia / Caskaydia
* Hack NF
* RobotoMono

### Communication

Currently used communication apps are:
* mailspring
* slack
* skype

### Browser

List of browsers to get:
* brave
* chrome for compatibility issues and selenium
* firefox for selenium

### Wallpaper

Install `feh` and setup random wallpaper selection from a given path.

### Music

Get spotify to enjoy new premium account!!

### Screenshot

Get i3-scrot

## Dev

### Neovim

Either use default neovim (pacman) or get the nightly neovim build with (yay).
Name should be something like `neovim-nightly`

Mainly using Neovim, but still using vscode every once in a while for specific
tasks (live server is just awesome!).

### Vscode

Get either vscode / vscodium. Note that there's apparently a way to get neovim
working under vscode.
