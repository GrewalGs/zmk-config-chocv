# zmk-config-chocv

ZMK firmware config for the [chocV](https://github.com/brickbots/chocV) keyboard with Nice!Nano v2.

## Layout

3-layer keymap:

- **Layer 0 — Base:** QWERTY with home row mods (tap = letter, hold = modifier)
- **Layer 1 — Nav/Numpad:** Arrow keys, Home/End/PgUp/PgDn, F2/F4, numpad 0–9
- **Layer 2 — Symbols:** !, @, #, $, %, ^, &, *, (, ) on top row; raw modifiers on home row

## Home Row Mods

| Key | Tap | Hold |
|-----|-----|------|
| A | A | Left Shift |
| S | S | Left Ctrl |
| D | D | Left Alt |
| F | F | Left GUI (Win/Cmd) |
| J | J | Right GUI |
| K | K | Right Alt |
| L | L | Right Ctrl |
| ; | ; | Right Shift |

## Flashing

1. GitHub Actions builds the firmware automatically on every push.
2. Go to **Actions → latest run → Artifacts** and download `firmware.zip`.
3. Unzip — you'll find `chocv-nice_nano_v2-zmk.uf2`.
4. Double-tap reset on the Nice!Nano — it mounts as `NICENANO`.
5. Drag and drop the `.uf2` file onto the `NICENANO` drive.
6. Done — it flashes and reboots automatically.
