This repository is a collection of different projects I've found around the internet relating to building a near-exact clone of the Apple-1 computer. My intention is for it to act as a central repository for information that may otherwise be obscure decentralized, or link rot in the future. For aspiring builders, having everything in one place helps with prep work, troubleshooting, and familiarizes with the scope of the project.

# About the "Doppel-1"
My personal contributions to this repo is the "Doppel-1", a new Replica PCB that is somewhat unique among clone boards floating around the internet. This is being done by working off of an imported copy of gerber files for the "PCB-11" replica that I found on [Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files), which were posted originally on a facebook group. The "PCB-11" is, I believe, the most common replica board you will see pictures of online as this is the only replica (that I know of) where the gerbers have been made publicly available. These are often marked on the back in the bottom right with "Apple 1 replica 2012-2016" in soldermasked copper. If a replica board was purchased post-2020, it is likely that it is based on these gerber files, as the Mimeo-1 has been out of production since that time and up unto the time of writing.

The Doppel-1 can be considered a complete native rebuilding of "PCB-11" in KiCad, whereby the board has its own set of custom footprints that are unique to the apple-1, 3d models (where needed) for 3D rendering purposes, native KiCad filled zones, rule areas, Text, and traces, as well as error fixes and fabrication notes for a production-ready PCB. Notable mistakes from the original vary from the file itself to fabrication choices by the customer or the manufacturer. Clarifying remarks have been made to ensure that the PCB is being fabricated to make a reasonable replica. I have made some remarks about my observations so far:

## Design Notes

1) The silkscreen text on the Apple-1 PCB is extremely difficult to reproduce. By all accounts it was hand-stenciled, and I have spent more time than I care to admit comparing uniform-stroke technical typefaces that are meant to replicate leroy lettering or other technical stencil packages that are freely available online, but none of them have quite matched what I have seen on the PCB-11 and on other clones. Trouble characters include "1" (with a top serif only), "4"(closed), "6", and "C". I have found the font "Routed Gothic" to be closest but kerning is not quite there, and it still does not match with the characters aforementioned.

2) The solder pads on the DIP sockets and breadboard area on "PCB-11" are round on both front and back layers, while on original units, the solderpads were actually different on the back side vs the front. On the back they were a squashed oval (basically an obround but the end arcs share a center point with the rectangle), and on the front they were smaller, tangent obrounds. This was most likely done to make it easy to solder while leaving room for trace paths on the front. This is something a lot of replicas miss, and to my knowledge only the Apple-1 Replica shop model has this. I do not know if the Mimeo-1 also has this feature. nevertheless, it is here on this pcb file set!

3) The trace leading to the positive lead between B&C @16 has been adjusted to match the Mimeo-1

4) The trace between C&D @15 leeting to the via below IN914 diode at a 45 degree angle has been moved down slightly to match the Mimeo-1

5) silkscreen outlines for DIP sockets has been increased to a width of 10mils to match what is expected

## Manufacturing Notes:

If you are going to get your own replica board manufactured, read this first:

1) Normally the green finish provided by PCB manufacturers is way too dark. It has become clear to me that it will be almost impossible to replicate near-exact finishes for small volume with any direct-to-customer fabricators. If the fabricator does allow for lighter green finishes and/or matte green, these colors should be selected instead of a "Standard" green.

2) Boards that are finished with hard gold or using an ENIG process (i.e. full-board gold plating) are unable to also accomodate silkscreening on top of non-soldermasked copper. This is extremely evident in the top-right corner of the board where diode markings are missing where the gold is plated over the copper. It is understandable to desire gold for the longevity of the board, but doing so will produce a poor replica. Gold plating should be confined to the edge fingers only, with the rest done in HAL SnPb.

## Why?

Why did I do this? as Mike Willegal said, If you have to ask that question, this project isn't for you. I have had a strange fascination for the Apple-1 ever since I was a kid. I've been drawn to the technical artistry of the board, the simplicity of it, and find the case design around it a very cool method of self-expression.

## Status of the Doppel-1

* Many footprints still need to be designed and assigned to schematic symbols
* Text work is always ongoing and is probably the most time consuming part.
* Due to the change of the dip pad shape and size, there are some pads bleeding into traces on the back


## Contents
For further information on the projects in questions, read the README.md within each directory:

[`/mainboard/`](./mainboard/) - Project folder for the Doppel-1

[`/doc/`](./doc/) - Contains various instruction manuals for building, soldering, wiring, and using the Apple-1 and its various accessories

[`/aci/`](./aci/) - Project folder for rebuilding the Apple Cassette Interface in KiCad

[`/serialboard/`](./serialboard/) - Project folder for rebuilding the Apple Serial Interface in KiCad

[`/transformers/`](./transformers/) - KiCad Schematics for the transformer wiring of the Apple-1

[`/datanetics_modern/`](./datanetics_modern/)- Datanetics Keyboard - Modern Version (Built by [@schlae](https://github.com/schlae/replica-datanetics))

[`/datanetics_original`](./datanetics_original/) - Datanetics Keyboard (Original) (Built by [willegal](https://www.willegal.net/appleii/apple1-datanetics.htm))

[`/software/`](./software/) - A repository of Cassette interface software (.wav) files for use with the Apple-1

[`/fw/`](./fw/) - Copies of wozmon.asm and wozaci.asm firmware files

[`/img/`](./img/) - support image files for various projects

## Other Things to check out

[Apple 1 Riser Card](https://p-l4b.github.io/riser/) - PCB to allow mounting expansion cards horizontally

## Goals and Contributing

If you'd like to contribute, I'm always happy to accept work on anything that makes these files more accurate and complete. For more details, see the `readme.md` file located within each board's folder
### Schematics
- Schematic files need creating for the original Datanetics keyboard and Serial Board


#### Datanetics Keyboard (Modern)
The PCB file requires the installation of the plug-in library for Cherry MX keyswitches
### Gerber Files
Gerbers based on the PCB files have not yet been generated. only the original imported gerbers are located within the respective board's folder

## Future Goals
In the future, once the above goals are met and I'm satisfied with them, I may consider working on an altered version of the main board that, while maintaining the same number and nature of the components, makes adequate substitutes such that another curious hobbyist would be able to buy as many components as possible off-the-shelf without having to hunt for "unicorn" parts. I'd also like to address electrical issues found by various hobbyists relating to stability and performance of the board

I'd like the ability to build one to be cheap and available to anyone who wants to do it, without having to sacrifice much at all in the way of board or schematic integrity. I would also like to provide a BOM that includes all required sockets needed for all the DIP chips in the system


## Acknowledgements

This repository contains only a fraction of original work. mostly, it is an amalgamation of a few different projects related to documenting and reproducing the Apple-1 Computer, with my work being mainly relegated to tying the gerber files and schematics together into a cohesive whole KiCad project. The attributions for the various portions of the project files are in the table above
* I am not sure the original source of the Mainboard PCB gerber files. the Applefritter forum post remarks that they were posted on an Apple-1 enthusiasts facebook group, but I do not have facebook nor would i know how to track down the original post. If anyone can give proper attribution to the files please reach out.

