---
date: 2023-03-03
draft: true
sr-due: 2023-03-17
sr-ease: 270
sr-interval: 4
tags:
    - inbox
    - definition
    - dev-tip
sr-due: 2024-01-22
sr-interval: 250
sr-ease: 290
---

# fzf

It's a general purpose fuzzy finder written in Golang that can be used with any
list of things: files, processes, command history, git branches, etc.

For [[z shell]], it provides the following key bindings

- `C-t`::Paste the selected file path(s) into the command line
- `C-r`::Paste the selected command from history into the command line
- `M-C`::`cd` into the selected directory

## Fuzzy completion mode

- Select multiple items with TAB key::`e **` and press `<TAB>`
- Select Files under parent directory::`e ../**<TAB>`
- Select Files under parent directory that match `fzf`::`e ../fzf**<TAB>`
- Select Files under your home directory::`e ~/**<TAB>`
- Select Directories under current directory (single-selection)::`cd **<TAB>`
- Select Host names::`ssh **<TAB>`
- Select Telent::`telnet **<TAB>`

- Select Directories under `~/.config` that match `nvim`
?
`cd ~/.config/nvim**<TAB>`

- Select Process IDs. Can select multiple processes with `TAB` or `S-TAB`
?
`kill -9 **<TAB>`

Select Environment variables / aliases
?
- `unset **<TAB>`
- `export **<TAB>`
- `unalias **<TAB>`
