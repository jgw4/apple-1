# Serial Board
# Prerequisites

The PCB File is being made by importing gerber files first into KiCad, and mapping the schematics to it by applying footprints to the symbols, placing over the gerber geometry, and then removing the import gerber geometry

# To Do
## Schematics
- a schematic is needed for the serial board
## PCB
- assign accurate pin mappings to all component footprints
- place footprints in their exact spot on the PCB.
- remove any duplicate layer geometry from laying the footprint over the gerber imported layers.
- re-attach all traces/nets to the footprints
- ultimately, passing a 0 error/0 warning DRC check

