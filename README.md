# macropad-4x4
# 4x4_hardwire_navi

This 4x4 macro pad features blue mechanical switches for a tactile and responsive typing experience. Powered by an RM2040 microcontroller, it offers seamless integration and customization through QMK firmware. Ideal for productivity enthusiasts, it streamlines complex commands into a compact, efficient tool.

* Keyboard Maintainer: [Vikas Lekule](https://github.com/naaviiiii)
* Hardware Supported: *Any mechanical switch, RM2040 based microcontrolller, Basic soldering iron*
* Hardware Availability: PI Pico - https://www.raspberrypi.com/products/raspberry-pi-pico/
                         Outemu blue switch - https://www.thecosmicbyte.com/product/outemu-mechanical-switches-for-swappable-keyboards-pack-of-20/   

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available
