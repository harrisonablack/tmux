![](https://skillicons.dev/icons?i=linux,apple,bash,github)

# tmux
This is my personal tmux configuration.

The config is designed to be simple but powerful, with plugins managed through [TPM](https://github.com/tmux-plugins/tpm) and sessions managed with [sesh](https://github.com/joshmedeski/sesh). It enables mouse support, sane defaults, and includes a minimal dotbar at the top for a clean UI.

## Installation
> [!IMPORTANT]
> You’ll need `tmux >= 3.3`, [TPM](https://github.com/tmux-plugins/tpm), and [sesh](https://github.com/joshmedeski/sesh) installed for this config to work as expected.

Clone the repo into your tmux config folder, typically `~/.config/tmux`:

```bash
git clone https://github.com/harrisonablack/tmux.git ~/.config/tmux
```

Then start tmux and install plugins with:

```
prefix + I
```

(`prefix` by default is `ctrl+b`)
