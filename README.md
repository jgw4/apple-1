# About
This repository is a collection of different projects I've found around the internet relating to building a near-exact clone of the Apple-1 computer. My intention is for it to act as a central repository for information that may otherwise be obscure or decentralized. For aspiring builders, having everything in one place helps with prep work, troubleshooting, and familiarizes with the scope of the project.

My personal contributions to this repo is the creation of a set of clone boards based in KiCad, that are fully editable and can be turned into production-ready gerbers. This was done by importing an existing set of gerber files found on applefritter/willegal, and essentially "decompiling" the imported geometry into matching custom footprints, and KiCad Native features. Work on these PCBs is ongoing, but the source gerbers are available in this repository also.

## Contents & Progress

| Component                     | Author                |Schematic  | PCB File  |Gerbers    |3D Model| BOM File |
|-|-|-|-|-|-|-|
| [`/mainboard/`](./mainboard/)     | Schematics:[@nicolas-robin](https://github.com/nicolas-robin/a1_schematics) Gerber Files:[Applefritter Forums/Facebook?](https://www.applefritter.com/content/apple-1-replica-gerber-files)   |Y|WIP|Y (unlinked to pcb)|N|Y|
| [`/aci/`](./aci/)                  |[Applefritter Forums/Facebook?](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |N|Y (unlinked to pcb)|N|
| [`/serialboard/`](./serialboard/) |[Applefritter Forums/Facebook?](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |Y (unlinked to pcb)|N|N|
| [`/transformers/`](./transformers/)                |Schematics:[@nicolas-robin](https://github.com/nicolas-robin/a1_schematics)|N/A|N/A |N|N|N|
| [`/datanetics_modern/`](./datanetics_modern/)- Datanetics Keyboard - Modern Version  |[@schlae](https://github.com/schlae/replica-datanetics)|Y|Y| Y (linked)| N|Y|
| [`/datanetics_original`](./datanetics_original/) - Datanetics Keyboard (Original)|[willegal](https://www.willegal.net/appleii/apple1-datanetics.htm)  |Needed | WIP|Y (unlinked to pcb)|N|N|

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

