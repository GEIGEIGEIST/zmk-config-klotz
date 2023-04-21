<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/KLOTZ_font_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/KLOTZ_font_bright.svg">
  <img alt="KLOTZ logo font" src="/docs/images/KLOTZ_font_bright.svg">
</picture>

# ZMK CONFIG FOR THE KLOTZ SPLIT KEYBOARD

[Here](https://github.com/GEIGEIGEIST/klotz) you can find the hardware files and build guide for the KLOTZ.

KLOTZ is a 34 key column-staggered split keyboard running [ZMK](https://zmk.dev/). It supports a low profile encoder and three status LEDs on every side.

![KLOTZ layout](/docs/images/KLOTZ_layout.svg)


## HOW TO USE

- fork this repo
- `git clone` your repo, to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- adjust the klotz.keymap file (find all the keycodes on [the zmk docs pages](https://zmk.dev/docs/codes/))
- `git push` your repo to your fork
- on the GitHub page of your fork navigate to "Actions"
- scroll down and unzip the `firmware.zip` archive that contains the latest firmware
- connect the left half of the KLOTZ to your PC, press reset twice
- the keyboard should now appear as a mass storage device
- drag'n'drop the `klotz_left-nice_nano_v2-zmk.uf2` file from the archive onto the storage device
- repeat this process with the right half and the `klotz_right-nice_nano_v2-zmk.uf2` file.


## KNOWN ISSUES

- The encoder on the secondary side doesn't work yet. This is a limitation of ZMK.
- The code for the status LEDs needs to be added.




