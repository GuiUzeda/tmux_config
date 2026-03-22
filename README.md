# 🐧 My Tmux Configuration

A high-performance, aesthetically pleasing `tmux` setup featuring **Bluloco** colors, specialized popups, and seamless integration with **Neovim** and **Fish Shell**.

---

## 🚀 Key Features

- **Shell:** Integrated with `fish` shell.
- **Leader Key:** Rebound to `Ctrl+a`.
- **Modern UI:** Bluloco color palette with custom status bar and pane borders.
- **Smart Popups:** Quick access to `lazygit`, `btop`, and a scratchpad.
- **Navigation:** Seamless pane switching between `tmux` and `neovim`.
- **Persistence:** Automatic session saving and restoration via `tmux-resurrect` and `tmux-continuum`.
- **Layout:** Symmetric forward-slash status bar design.

---

## ⌨️ Key Bindings

### Core

| Binding        | Action                                   |
| :------------- | :--------------------------------------- |
| `Prefix + r`   | Reload configuration                     |
| `Prefix + I`   | Install plugins & check dependencies     |
| `Prefix + c`   | Create new window (preserves path)       |
| `Prefix + \| ` | Split pane horizontally (preserves path) |
| `Prefix + _`   | Split pane vertically (preserves path)   |
| `Prefix + x`   | Kill pane (with confirmation)            |

### Popups & Utilities

| Binding      | Action                         |
| :----------- | :----------------------------- |
| `Prefix + g` | Open **Lazygit** popup         |
| `Prefix + t` | Open **Btop** popup            |
| `Prefix + f` | Fuzzy session switcher (`fzf`) |
| `Prefix + h` | Open floating scratchpad       |

### Session Management

| Binding      | Action                               |
| :----------- | :----------------------------------- |
| `Prefix + N` | Create and switch to a new workspace |
| `Prefix + S` | Manually save session                |
| `Prefix + R` | Manually restore session             |

### Smart Navigation (Ctrl-based)

_Works seamlessly across Tmux and Neovim._

- `Ctrl + h/j/k/l`: Select pane Left/Down/Up/Right.
- `Alt + h/j/k/l`: Resize pane Left/Down/Up/Right.

### Copy Mode (Vim style)

- `v`: Begin selection.
- `y`: Copy to Wayland clipboard (`wl-copy`).
- `Esc`: Cancel.

---

## 🎨 Theme (Bluloco)

- **Active Pane:** Highlighted with `#10B1FE` bold borders and specialized headers.
- **Status Bar:** Top-positioned with a symmetric slash layout.
- **Modules:**
  - `` Session Name
  - `` CPU Usage
  - `󰍛` Memory Usage
  - `󟀵` Disk Space
  - `󱐋` Prefix Indicator

---

## 🔌 Plugins

This configuration uses [TPM (Tmux Plugin Manager)](https://github.com/tmux-plugins/tpm):

- `tmux-plugins/tpm`: Plugin manager.
- `tmux-plugins/tmux-resurrect`: Save and restore tmux environment.
- `tmux-plugins/tmux-continuum`: Continuous saving of tmux environment.

---

## 🛠️ Requirements

To use all features of this config, you need:

- `fish` shell
- `fzf` (for session switcher)
- `lazygit` (for Git popup)
- `btop` (for system monitoring)
- `wl-copy` (for Wayland clipboard support)
- A Nerd Font (for icons)
