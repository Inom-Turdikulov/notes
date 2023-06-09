---
date: 2022-12-29
draft: true
sr-due: 2024-03-17
sr-ease: 270
sr-interval: 4
tags:
- inbox
- definition
- dev-tip
---

# dwm (dynamic window manager)

> dwm is a dynamic window manager for X. It manages windows in tiled, monocle
> and floating layouts. All of the layouts can be applied dynamically,
> optimizing the environment for the application in use and the task performed\
> —&thinsp;<cite>[dwm](https://dwm.suckless.org/)</cite>

![My configured DWM with 2 windows in
foreground](../pasted_img_20230102033318.png)
_My configured DWM with 2 windows in foreground_

I used long time `i3wm`, `KWin`, `GNOME`, `Desktop Window Manager`, various
status bars (like `polybar`), etc. But after that I discovered DWM, I just
switched to it and use it with maximum pleasure. It has some "disadvantages",
maybe not clear logic if you use it first time, but It's all manageable and
solvable. Especially if you use something like `DWM flexipatch`.

Right now I use various patches, with this DWM fork:
[bakkeby/dwm-flexipatch](https://github.com/bakkeby/dwm-flexipatch).

To use dwm effectively, I use my own [[dwm keyboard shortcuts]].

## Launching

Here my `~/.xinitrc`:

```bash
# load my environment variables
[ -f ~/.profile ] && . ~/.profile
[ -f ~/.profile-keys ] && . ~/.profile-keys

# load autostart programs and autorandr
[ -f ~/.xprofile ] && . ~/.xprofile

picom --experimental-backend  --backend glx --config ~/.config/picom/picom.conf -b
exec dwm
```

## Window model

```
+------+----------------------------------+--------+
| tags | title                            | status |
+------+---------------------+------------+--------+
|                            |                     |
|                            |                     |
|                            |                     |
|                            |                     |
|          master            |        stack        |
|        (first window)      |     (second window) |
|                            |                     |
|                            |                     |
|                            |                     |
+----------------------------+---------------------+
```

_Tiled layout_

By default, dwm in ==tiled== layout. But you can switch between ==tiled==,
==monocle==, ==floating== layouts.

For additional information, see [[dwm keyboard shortcuts]].

## Additional functional

### Status bar

I use customized `dwmblocks`.

Enabled modules are: `datetime`, volume status and keyboard layout.
That items are not interactive.

I also created custom modules, `dnd`.

- [dnd](https://github.com/inomoz/dotfiles/blob/main/.local/bin/dnd)
(Do Not Disturb), key <kbd>s-C-n</kbd>.
It's toggling notifications pause mode, in status bar displayed ⛔ icon.

## Keyboard shortcuts

Keyboard shortcuts are described in [[dwm keyboard shortcuts]] note.

## Useful links
- <https://dwm.suckless.org/tutorial/>
- <https://ratfactor.com/dwm>
- <https://wiki.gentoo.org/wiki/Dwm>
- <https://dwm.suckless.org/customisation/windows_key/>

## To-Do

- TODO: create repo with my patches
- TODO: describe dwmblocks
