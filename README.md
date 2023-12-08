# RetroTINK 4K SCART2VGA Adapter

This is an adapter that converts the SCART IN port on the side of the RetroTINK 4K to a rear-facing HD-15 VGA port.

This adapter makes it super easy to hook up my [Console VGA Dongle Series](https://github.com/jeffqchen/Console-VGA-Dongle-Series) to the RetroTINK 4K with one single VGA cable. Since my VGA dongles are not RGBHV devices, it makes more sense to leave the real HD-15 port for those that require RGBHV and use the SCART port instead.

This adapter is physically compatible with both the official shell and my own Founders Edition shell, which will be available at a later point.

## Signals

This adapter can also pass the following formats through the proper pins:
- YPrPb
- RGsB
- CVBS on Pin 20

This adapter does not have a discrete analog audio input, since I wish to make the design as simple as possible. If you wish to hook up an external analog/digital audio source, please make use of the audio input assignment feature of the Tink4K and save the changes as your own profile.


## Parts

- PCB
- 3D Printed Shell

- VGA Port Slim, Female - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Connectors/HD15/Slim/Female%20PCB/info.md)
- SCART Male Plug, Cable Type - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Connectors/SCART/Male%20Cable/info.md)
- SMD Resistor, imperial 0603 size, 470 Ohm
  - Buy from wherever you feel like (DigiKey, Mouser, Amazon, AliExpress, eBay)
- 2.54mm-pitched Pin Headers 1x2 and jumper

- [2x] M2x16mm screw and hex nut - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Parts/M2%20M3%20Hex%20Screw%20%26%20Nut/info.md)
- [1x] M4x20mm screw

## 3D Print

Print the models in the given vertical orientation. Support is necessary.

## Preparation

The plastic part of the SCART plug has several injection marks that need to be cleaned up with a sharp knife. Otherwise the PCB won't be able to sit flush with the back of the SCART plug.

## Assembly

The most interesting part is to fit the SCART plug into the special footprint and solder it in.

Since these plugs are all made slightly differently, you will need some wiggling action to make all the pins go through the board. My advice would be to use a pair of tweezers and wiggle whichever pin that's not compliant. Fit one entire row/side first, then work on the other. Have patience and it will eventually go in. Never force it as you will bend the pins and make it impossible to fit.

Once the pins are all in, make sure the PCB can sit flush to the back of the plug. If there is any gap, the shell won't be able to close. Check if you missed any injection mark and cut it flush.

Then solder in the pin headers. Make sure they are not crooked or they will interfere with the shell.

Then, solder in the 470 Ohm SMD resistor and the VGA port. All ordinary.

Finally, close up the shell with two sets of M2x16mm screws and nuts.

## Attenuation

When the jumper is closed, there is no additional attenuation on the sync line. This works with in-spec SCART signals.

If you are using 5V TTL-level sync from an out-of-spec device, or a VGA switcher box, you will want to leave the jumper open for safety of the Tink4K. Addition space below is provided to store the jumper.

## Installation

To install the adapter to the RetroTINK 4K, simply plug it in from the side, and fasten it in with one M4x20mm screw. This connection is robust enough for daily abuse.