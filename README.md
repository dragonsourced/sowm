# sowm (*Simple Opinionated Window Manager*)

<a href="https://github.com/dragonsourced/sowm/tree/master/img/light.png"><img src="img/light.png" width="48%"></a>
<a href="https://github.com/dragonsourced/sowm/tree/master/img/dark.png"><img src="img/dark.png" width="48%"></a>

An itsy bitsy floating window manager (*220~ sloc / 24kb compiled!*).

- Floating only.
- Fullscreen toggle.
- Window centering.
- Mix of mouse and keyboard workflow.
- Focus with cursor.
- Rounded corners (*[through patch](https://github.com/dylanaraps/sowm-patches)*)

- Alt-Tab window focusing.
- All windows die on exit.
- No window borders.
- [No ICCCM](https://web.archive.org/web/20190617214524/https://raw.githubusercontent.com/kfish/xsel/1a1c5edf0dc129055f7764c666da2dd468df6016/rant.txt).
- No EWMH.
- etc etc etc


<br>

Patches available here: https://github.com/dylanaraps/sowm-patches

## Default Keybindings

**Window Management**

| combo                      | action                 |
| -------------------------- | -----------------------|
| `Mouse`                    | focus under cursor     |
| `MOD4` + `Left Mouse`      | move window            |
| `MOD4` + `Right Mouse`     | resize window          |
| `MOD4` + `f`               | maximize toggle        |
| `MOD4` + `c`               | center window          |
| `MOD4` + `q`               | kill window            |
| `MOD4` + `1-9`             | desktop swap           |
| `MOD4` + `Shift` +`1-9`    | send window to desktop |
| `MOD1` + `TAB` (*alt-tab*) | focus cycle            |

**Programs**

| combo                    | action           | program          |
| ------------------------ | ---------------- | ---------------- |
| `MOD4` + `Return`        | terminal         | `st`             |
| `MOD4` + `Shift` + `q`   | kill sowm        | `killall`        |
| `MOD4` + `p`             | dmenu            | `menu_run`       |
| `MOD4` + `p`             | headphones menu  | `headphones`     |
| `MOD4` + `p`             | music menu       | `music`          |
| `MOD4` + `a`             | file manager     | `fman`           |
| `MOD4` + `s`             | screenshot       | `screenshot`     |
| `MOD4` + `space`         | keyboard layout  | `nextlayout`     |
| `XF86_AudioLowerVolume`  | volume down      | `chvol`          |
| `XF86_AudioRaiseVolume`  | volume up        | `chvol`          |
| `XF86_AudioMute`         | volume toggle    | `chvol`          |
| `XF86_MonBrightnessUp`   | brightness up    | `bri`            |
| `XF86_MonBrightnessDown` | brightness down  | `bri`            |


## Dependencies

- `xlib` (*usually `libX11`*).


## Installation

1) Copy `config.def.h` to `config.h` and modify it to suit your needs.
2) Run `make` to build `sowm`.
3) Copy it to your path or run `make install`.
    - `DESTDIR` and `PREFIX` are supported.
4) (Optional) Apply patch with `git apply patches/patch-name`
    - In case of applying multiple patches, it has to be done **manually**.


## Updating

    git pull
    git pull https://github.com/DylanAraps/sowm


## Thanks

- 2bwm
- SmallWM
- berry
- catwm
- dminiwm
- dwm
- monsterwm
- openbox
- possumwm
- swm
- tinywm
