# Mainboard
# Prerequisites

To properly view the pcb file's text elements, please download and install "Routed Gothic" font located in `/doc/`. This is the closest match I have found to the original PCB lettering in font form and is based on the Leroy stenciling system common with draftsman before computer fonts.

The PCB File is being made by importing gerber files first into KiCad, and mapping the schematics to it by applying footprints to the symbols, placing over the gerber geometry, and then removing the import gerber geometry

# To Do
## Font
I am currently using routed Gothic font, but I believe Iwater GMaru Gothic Pro is a better match to the original. problem characters include the number 1, letter C,and the number 4
## Schematics
- footprints need assigned to all components within all schematic files. this in most cases require the creating of custom footprints to ensure reproduction accuracy
## PCB
The gerber files were noted to have differences from the original in the forum posts, namely:
- The original has a matte finish, this one has a sligtly brighter green.
- The silkscreen doesn't cover the plated areas without soldermask.
- The DIP and breadboard solder pads should be wider although it only really matters in the breadboard area.
- The video adjustment pot pads are  narrower by 0.025", making it difficult to insert the trimpot.
- assign accurate pin mappings to all component footprints
- place footprints in their exact spot on the PCB.
- remove any duplicate layer geometry from laying the footprint over the gerber imported layers.
- re-attach all traces/nets to the footprints
- ultimately, passing a 0 error/0 warning DRC check

