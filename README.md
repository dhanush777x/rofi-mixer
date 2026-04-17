# Rofi-mixer

Rofi-mixer allows you to manage your speakers, apps and microphones on systems with pulse audio (or pipewire with the pulse audio capabilities).

<img src="https://i.postimg.cc/TP1CRvMB/rofi-mixer.png" alt="rofi-mixer" />

## Usage

### Run rofi-mixer

```bash
rofi-mixer
```

### Use it

There are three available modes:

- **output** (speakers and the default)
- **applications**
- **input** (microphones, you have to switch to)

`Shift+left` or `Shift+right` are the default keybindings for changing modes in rofi.

## Shortcuts

| Shortcut     | Action                |
| ------------ | --------------------- |
| `+`, `=`     | Increase volume by 5  |
| `-`, `_`     | Decrease volume by 5  |
| `Alt+m`      | Mute device           |
| `Ctrl+equal` | Equalize L+R Speakers |

## Installation

Clone the repository and install the scripts to `~/.local/bin/`:

```bash
git clone https://github.com/dhanush777x/rofi-mixer.git && \
mkdir -p ~/.local/bin && \
cp rofi-mixer/src/rofi-mixer rofi-mixer/src/rofi-mixer.py ~/.local/bin/ && \
chmod +x ~/.local/bin/rofi-mixer ~/.local/bin/rofi-mixer.py && \
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc && \
source ~/.bashrc
```

This command will:

1. Clone the dotfiles repository
2. Create `~/.local/bin/` directory if it doesn't exist
3. Copy `rofi-mixer` and `rofi-mixer.py` from `src/` to `~/.local/bin/`
4. Make the scripts executable
5. Add `~/.local/bin/` to your PATH in `.bashrc`
6. Reload `.bashrc` to apply changes

After installation, you can run `rofi-mixer` from anywhere in your terminal.
