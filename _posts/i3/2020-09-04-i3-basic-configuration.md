---
layout: post
title:  "My dev environment"
tags: linux manjaro i3 wm i3wm
---
# i3 basic configuration

## Why i3?

i3wm is a tiling window manager. As opposed to more traditional window managers,
a tiling window manager aims to keep your hands on the keyboard. When an
application is launched in a workspace, it will occupy your whole screen real
estate. When a second application is launched on the same workspace, your screen
will be split in half to accomodate both windows.

Tiling window managers make great use of workspaces, and facilitates the opening,
closing, resizing or moving of windows without your hand needing to reach for
your mouse.

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

i3wm can be installed through your default package manager, but if you are on an
arch based system, you may install i3wm and a few other essential components with
the following command:

```sh
$ sudo pacman -S i3-gaps i3lock i3status
```

> **Note:** if you're creating a fresh Manjaro installation, know that there
> Manjaro ships a community edition ISO with the i3 window manager
> [More info here...](https://manjaro.org/download/#i3)
