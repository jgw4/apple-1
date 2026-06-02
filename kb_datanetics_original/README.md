# Original Datanetics Keyboard
This board is a trace-for-trace copy of the original Datanetics keyboard, created by willegal. It contains all the flaws of the original board and requires a wire jumper to make work correctly. For more info, see the [Datanetics Keyboard Reproduction.dotx file](/doc/Datanetics%20Keyboard%20Reproduction.docx).

I would personally recommend using the modern keyboard, as it has been slightly altered to use Cherry MX keyswitches, fixes the board's mistakes, has prewritten firmware, and takes advantage of a modern ATMega644P microcontroller that is easier to obtain. If you instead want the most historical accuracy, this would be the folder to use.
# Prerequisites

The PCB File is being made by importing gerber files first into KiCad, and mapping the schematics to it by applying footprints to the symbols, placing over the gerber geometry, and then removing the import gerber geometry

# To Do
## Schematics
- Schematics need created for the board. the source software file is a .osm file that i don't know how to open.
- footprints need assigned to all components within all schematic files. this in most cases require the creating of custom footprints to ensure reproduction accuracy
## PCB
- assign accurate pin mappings to all component footprints
- place footprints in their exact spot on the PCB.
- remove any duplicate layer geometry from laying the footprint over the gerber imported layers.
- re-attach all traces/nets to the footprints
- ultimately, passing a 0 error/0 warning DRC check

