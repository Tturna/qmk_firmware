# Quantum Mechanical Keyboard Firmware

[Original readme](https://github.com/qmk/qmk_firmware)

# Setup

1. Get QMK Firmware (clone this repo)
2. Install QMK (`pacman -S qmk`)
3. `qmk setup`
4. Find your keyboard with `qmk list-keyboards`
5. `qmk config user.keyboard=<keyboard path from above command>. Example:
   `qmk config user.keyboard=keebio/iris_ce/rev1`
6. Choose default keymap name: `qmk config user.keymap=tturna`
7. Compile my keymap: `qmk compile -km tturna`
8. Put keyboard in bootloader mode. [Iris CE Info](https://github.com/Tturna/qmk_firmware/blob/master/keyboards/keebio/iris_ce/readme.md#bootloader), [General Info](https://docs.qmk.fm/newbs_flashing#put-your-keyboard-into-dfu-bootloader-mode) 
8. Flash default keymap: `qmk flash` or follow [this](https://docs.qmk.fm/newbs_flashing#flash-your-keyboard-from-the-command-line)
   *Note: This didn't work on my Linux system. My keyboard uses the rp2040 controller so I was able to get around it by just enabling bootloader mode, which made the keyboard show up in my file manager and then copying the compiled firmware onto the kb.*

[General QMK info](https://docs.qmk.fm/)
[Setting up QMK environment](https://docs.qmk.fm/newbs_getting_started)
[Building firmware](https://docs.qmk.fm/newbs_building_firmware)
[Flashing firmware](https://docs.qmk.fm/newbs_flashing)
[Keycodes. More on the left side list](https://docs.qmk.fm/keycodes)

