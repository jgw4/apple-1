This repository is a collection of different projects I've found around the internet relating to building a near-exact clone of the Apple-1 computer, as well as the home of the "Doppel-1" replica Apple-1 PCB. My intention is for it to act as a central repository for information that may otherwise be obscure decentralized, or link rot in the future. For aspiring builders, having everything in one place helps with prep work, troubleshooting, and familiarizes with the scope of the project.

## Contents
For further information on the projects in questions, read the README.md within each directory:

[`/mainboard/`](./mainboard/) - Project folder for the Doppel-1

[`/doc/`](./doc/) - Contains various instruction manuals for building, soldering, wiring, and using the Apple-1 and its various accessories

[`/aci/`](./aci/) - Project folder for rebuilding the Apple Cassette Interface in KiCad (Complete)

[`/serialboard/`](./serialboard/) - Project folder for rebuilding the Apple Serial Interface in KiCad

[`/graphicard/`](./graphicard/) - Mirror and minor alteration of the original P-L4B graphics card [here](https://p-l4b.github.io/graphic/) based on the Texas Instruments VDP TMS9918A. It has been modified cosmetically to look more similar to the Apple Cassette Interface. This project is licensed under CC BY 4.0 by the creator.

[`/protoboard/`](./protoboard/) - Mirror and minor alteration of the original P-L4B proto board [here](https://p-l4b.github.io/proto/). It has been modified cosmetically to look more similar to the Apple Cassette Interface. This project is licensed under CC BY 4.0 by the creator.

[`/risercard/`](./risercard/) - Mirror and minor alteration of the original P-L4B riser board [here](https://p-l4b.github.io/riser/). It has been modified cosmetically to look more similar to the Apple Cassette Interface. This project is licensed under CC BY 4.0 by the creator.

[`/datanetics_modern/`](./datanetics_modern/)- Datanetics Keyboard - Modern Version (Built by [@schlae](https://github.com/schlae/replica-datanetics))

[`/datanetics_original`](./datanetics_original/) - Datanetics Keyboard (Original) (Built by [willegal](https://www.willegal.net/appleii/apple1-datanetics.htm))

[`/software/`](./software/) - A repository of Cassette interface software (.wav) files for use with the Apple-1

[`/fw/`](./fw/) - Copies of wozmon.asm and wozaci.asm firmware files

[`/img/`](./img/) - support image files for various projects

## Other Things to check out

[P-Lab Projects](https://p-l4b.github.io) - Hosts various neat expansion cards and mods for the apple-1, such as a Wi-Fi Card, SD Storage card, riser card, sound card, Video card, various IC replacement boards, expansion port breadboards, and much more. Really cool stuff!

[Erik's Ponderings - Building an Apple-1](https://blog.bruchez.name/posts/apple-1-reproduction-part-1-components/) - Erik Bruchez documented his process of building an exceptional Apple-1 clone in great detail, including some great tips for power supply building, adding more decoupling capacitors, mechanical tips, and more. Really neat to check out, especially before you build one of your own

## Goals and Contributing

If you'd like to contribute, I'm always happy to accept work on anything that makes these files more accurate and complete. For more details, see the `readme.md` file located within each board's folder

### Schematics
- Schematic files need creating for the original Datanetics keyboard
### Gerber Files
Gerbers based on the PCB files have not yet been generated. only the original imported gerbers are located within the respective board's folder

## Future Goals
In the future, once the above goals are met and I'm satisfied with them, I may consider working on an altered version of the main board that, while maintaining the same number and nature of the components, makes adequate substitutes such that another curious hobbyist would be able to buy as many components as possible off-the-shelf without having to hunt for "unicorn" parts. I'd also like to address electrical issues found by various hobbyists relating to stability and performance of the board

I'd like the ability to build one to be cheap and available to anyone who wants to do it, without having to sacrifice much at all in the way of board or schematic integrity. I would also like to provide a BOM that includes all required sockets needed for all the DIP chips in the system


## Acknowledgements

This repository contains only a fraction of original work. mostly, it is an amalgamation of a few different projects related to documenting and reproducing the Apple-1 Computer, with my work being mainly relegated to tying the gerber files and schematics together into a cohesive whole KiCad project. The attributions for the various portions of the project files are in the table above
* I am not sure the original source of the Mainboard PCB gerber files. the Applefritter forum post remarks that they were posted on an Apple-1 enthusiasts facebook group, but I do not have facebook nor would i know how to track down the original post. If anyone can give proper attribution to the files please reach out.

