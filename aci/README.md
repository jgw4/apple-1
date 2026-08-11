# Cassette Interface

The Apple Cassette Interface "ACI" card has been completely reverse-engineered in KiCad 10, with linked KiCad and schematic files, which output production-ready gerber files and a fully-populated step file of the card with components.


The PCB File was made by importing gerber files for "PCB-07" first into KiCad, and mapping the schematics to it by applying footprints to the symbols, placing over the gerber geometry, and then removing the import gerber geometry

The Board is 100% complete and ready for production. gerber files are available in the /gerbers/ folder

## Changes from PCB-07

* the soldermask on the gold contact fingers has been extended slightly upward into the full board width
* pads have been redone from circles to ovals/ squashed obrounds in the same style as /mainboard
* the inside corner between the edge connector and the card was sharp, it is now radiused to reflect the original

## Known deviations from the original
* there is no manufacturer logo on the part as of now.
* I have not done enough research on this card yet to determine if this is a 1st rev version or a second rev version. I would like this card to be the second revision if it is not already.

## Ordering
* as with the mainboard, make sure to order soldermask in a matte or light green finish
* there are some silkscreen remnants on the KiCad file, but they are not to be used in production. Do not send silkscreen files to the Manufacturer!
* For the most historical accuracy, specify hard gold on the edge connector. It adds cost, but 