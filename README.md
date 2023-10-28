# Eurorack-PSU
This repository has the KiCAD design files for my +12/-12V Eurorack PSU PCB. It also includes the BOM, CPL, and compressed GERBER files to order directly from a PCB Fab.

## Schemetic Design

![image](https://github.com/JacobParent7/Eurorack-PSU-/assets/105901480/8efcebb9-f54d-45e0-b2d8-d591e7b11a28)

## Footprint Design

![image](https://github.com/JacobParent7/Eurorack-PSU-/assets/105901480/083ee302-c9da-422e-bead-0cb98824cdaa)

## Design Description
This design utilizes a wall wart AC/AC converter which provides a 15V AC signal to the board. The board then rectifies this signal into its positive and negative parts and filters the rectified signals to a max ripple of 1V, as per tolernace of the voltage regulators inputs. This filtered signal is sent to two voltage regulators which have high frequency tantalum compensation capacitors. These regulators directly provide the -12/+12V rails. 
