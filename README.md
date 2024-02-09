Custom Keyboards
================

As of the moment I only have one custom keyboard: the Ferris Sweep. 


### QMK
I use QMK for my firmware. You can start by moving cloning this repository into `qmk_firmware/keyboards/ferris/keymaps/Ramsesian` 

How do I edit and update the keymap?
------------------------------------

To view and edit the keymap use [qmk configurator](https://config.qmk.fm) by importing and exporting `keymap.json`

**What's with all the N/A's?**\n
The N/A stops you from going to other layers while not on the first. 

If you go from layer 01 to layer 02 you return to layer 01. However if you go from layer 01 -> layer 02 -> layer 03 then it returns to layer 02 and essentially now you're stuck there until you unplug and plug the keyboard back in again.

Flashing the Firmware
---------------------
Because of the `#define MASTER_LEFT` rule in `config.h` the keyboard needs to be plugged from the left side when flashing.

To flash run the following command in the terminal: `qmk flash -kb ferris/sweep -km Ramsesian` and then hit the reset button on the keyboard.
