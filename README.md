# About
This repository is a central collection and improvements to various Apple-1 clone projects I've found around the internet. I have a particular fascination for the original Apple-1 and Datanetics Keyboard, so primarily I have compiled gerber files, kicad projects, instructions, and BOMs for how to build your own Apple-1 Clone as accurately as possible.
## Contents & Progress

| Component                     | Author                |Schematic  | PCB File  |Gerbers    |3D Model| BOM File |
|-|-|-|-|-|-|-|
| [`/mainboard/`](./mainboard/)     | Schematics:[@nicolas-robin](https://github.com/nicolas-robin/a1_schematics) Gerber Files:[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)   |Y|WIP|Y (unlinked to pcb)|N|Y|
| [`/aci/`](./aci/)                  |[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |N|Y (unlinked to pcb)|N|
| [`/serialboard/`](./serialboard/) |[Applefritter Forums](https://www.applefritter.com/content/apple-1-replica-gerber-files)|N|WIP |Y (unlinked to pcb)|N|N|
| [`/transformers/`](./transformers/)                |Schematics:[@nicolas-robin](https://github.com/nicolas-robin/a1_schematics)|N/A|N/A |N|N|N|
| [`/kb_datanetics_modern/`](./kb_datanetics_modern/)- Datanetics Keyboard - Modern Version  |[@schlae](https://github.com/schlae/replica-datanetics)|Y|Y| Y (linked)| N|Y|
| [`/kb_datanetics_original](./kb_datanetics_original/) - Datanetics Keyboard (Original)|[willegal](https://www.willegal.net/appleii/apple1-datanetics.htm)  |Needed | WIP|Y (unlinked to pcb)|N|N|

## Goals and Contributing

If you'd like to contribute, I'm always happy to accept work on anything that makes these files more accurate and complete. For more details, see the `readme.md` file located within each board's folder
### Schematics
- Schematic files need creating for the original Datanetics keyboard and Serial Board


#### Datanetics Keyboard (Modern)
The PCB file requires the installation of the plug-in library for Cherry MX keyswitches
### Gerber Files
Gerbers based on the PCB files have not yet been generated. only the original imported gerbers are located in the project.

## Future Goals
In the future, once the above goals are met and I'm satisfied with them, I may consider working on an altered version of the main board that, while maintaining the same number and nature of the components, makes adequate substitutes such that another curious hobbyist would be able to buy as many components as possible off-the-shelf without having to hunt for "unicorn" parts. I'd like the ability to build one to be cheap and available to anyone who wants to do it, without having to sacrifice much at all in the way of board or schematic integrity. I would also like to provide a BOM that includes all required sockets needed for all the DIP chips in the system


## Acknowledgements

This repository contains only a fraction of original work. mostly, it is an amalgamation of a few different projects related to documenting and reproducing the Apple-1 Computer, with my work being mainly relegated to tying the gerber files and schematics together into a cohesive whole KiCad project. The attributions for the various portions of the project files are in the table above
* I am not sure the original source of the Mainboard PCB gerber files. the Applefritter forum post remarks that they were posted on an Apple-1 enthusiasts facebook group, but I do not have facebook nor would i know how to track down the original post. If anyone can give proper attribution to the files please reach out.

