# macropad-4x4
# 4x4_hardwire_navi

This 4x4 macro pad features blue mechanical switches for a tactile and responsive typing experience. Powered by an RM2040 microcontroller, it offers seamless integration and customization through QMK firmware. Ideal for productivity enthusiasts, it streamlines complex commands into a compact, efficient tool.

* Keyboard Maintainer: [Vikas Lekule](https://github.com/naaviiiii)
* Hardware Supported: *Any mechanical switch, RM2040 based microcontrolller, Basic soldering iron, 1N4148 Diode*
* Hardware Availability: PI Pico - https://www.raspberrypi.com/products/raspberry-pi-pico/
                         Outemu blue switch - https://www.thecosmicbyte.com/product/outemu-mechanical-switches-for-swappable-keyboards-pack-of-20/
                         1N4148 Diode - https://www.amazon.in/100PCS-1N4148-IN4148-switching-Switching/dp/B08DYFFYPQ  

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Hard wiring switches and diodes

* Refer - https://drive.google.com/file/d/1gYBCJdPZoJWls1ArRAr4n0JoImES1Bxe/view?usp=drivesdk
* Note - Use insulated wire for rows, non insulated wire is fine for columns (so that they dont bridge connections


## Direct firmware install

Installing firmware without editing keymap.c and keyboard.json file 

* 4x4_hardwire_navi_default is firmware file which you can directly copy to pi pico in bootloader mode
* Connect ROWs to pin - GP0, GP1, GP2, GP3 (Refer -https://www.raspberrypi.com/documentation/microcontrollers/images/pico-pinout.svg)
* Connect COLs to pin - GP10, GP11, GP12, GP13 (Refer -https://www.raspberrypi.com/documentation/microcontrollers/images/pico-pinout.svg)


## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available
