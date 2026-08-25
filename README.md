# Eva-01 for Xfce Terminal

A compact color scheme for **Xfce4 Terminal**, available in two variants:

- **`Eva-01.theme`** — 8-color palette, mirrored into the bright ANSI slots for Xfce4 Terminal compatibility.
- **`Eva-01.16.theme`** — full 16-color palette with dedicated normal and bright colors.

## Palette

The theme is built around these colors:

| Role | Color |
|---|---|
| Background | `#000000` |
| Purple | `#A877C8` |
| Green | `#A2DB5A` |
| Blue | `#A1B2DE` |
| Yellow | `#F7BB29` |

The 16-color version also includes darker and lighter variations of the same palette.

## Installation

Xfce4 Terminal follows the XDG base directory specification for its data files.

### Per-user installation

Install the themes only for the current user:

```bash
mkdir -p ~/.local/share/xfce4/terminal/colorschemes
cp Eva-01.theme Eva-01.16.theme ~/.local/share/xfce4/terminal/colorschemes/
```

If you use a custom `XDG_DATA_HOME`, install them under:

```text
$XDG_DATA_HOME/xfce4/terminal/colorschemes/
```

By default, `XDG_DATA_HOME` is `~/.local/share`.

### System-wide installation

For all users, install the themes in a system XDG data directory.

On most Linux distributions:

```bash
sudo mkdir -p /usr/share/xfce4/terminal/colorschemes
sudo cp Eva-01.theme Eva-01.16.theme /usr/share/xfce4/terminal/colorschemes/
```

A cleaner location for manually installed files is often `/usr/local/share`:

```bash
sudo mkdir -p /usr/local/share/xfce4/terminal/colorschemes
sudo cp Eva-01.theme Eva-01.16.theme /usr/local/share/xfce4/terminal/colorschemes/
```

You can check the system data directories currently configured with:

```bash
echo "${XDG_DATA_DIRS:-/usr/local/share:/usr/share}"
```

The theme directory must be placed below one of those paths as:

```text
xfce4/terminal/colorschemes/
```

## Enable the theme

Open **Xfce4 Terminal** and go to:

```text
Edit → Preferences → Colors → Presets
```

Select either:

- **Eva-01**
- **Eva-01.16**

If the theme does not appear immediately, close and reopen Xfce4 Terminal.

You can display the terminal's ANSI color table with:

```bash
xfce4-terminal --color-table
```

## Uninstall

### Per-user

```bash
rm -f ~/.local/share/xfce4/terminal/colorschemes/Eva-01.theme
rm -f ~/.local/share/xfce4/terminal/colorschemes/Eva-01.16.theme
```

### System-wide

If installed under `/usr/share`:

```bash
sudo rm -f /usr/share/xfce4/terminal/colorschemes/Eva-01.theme
sudo rm -f /usr/share/xfce4/terminal/colorschemes/Eva-01.16.theme
```

If installed under `/usr/local/share`:

```bash
sudo rm -f /usr/local/share/xfce4/terminal/colorschemes/Eva-01.theme
sudo rm -f /usr/local/share/xfce4/terminal/colorschemes/Eva-01.16.theme
```

## Files

```text
Eva-01.theme
Eva-01.16.theme
README.md
```

## License

No license is included by default. Add a `LICENSE` file before publishing if you want to specify how others may use, modify, and redistribute the themes.
