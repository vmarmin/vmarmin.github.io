---
layout: post
title:  "i3 window manager"
tags: linux manjaro i3 wm i3wm
---

## Why i3?

i3wm is a tiling window manager. As opposed to more traditional window
managers, a tiling window manager aims to keep your hands on the keyboard. When
an application is launched in a workspace, it will occupy your whole screen
real estate. When a second application is launched on the same workspace, your
screen will be split in half to accomodate both windows.

Tiling window managers make great use of workspaces, and facilitates the
opening, closing, resizing or moving of windows without your hand needing to
reach for your mouse.

> **Note:** the version I'm using is i3-gaps, which is a fork of i3-wm with
> gaps available by default

Other popular tiling window managers out there:
* dwm
* awesomewm
* bspwm
* xmonad

More traditional desktop environments:
* kde
* xfce
* gnome

## Installing i3wm

i3wm can be installed through your default package manager, but if you are on
an arch based system, you may install i3wm and a few other essential components
with the following command:

```sh
$ sudo pacman -S i3-gaps i3lock i3status
```

> **Note:** if you're creating a fresh Manjaro installation, know that there
> Manjaro ships a community edition ISO with the i3 window manager
> [More info here...](https://manjaro.org/download/#i3)

## Configuring i3wm

[i3wm user guide](https://i3wm.org/docs/userguide.html)

When starting your i3 desktop environment for the very first time, you should
be prompted a warning stating that no i3 configuration has been found, and
suggest one is automatically generated for you.

### Terminal app

Current terminal preference goes to
[Alacritty](https://github.com/alacritty/alacritty), a cross platform terminal
emulator written in rust, wiwth GPU acceleration. It's simple, fast, and easy
to configure with its yaml config file.

```sh
sudo pacman -S alacritty
```

Configuration file can be found at `$HOME/.config/alacritty/alacritty.yml`

### Compositor

I've been using `compton` so far (config in `$HOME/.config/i3`) but the repo
is apparently stale so have a look at [`picom`](https://github.com/yshui/picom)

### launcher

For now still hesitating between `rofi` and `dmenu` so get both. Personal config
now uses `rofi`.

```sh
$ sudo pacman -S rofi dmenu
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
Configuration files and scripts are in `$HOME/.config/polybar`

```
exec_always --no-startup-id $HOME/.config/polybar/launch.sh
```
