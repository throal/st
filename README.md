# althro's st build
My personal build of the suckless simple terminal

## Patches & Features
- Xresources and pywal support
- alpha: adjustable from Xresources
- font2: emoji support
- scrollback: (`alt+↑/↓` or `mouse-up/mouse-down`)
- boxdraw

## Installation
In order to build st you need the Xlib header files.

```
git clone https://github.com/throal/st.git
cd st
sudo make install
```

If st crashes when viewing emojis, install [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra/) from the AUR.

On OpenBSD, be sure to edit `config.mk` first and remove `-lrt` from the `$LIBS` before compiling.

Be sure to have a composite manager (`xcompmgr`, `picom`, etc.) running if you want transparency.
