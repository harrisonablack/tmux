![](https://skillicons.dev/icons?i=linux,apple,bash,github)

# tmux
This is my personal tmux configuration.

The config is designed to be simple but powerful, with plugins managed through [TPM](https://github.com/tmux-plugins/tpm) and sessions managed with [sesh](https://github.com/joshmedeski/sesh). It enables mouse support, sane defaults, and includes a minimal dotbar at the top for a clean UI.

## Installation and setup
> [!IMPORTANT]
> You’ll need `tmux >= 3.3`, [TPM](https://github.com/tmux-plugins/tpm), and [sesh](https://github.com/joshmedeski/sesh) installed for this config to work as expected.

Clone the repo into your tmux config folder, typically `~/.config`:

```bash
git clone https://github.com/harrisonablack/tmux.git ~/.config/tmux
```

Then start tmux and install plugins with:

```
prefix + I
```

(`prefix` by default is `ctrl+b`)

## Plugins
```tmux
set -g @plugin 'tmux-plugins/tpm'             # Plugin manager
set -g @plugin 'tmux-plugins/tmux-sensible'   # Sane defaults
set -g @plugin 'vaaleyard/tmux-dotbar'        # Minimal top bar
set -g @plugin 'alexwforsythe/tmux-which-key' # Keymap hints
```

## Features
- **Mouse support** enabled by default
- **Base index = 1** for panes and windows
- **Dotbar** on top (`black background`)
- **Which-key style help** for bindings
- **Extended keys & focus events** for modern terminals
- **Sesh integration**:
  - `prefix + k`: Fuzzy session selector with preview
  - `prefix + L`: Jump to last session
- **Reload config** with `prefix + r`
- **Kill pane** with `prefix + x`
- Keeps sessions alive with `detach-on-destroy off`

---
