# About
This repository is a central collection and improvements to various Apple-1 clone projects I've found around the internet. I have a particular fascination for the original Apple-1 and Datanetics Keyboard, so primarily I have compiled gerber files, kicad projects, instructions, and BOMs for how to build your own Apple-1 Clone as accurately as possible.

## Goals and Contributing

If you'd like to contribute, I'm always happy to accept work on anything that makes these files more accurate and complete.
### Schematics
- Schematic files need creating for the original Datanetics keyboard and Serial Board
- footprints need assigned to all components within all schematic files. this in most cases require the creating of custom footprints to ensure reproduction accuracy
### KiCad PCB Files
#### General
the PCB files should match as closely to the originals as possible.
All PCB files should be considered in WIP at current.
Ultimately:
- assign accurate pin mappings to all component footprints
- place footprints in their exact spot on the PCB.
- remove any duplicate layer geometry from laying the footprint over the gerber imported layers.
- re-attach all traces/nets to the footprints
- ultimately, passing a 0 error/0 warning DRC check

The PCB Files for all boards (with the exception of the Datanetics modern PCB) were made by importing gerber files first into KiCad, and mapping the schematics to it by applying footprints to the symbols, placing over the gerber geometry, and 
#### Mainboard
To properly view the pcb file's text elements, please download and install "Routed Gothic" font located in `/doc/`. This is the closest match I have found to the original PCB lettering in font form and is based on the Leroy stenciling system common with draftsman before computer fonts.

The gerber files were noted to have differences from the original in the forum posts, namely:
- The original has a matte finish, this one has a sligtly brighter green.
- The silkscreen doesn't cover the plated areas without soldermask.
- The DIP and breadboard solder pads should be wider although it only really matters in the breadboard area.
- The video adjustment pot pads are  narrower by 0.025", making it difficult to insert the trimpot.
#### Datanetics Keyboard (Modern)
The PCB file requires the installation of the plug-in library for Cherry MX keyswitches
### Gerber Files
Gerbers based on the PCB files have not yet been generated. only the original imported gerbers are located in the project

## Future Goals
In the future, once the above goals are met and I'm satisfied with them, I may consider working on an altered version of the main board that, while maintaining the same number and nature of the components, makes adequate substitutes such that another curious hobbyist would be able to buy as many components as possible off-the-shelf without having to hunt for "unicorn" parts. I'd like the ability to build one to be cheap and available to anyone who wants to do it, without having to sacrifice much at all in the way of board or schematic integrity. I would also like to provide a BOM that includes all required sockets needed for all the DIP chips in the system

## Contents & Progress

| Component                     | Author                |Schematic  | PCB File  |Gerbers    |3D Model| BOM File |
|-|-|-|-|-|-|-|
| mainboard                     | Schematics:[@nicolas-robin](https://github.com/nicolas-robin/a1_schematics) Gerber Files:[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)   |Y|WIP|Y (unlinked to pcb)|N|Y|
| aci                           |[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |N|Y (unlinked to pcb)|N|
| serialboard                   |[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |Y (unlinked to pcb)|N|N|
| transformers                  |[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |Y (unlinked to pcb)|N|N|
| Datanetics Keyboard (Modern)  |[@schlae](https://github.com/schlae/replica-datanetics)|Y|Y| Y (linked)| N|Y|
| Datanetics Keyboard (Original)|[willegal](https://www.willegal.net/appleii/apple1-datanetics.htm)  |Needed | WIP|Y (unlinked to pcb)|N|N|

## Acknowledgements

This repository contains only a fraction of original work. mostly, it is an amalgamation of a few different projects related to documenting and reproducing the Apple-1 Computer, with my work being mainly relegated to tying the gerber files and schematics together into a cohesive whole KiCad project. The attributions for the various portions of the project files are in the table above
* I am not sure the original source of the Mainboard PCB gerber files. the Applefritter forum post remarks that they were posted on an Apple-1 enthusiasts facebook group, but I do not have facebook nor would i know how to track down the original post. If anyone can give proper attribution to the files please reach out.
* The manual files I originally obtained from the Briel Computers website probably 15+ years ago and have kept on my system since. They are probably the best scans I've seen on the internet: watermark free, clean white pages, and clean, readable text without an overreliance on the contrast and brightness dials.



# Contents

