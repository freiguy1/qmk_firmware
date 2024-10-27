# Sofle Choc Keyboard

![Sofle Choc Photo](https://i.imgur.com/MhSEAZYh.jpg)

## Ethan's notes:

Command to build using docker build environment:

`util/docker_build.sh sofle_choc:default -e CONVERT_TO=helios`

Then to flash the device:
1. Unplug usb & trrs cable
2. Plug in one side
3. Wait for boot up (lights)
4. Hold reset for like 1 second, will boot as removable disk
5. Copy uf2 file to disk
6. Do same to other half

Todos:
- Would be nice to just use the delete key with the left hand (like when deleting emails or any other thing I'm selecting with my mouse). Done - lower + F
- All number keys and number symbols can go away
- Is there home and end? Yes - lower + M or \[period]
- Remove all stuff related to dvorak/colmak
- Win/alt switch for mac mode (includes copy, paste, cut, home, end, next word, previous word, maybe more) kinda done
- Change arrows to vim style arrows done
- Screenshot hotkey (different between mac and win)


The Sofle Choc is 6×4+5 keys column-staggered split keyboard. Based on Lily58, Corne and Helix keyboards. The Sofle Choc variant uses low profile Kailh choc switches, hotswap sockets, per-key RGB using the easier to solder SK6812 Mini-E, and is fairly thin at 15mm from desktop to top of keycaps.

More details about the keyboard and build guide: [Sofle Choc Build GUide](https://josefadamcik.github.io/SofleKeyboard/build_guide_choc.html)

* Keyboard Maintainer: [Brian Low](https://github.com/brianlow/)
* Hardware Supported: Sofle Choc PCB 2.x, ProMicro
* Hardware Availability: [PCB & Case Data](https://github.com/josefadamcik/SofleKeyboard)

Make example for this keyboard (after setting up your build environment):

    make sofle_choc:default

Flashing example for this keyboard:

    make sofle_choc:default:flash

Press reset button twice on the keyboard when asked.

Disconnect the first half, connect the second one and repeat the process.

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).
