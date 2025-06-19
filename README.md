# Installation

Build Helix with steel (this also installs the `forge` package manager):

```sh
git clone https://github.com/mattwparas/helix.git
git checkout steel-event-system
cargo xtask steel
```

Install the plugin:

```sh
forge pkg install --git https://github.com/mattwparas/steel-pty
```

Load the plugin by adding the following line to `~/.config/helix/init.scm`:

```
(require "steel-pty/term.scm")
```

# Usage

- `:open-term`: open a new terminal
- `Shift-Tab`: switch back to the editor
- `:new-term`: create a new terminal instance
- `:switch-term`: switch between terminal instances
- `:hide-terminal`: hide the terminal
- `:kill-current-terminal`: kill the current terminal instance

