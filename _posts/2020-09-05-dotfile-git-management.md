---
layout: post
title: "Dotfiles management with git"
tags: dotfile config git linux
---

## Why?

When you work on different setups, different platforms, different setups, or if
you regularly distro hop, managing your configuration files with git becomes a
real life savior.

This article gives information about how to handle this feat.

## First time

If you do not manage your dotfiles with git, you may do so with the following
commands:

```sh
# Create bare repository
git init --bare $HOME/.cfg
# Create alist
alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'
# Deactivate showing untracked files
config config --local status.showUntrackedFiles no
# Add alias to your bashrc / zshrc file
echo "alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'" >> $HOME/.zshrc
```

You can then start adding your files to your git repo as such:

```sh
config status
config add .vimrc
config commit -m "Add vimrc"
config add .bashrc
config commit -m "Add bashrc"
config push
```

## Manage new host

> Note: need to update my own alias there. TODO on `work-linux`

```sh
# Clone dotfile folder
git clone --bare <git-repo-url> $HOME/.cfg
# Define local alias
alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'
# Checkout
config checkout
```

## Sources

https://www.atlassian.com/git/tutorials/dotfiles
