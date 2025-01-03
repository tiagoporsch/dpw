# Declarative Pacman Wrapper
Wraps Arch's `pacman` based on a `.ini` file containing a list of packages.

The packages file lives by default in `$HOME/.config/dpw/packages.ini`, and if it doesn't exist, it may be created upon executing the script for the first time using your currently installed packages.

It supports comments using `#`, either on the start or the middle of the line, for example:

```ini
### gui
kitty
nautilus-open-any-terminal # kitty
```

Searches for any available `pacman` wrapper by default, but it can be easily changed by modifying the `PACMAN` environment variable.

## Usage
See `dpw help`
