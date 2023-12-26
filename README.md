# Scratchpad

A scratchpad for bspwm. Can be easily edited to support any WM.

### What is a scratchpad?

A scratchpad is a feature or utility that provides a quick and accessible space for temporary notes, calculations, or other quick information.

This script lets you store a window(s) to a toggleable desktop in bspwm, so you can quickly access them.

## Dependencies

-   `xdotool`
-   `bspwm` (default, customize the script to match your WM)

## Usage

There are 3 scripts:

1. `scratchpad` (Single window)

```sh
# Add the focused window to scratchpad if a window doesn't already exist:
scratchpad

# To toggle show/hide the window in scratchpad:
scratchpad

# To remove the window from the scratchpad
# 1. Kill the window
# 2. Delete .cache
```

2. `scratchpad-tiles` (Multi-window)

```sh
Usage:
    scratchpad-tiles [CONFIG]       Toggle the scratchpad

Commands:
    save [CONFIG]                   Save the current layout to the given config
    edit [CONFIG]                   Edit the given config

The default config location is ~/.config/scratchpad/mainrc
```

3. `scrachpad-global-toggle` (Multi-window)

Helper script that toggles visibility of multiple scratchpad windows. Any window that is marked as sticky is considered as a scratchpad window.

This is basically a simplified `scratchpad-tiles` with no config file and program launching.

```sh
scrachpad-global-toggle # Toggle visibility of sticky windows
```
