# RetroTINK 4K SCART2VGA Adapter

<img width="800" alt="pic08" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/5b902c31-59d6-4c3b-925e-643c47eb7815">

<img width="400" alt="pic01" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/e220464e-67d5-454c-a327-1b88799e715c"> <img width="400" alt="pic02" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/08c8b0ed-8aab-4e07-b2a3-94fadef2626f">
<img width="400" alt="pic03" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/8a7983ca-324f-4082-a550-b414791a461b"> <img width="400" alt="pic04" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/03e6a43b-b77b-4c51-8103-93f344e84073">

This is an adapter that converts the SCART IN port on the side of the [RetroTINK 4K](https://www.retrotink.com/product-page/retrotink-4k) to a rear-facing HD-15 VGA port.

This adapter makes it super easy to hook up my [Console VGA Dongle Series](https://github.com/jeffqchen/Console-VGA-Dongle-Series) to the RetroTINK 4K with one single VGA cable. Since my VGA dongles are not RGBHV devices, it makes more sense to leave the real HD-15 port for those that require RGBHV and use the SCART port instead.

This adapter is physically compatible with both the official shell and my own Founders Edition shell, which will be available at a later point.

<img width="400" alt="ogshell_out" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/b7464ea3-9be8-4d3f-bb4a-1661146d5f11"> <img width="400" alt="oghsell_in" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/ab4a3066-2132-49d7-85a1-34e73890db83">

<img width="400" alt="pic09" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/3cf8e537-7be8-4db5-a9b5-3bd96a1edc93"> <img width="400" alt="pic10" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/aa0377e1-0769-4d38-aaf6-4b5022b710d8">

------

## Signals

### Video

This adapter mainly accepts SCART-compliant RGBS video signal. Sync formats accepted are CSync, Luma or Composite Video.

This adapter can also pass the following formats through the proper pins:
- YPrPb
- RGsB
- CVBS on Pin 20

Please remember to adjust the input options in the Tink4K respectively.

### Audio

This adapter does not have a discrete analog audio input, since I wish to make the design as simple as possible. If you wish to hook up an external analog/digital audio source, please make use of the audio input assignment feature of the Tink4K and save the changes as your own profile.

------

## Parts

- PCB. 1.6mm thick - [Gerber File](https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/blob/main/KiCAD/gerber/RT4K_SCART2VGA.zip)
- 3D Printed Shell - [Link](https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/tree/main/3D%20Print)

- VGA Port Slim, Female - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Connectors/HD15/Slim/Female%20PCB/info.md)
- SCART Male Plug, Cable Type - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Connectors/SCART/Male%20Cable/info.md)
- SMD Resistor, imperial 0603 size, 470 Ohm
  - Buy from wherever you feel like (DigiKey, Mouser, Amazon, AliExpress, eBay)
- 2.54mm-pitched Pin Headers 1x2 and jumper

- [2x] M2x16mm screw and hex nut - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Parts/M2%20M3%20Hex%20Screw%20%26%20Nut/info.md)
- [1x] M4x20m screw and hex nut - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Parts/M4%20Hex%20Screw%20%26%20Nut/info.md)

### 3D Print

Print the models in the given vertical orientation. Support is necessary.

### Preparation

The plastic part of the SCART plug has several injection marks that need to be cleaned up with a sharp knife. Otherwise the PCB won't be able to sit flush with the back of the SCART plug.

<img width="400" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/f01cb6db-7968-4b5f-9419-6c7ee223280f"> <img width="400" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/682cbabd-526a-4427-9477-fe2a89396e83">

------

## Assembly

The most interesting part is to fit the SCART plug into the special footprint and solder it in.

Since these plugs are all made slightly differently, you will need some wiggling action to make all the pins go through the board. My advice would be to use a pair of tweezers and wiggle whichever pin that's not compliant. Fit one entire row/side first, then work on the other. Have patience and it will eventually go in. Never force it as you will bend the pins and make it impossible to fit.

<img width="400" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/6f57a5f5-26c1-4ebd-aa0b-3f6d1654d21a"> <img width="400" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/7fb9b6bc-7c61-4784-b078-2a4a856921f5">

Once the pins are all in, make sure the PCB can sit flush to the back of the plug. If there is any gap, the shell won't be able to close. Check if you missed any injection mark and cut it flush.

Then solder in the pin headers. Make sure they are not crooked or they will interfere with the shell.

Then, solder in the 470 Ohm SMD resistor and the VGA port. All ordinary.

The shell was designed with a very tight tolerance for physical strength. Please make sure you are going straight when sliding the PCB assembly into the shell.

Finally, close up the shell with two sets of M2x16mm screws and nuts.

## Attenuation

<img width="600" alt="attn" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/10aa0238-03ad-4dce-a59e-f1be09e8c44e">

When the jumper is closed, there is no additional attenuation on the sync line. This works with in-spec SCART signals.

If you are using 5V TTL-level sync from an out-of-spec device, or a VGA switcher box, you will want to leave the jumper open for the safety of the Tink4K. Addition space below is provided to store the loose jumper.

## Installation

<img width="400" alt="pic07" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/321a4bd5-e22b-4670-89b7-6ac1e6627375"> <img width="400" alt="pic06" src="https://github.com/jeffqchen/RetroTINK-4K-SCART2VGA-Adapter/assets/25773768/bfd60685-0151-44ab-a41a-4c99c1f521cd">

To install the adapter to the RetroTINK 4K, simply plug it in from the side, and fasten it in with one M4x20mm screw. This connection is robust enough for daily abuse.

------

## Special Thanks

Mike Chi - The Father of RetroTINK
- [RetroTINK 4K Product Page](https://www.retrotink.com/product-page/retrotink-4k)
- [Official Website](https://www.retrotink.com)
- [Twitter](https://twitter.com/retrotink2)

------

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
