---
title: "tmux configuration"
date: 2022-05-14
menu: "configuration"
weight: 1
---

Set keyboard shortcut (ctr+a) to screens and colorize. Place this tmux.conf in /etc or as .tmux.conf file in your home directory (~).
```
unbind C-b
set -g prefix C-a

# Set status bar
set -g status-bg black
set -g status-fg white
set -g status-left ‘#[fg=green]#H’
```

