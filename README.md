# Raindrop by Granola Arcade

![Raindrop fightstick](/Images/raindrop.png "Raindrop fightstick")

The Raindrop is a button box style arcade controller by Granola Arcade. It is an upgraded version of the <a rel="TrailMix" href="https://github.com/michaelswitzer/granola-trailmix">TrailMix</a>, our first design. It has the same capabilities as the TrailMix but with a fully enclosed case and hotswap sockets that support Kailh Choc v1 and v2 switches. Due to the simple design requiring no tools or additional hardware for assembly, the Raindrop is available at a very competitive price.

You can buy the Raindrop at https://granola.games

## Should you make a Raindrop?
Building your own Raindrop will definitely be more expensive than buying one directly from Granola Arcade, and it isn't as fun to put together as some of the other DIY options out there. Nevertheless, if you decide to press on, the files in this repository should have everything you need.

## License
The Raindrop is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>. In simple terms, this means you are welcome to use or remix these designs to build your own Raindrop free of cost. You are *not* permitted to sell the Raindrop commercially. You also can't republish the designs without attribution and without carrying this license forward into your new designs. For more information see the license file in this repository.

## How to build
To build your own Raindrop, import the PCB designs and bill of materials using KiCAD. I provided a list of parts that use JLCPCB's part assembly services, since that is the company I use to manufacture the PCB. You can use these files as a starting point for building your own PCB.

The STL file for the case is optimized for FDM 3D printers. I recommend PLA with at least 15% infill but you can use any material you wish. The case is designed to be printed on the thin edge on the right side, which can cause some stability challenges when printing. **This orientation is better suited to printers that do not move their print bed side to side, and can be tricky to print on Prusa/Ender/etc. printers.** If you use a "bed slinger" printer such as these, make sure you have good bed adhesion.

You will also need to source your own key switches, hotswap sockets and keycaps. The Raindrop uses Kailh low-profile Choc keyboard switches.

## Firmware
The Raindrop is designed to use the <a rel="GP2040-CE firmware" href="https://github.com/OpenStickCommunity/GP2040-CE">GP2040-CE firmware</a>. You want the .uf2 file for the Raspberry Pi Pico as it has the same pinouts as the Raindrop. If you wish to use different firmware, you can view the schematic files to understand the layout of the board. If you bridge the Boot and GND pins (marked "BOOT" on the PCB) as you plug in the USB cord, you can upload new firmware in .uf2 format.

## Credits
The Raindrop was designed by Michael Switzer. The GP2040-CE firmware is maintained by <a href="https://github.com/OpenStickCommunity">OpenStickCommunity</a>. This project was inspired by the <a href="https://github.com/jfedor2/flatbox">Flatbox</a>.
