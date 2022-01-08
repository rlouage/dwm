# My Personal build of DWM
See [suckless.org](https://dwm.suckless.org "dwm.suckless.org") for the original source code.


## Patches
- [Systray](https://dwm.suckless.org/patches/systray/ "systray"): A simple system tray implementation. Multi-monitor is also supported. The tray follows the selected monitor. I use this for nm-applet.
- [attachbelow](https://dwm.suckless.org/patches/attachbelow/ "attachbelow"): Make new clients attach below the selected client, instead of always becoming the new master. Inspired heavily from the atttachabove patch.
- [autostart](https://dwm.suckless.org/patches/autostart/ "autostart"): This patch will make dwm run "~/.dwm/autostart.sh &" before entering the handler loop. One or both of these files can be ommited.
- [Keycodes](https://dwm.suckless.org/patches/keycodes/ "keycodes"): With this patch, handling key input is done with keycodes instead of keysyms. This way, input is independent from keyboard layout (you can get keycodes using xev to adapt config.h. This is useful for people that use azerty keyboard layouts.
- [statusbar on all monitors](https://dwm.suckless.org/patches/statusallmons/ "statusbar on all monitors"): This patch draws and updates the statusbar on all monitors. This system trays are only drawn on the active monitor.

## Installation
Clone this repository in whatever folder you want to keep the source code in, then go in the cloned directory and build the package:

```bash
  git clone https://www.github.com/rlouage/dwm
  cd dwm
  sudo make clean install
```
