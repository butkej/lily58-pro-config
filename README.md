# Flashing Instructions for my Lily58 Pro with my custom keymap

![My custom Lily58 Pro with 2 EliteC controllers and acrylic case](PXL_20201214_092310162.jpg?raw=True "Lily58 Pro")


1. Download and install qmk_firmware
2. get this lily58 repo and replace the original lily58 folder that can be found in qmk_firmware/keyboards/lily58
3. in lily58/keymaps/bigbang you can find my personal keymap that can be modified by editing keymap.c

## How to flash
- connect the left keyboard half (without TRRS cable) only
- cd into qmk_firmware/
- run  
    sudo make lily58/rev1:bigbang:dfu-split-left
- while running reboot the keyboard half by pressing the small switch under the OLED cover

Do the same steps for the right side afterwards (also with only the right side connected)  
    sudo make lily58/rev1:bigbang:dfu-split-right

