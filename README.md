<h1 align="center">:vertical_traffic_light: fuzzy-sys</h1>
<p align="center">
    <em>Utility for using systemctl interactively via <a href="https://github.com/junegunn/fzf">junegunn/fzf</a>.</em>
</p>

## :package: Installation

```bash
curl -LO https://raw.githubusercontent.com/sheepla/fuzzy-sys/master/fuzzy-sys && chmod +x fuzzy-sys
```

## :star: Features

All commands support multi selection via Tab.

```bash
Usage: fuzzy-sys [options]
Utility for using systemctl interactively via fzf.
If no options are given fully interactive mode is launched with system service units being used.
    -u          : work with --user services
    --start     : systemctl start <unit>
    --stop      : systemctl stop <unit>
    --restart   : systemctl restart <unit>
    --status    : systemctl status <unit>
    --edit      : systemctl edit --full <unit>
    --enable    : systemctl enable --now <unit>
    --disable   : systemctl disable --now <unit>
    --help      : print this message and exit

Examples:
    fuzzy-sys -u --edit    : edit a user service
    fuzzy-sys --start      : start a system service
```

## Demo

[![asciicast](https://asciinema.org/a/390806.svg)](https://asciinema.org/a/390806)
