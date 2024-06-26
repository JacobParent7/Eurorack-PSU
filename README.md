# Eurorack-PSU
This repository has the KiCAD design files for a simple +12/-12V Eurorack PSU PCB. It also includes the BOM, CPL, and compressed GERBER files to order directly from a PCB Fab.

## Schematic Design

![image](https://github.com/JacobParent7/Eurorack-PSU-/assets/105901480/8efcebb9-f54d-45e0-b2d8-d591e7b11a28)

## Footprint Design

![image](https://github.com/JacobParent7/Eurorack-PSU-/assets/105901480/083ee302-c9da-422e-bead-0cb98824cdaa)

## Design Description
This design utilizes a wall wart AC/AC converter which provides a ~17Vpp AC signal to the board. The board then rectifies this signal into its positive and negative parts and filters the rectified signals to a max ripple of 1V for the inputs of both regulators. This filtered signal is sent to two voltage regulators which have high frequency tantalum compensation capacitors. These regulators directly provide the -12/+12V rails. The LM7812 does not have a built in protection diode so that is why it's included.

![IMG_20231113_154112](https://github.com/JacobParent7/Eurorack-PSU/assets/105901480/92d30cf9-9e76-4124-9e80-d23b5c7c602d)

