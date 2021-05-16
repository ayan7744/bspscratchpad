# bspscratchpad
![posix-compliant](https://img.shields.io/static/v1?label=posix&message=compliant&color=blue&style=for-the-badge) &nbsp;

A simple script to provide i3-like scratchpad functionality for bspwm. 
## Installation and Usage
Put the script in your `$PATH`. Main functions:
1. Put focused window into scratchpad or remove it from scratchpad:
```bash
bspscratchpad --toggle
```
1. Cycle through the windows in scratchpad:
```bash
bspscratchpad --cycle
```
These commands are meant to be executed with the help of a hot-key daemon, for instance, `sxhkd`, `xbindkeysrc`, etc. I have the following lines in my `sxhkdrc`:
```cfg
mod1 + shift + w
    bspscratchpad --toggle

mod1 + w 
    bspscratchpad --cycle
```
