# Datanetics Keyboard Reproduction

Extracted from `doc/Datanetics Keyboard Reproduction.docx`.

(Available from Willegal.net)

![](/img/dmbuildman-01.png)

## Build Guide

(Draft-2)

# BOM with suppliers

Note: Some suppliers have order minimums, this does not account for that.

Part ID | Description | Vendor | Part# | Optional Part #
--- | --- | --- | --- | ---
| 40 pin Socket (white) | Mouser | NA | | 
| TI 14 pin Socket- Qty 2 | Mouser | NA | |
M2 | 555 Timer (Fairchild) | Mouser | NA |-
M3 | 555 Timer (Fairchild) | Mouser | NA | 
M1 | MM5740 AAE | Expediters | NA | MM570AAF
M4 | 7404 TTL (National Semi) |  |  | 
M5 | 7404 TTL (TI) |  |  | 
R1 | 100 ohm |  |  | 
R2 | 100 ohm |  |  | 
R3 | 360 ohm |  |  | 
R4 | 3.6k ohm |  |  | 
R5 | 510k ohm |  |  | 
R6 | 30k ohm |  |  | 
R7 | 3k ohm |  |  | 
C1 | 250 pf |  |  | 
C2 | .01uf ceramic disc |  |  | 
C3 | .68uf tantalum |  |  | 
-- | Eyelets #27 qty - 4 | Mouser | 534-27 | 
-- | Eyelets #26 qty-10 | Mouser | 534-26 | 
-- | Edge connector -30 pin | Digikey | EBM15DSEH | 
-- | 16 pin Dip Connector | Mouser |  | 151-2P16-E
-- | 16 connector rainbow ribbon cable (by foot) | Mouser | 517-3302/16 | 

Note: You will also need 54 key switches from an Apple II Datanetics keyboard and keycaps, plus the following extra keycaps (if you do not have custom keycaps made)

L, U, V, O, X, I, and an extra “Arrow” key.

Note: These keys will be turned on their side, so you must use keycaps for the bent Datanetics key switch and not for the later Apple II keyboards.

# Special Tools Required

Pin Vise (available at Hobby Lobby, Michaels or your local hobby shop)

#64/#67 Drill Bit .036”

Temperature Controlled Soldering Iron (with solder)

1/16 Eyelet Setting tool

# Keyboard Brackets

If your kit did not include keyboard brackets, they will need to be fabricated and either powder coated black semi-gloss or spray painted with paint that includes a metal primer.

Here is the dimensions are per Willegal.net

![](/img/dmbuildman-02.png)

# Schematics

![](/img/dmbuildman-03.png)

# Notes on the keyboard encoder

The MM5740 encoder is static sensitive and difficult to find. There are multiple types of the MM5740 encoder. The original was an MM5740AAE which supports N-Rollover. However the Datanetics keyboard does not implement this feature. The same mapping is available in a 2 key rollover in MM5740AAF. This is more easily found.

There are cases of mislabeled MM5740 encoders that do no map to the correct type. If you get a bad mapping it may not be your keyboard. You will need to try another encoder from a different lot. Additionally there have been cases of encoders which work in Apple II Datanetics keyboards and should work in this keyboard design, but do not.

# Reaming/Drilling out the matrix

The original Datanetics keyboard contains a matrix of vias that are not plated completely through (these are the red areas in the schematics). The matrix is used to either re-map the unused keyswitches by inserting a small bare wire and soldering on both sides of the PCB.

The Datanetics reproduction uses standard via, to replicate this so you need to manually ream/drill out each hole in the matrix

Tips:

The matrix vias are plated through and must be drilled out to eliminate connectivity between top and bottom copper layers

This step must be done carefully or you risk delaminating the copper pads

The holes are drilled undersize, to .026 mils dimension, you should drill them out to about .036 mils (1/32" drill bit will do)

Use a sharp drill bit, in order to reduce risk of delaminating pad

It is recommended to ream/drill partway through from each side, to reduce the possibility of delaminating pad

Check connectivity after drilling out with an ohm-meter (not continuity tester) to ensure that the connectivity is removed between the copperaround the holes between sides.

# Attaching The Brackets

Attaching the brackets requires drilling holes to match the PCB in the metal brackets. This is an easy task to make a mistake with.

To drill the holes you will need to initially attach the side brackets with a minimum of 2 eyelets (I suggest on the side brackets to use the last hole on the “bar” that is on the edge connector side of the board and the second to last hole on the other side). If you can, use a fine silver sharpie so you can see the mark to indicate where to drill but holding the bracket in position and using the sharpie though the hole. After marking the two holes, then using a sharp 1/16” drill bit place the brackets on a supporting block of wood and drill the holes.

Now attach the brackets to the PCB using the smaller eyelets and the eyelet tool. I recommend attaching from the front side of the keyboard, if you use the tool from the back you will need to support the bracket and possibly need a second set of hands. The eyelet tool is like a small spring weighted hammer and which will crush the eyelet end. Be careful it is in position and does not jump or it will “dent” the paint on the brackets and you will have to touch them up later.

Use the smaller eyelets to attach the sides. The two longer eyelets are for the overlap with the stiffener on the bottom of the keyboard with the side brackets.

![](/img/dmbuildman-04.png)

After initially attaching the sides, drill the rest of the holes and use eyelets to attach.

Repeat this entire process to attach the stiffener. Remember the longer eyelets are for the four holes what will overlap with the side brackets.

![](/img/dmbuildman-05.png)

![](/img/dmbuildman-06.jpeg)

# Fixing the intentional trace mistake on the reproduction

![](/img/dmbuildman-07.jpeg)

On the front of your PCB you will notice an intersection traces in the lower area of the front of the PCB just to the left of center.

You will need to use a sharp hobby knife or box cutter and score both sides if the trace as shown in the picture above. You need to score it to break the connection.

Then using a small piece of wire jumper over the trace as shown the picture. This jumper will be hidden underneath the keys when the keyboard is complete, but maintains originality.

# Installing the soldered components

![](/img/dmbuildman-08.png)

Installing the soldered components is the easiest part of the keyboard build. You will not install the key switches at this point, but all other components will be installed.

Simply follow the schematic and the part ID from the BOM in this document to place the components. Note: The 555 timers are soldered directly in.

Pay close attention to the “dot” that indicates pin one of each component. Note: Resistors and capacitors in this project are not polarized, but for ascetics, you will want all the resistors tolerance bands to point in the same direction (i.e. Gold Band).

# Making the keyboard to Apple-1 cable

![](/img/dmbuildman-09.png)

The most difficult task of the Datanetics keyboard build is to create the cable to connect the keyboard to the Apple-1. Using a rainbow 16 wire ribbon cable makes the implementation easier to keep track of.

![](/img/dmbuildman-10.png)

In these instructions it will be assumed that you are using a colored ribbon cable with has 10 unique colors.

The color pattern is assumed to be the following listed in order of appearance with pin.

![](/img/dmbuildman-11.png)

Pin | Color
--- | ---
16 | Brown
1 | Red
15 | Orange
2 | Yellow
14 | Green
3 | Blue
13 | Purple
4 | Grey
12 | White
5 | Black
13 | Brown 2
6 | Red 2
14 | Orange 2
7 | Yellow 2
13 | Green 2
8 | Blue 2

![](/img/dmbuildman-12.png)

To build the cable you will need to first separate using a sharp knife blade the individual wires on one side of the cable. You will need to go back about 6” into the cable to give you enough room to make clean connections. If you are comfortable building the cable (i.e. this isn’t your first) you may go shorter.

A note on cable length, you may experience issues with a keyboard cable in excess of 24”.

On each wire strip off about ½ inch of plastic sheathing so that you can loop them around the eyelets on the connector before soldering. Follow the instructions below to hook up the wires. Note: You may wish to put small pieces of heat shrink tubing on the wires before you solder them to prevent potential shorts later. When you have completed the cable you can slide the tubing over the eyelets and heat them with a hair dyer or heat gun.

Hint: Put a small drop of white model paint using a tooth pick on the PCB and on the edge connector to mark pin #1.

Connector Pin | Cable wire | Cable Color
--- | --- | ---
1 TOP | 11 | Brown 2
2 TOP | 7 | Yellow 2
3 TOP | 6 | Red 2
4 TOP | 2 | Yellow
5 TOP | 5 | Black
6 TOP | 4 | Grey
7 TOP | 3 | Blue
8 TOP | 1 | Red
4 BOTTOM to 9 BOTTOM | 15 & 16 | Brown
11 TOP | 14 | Green
12 TOP | 8 | Blue 2
15 TOP to 9 TOP | 9 | Green 2
8 BOTTOM | 12 | White

When you have completed wiring up the connector you can then attach the 16-pin dip connector to the end of the ribbon cable. If you do not have a panavise, you can use an old IC socket or proto-perf board to protect the pins and a block of wood to push the connector together. Note: Make sure your ribbon cable is strait and lined up with the connections inside of the connector before you crush it closed.

Using a continuity tester verify the cable matches the chart and that pins on the 16 pin DIP across from each other are not accidently shorted.

# Testing the initial configuration/Stuffing sockets

![](/img/dmbuildman-13.jpeg)

To initially test your keyboard, plug in the MM5740 and the two 7404s.

You will need to check for hot chips.

Using a jumper wire, short the clear screen pads and then reset your Apple-1 by shorting the reset pads with a spare piece of wire. Note the positions of the Reset and clear buttons in the picture below. You will need to locate these pads to short.

![](/img/dmbuildman-14.png)

After clearing screen and resetting, Go through the keyboardshorting each pair of pads making sure that each key works, than as in the picture below, jumper the shift key and checked that shift characters work (i.e. numeric keys). You may also with to test the repeat function.

![](/img/dmbuildman-15.jpeg)

If you get strange results, you need to check that you do not have partial connections in the matrix that was drilled or reamed out. Remember to use an ohm meter and not a continuity tester.

Installing the Keyswitches

![](/img/dmbuildman-16.png)

Installing keyswitches is strait forward, though I suggest getting a set of test clips and a continuity tester and verify each keyswitch works before installing. If the switch does not work, you can try using 99% isopropyl alcohol and an eyedropper to put some solution in the switch and work it in using a needle nose pliers working the stem up and down about 100 times. Then check continuity, Repeat this at least 2-3 times until the switch works, then let it dry. If after that has been performed it still does not work you will need a replacement. If you switch simply sticks, you may try the same process by use DeOxit #5 spray instead of the alcohol and eyedropper. You will need to let the switch dry to determine if it works when using DeOxit.

To install the switches push them into the holes, if the hole is tight you can slight expand the hole with a drill bit, though I would suggest just rocking it in carefully. Then insert the screw into place from underneath. After you have filled all the keys, then flip the board over and solder the switches. Use a temperature-controlled soldering iron and don’t heat the switches up too much so they won’t melt internally.

# Complete Keyboard Test

![](/img/dmbuildman-17.png)

Now you can perform a complete test. Optionally you can skip ahead to the keycap layout and then skip back and test the keyboard.

First test each key, then test the shifted keys (numeric) and verify the expected characters are displayed. Next test the repeat key. It should only repeat once unless you hold down the key to repeat and the repeat key.

# Keycap layout

![](/img/dmbuildman-18.png)

Follow the pattern above to install the key caps. To install the space bar, there are two hinge brackets for the spacer’s metal torsion bar. You may need to adjust which hole the bar goes though.

<INSERT SPACE BAR PIC HERE>

# Adding the Underscore character using the matrix (optional)

While the “RubOut” key on the Datanetics keyboard appears to create an underscore, the WOZ monitor for deletion of a character does not use the actual rubout character. You require an actual underscore, which is key code 0x5F.

To produce this character on the Datanetics keyboard you will need to connect line X4 of the matrix to one lead of a blank key switchand Y3 to the other lead of the same key switch.

To create an underscore character, you will need to hold down the shift key when pressing the new underscore key, there is no way to avoid this requirement.

<INSERT PIC HERE>

![](/img/dmbuildman-19.png)

