## Members
Corey Ahl, Computer Engineering Student (Sophomore)
corahl@vt.edu
Lauren Castro, Computer Engineering Student (Sophomore)
lacastro@vt.edu

## Mentor
TBD

## Current Status
WAITING FOR APPROVAL

## Project Overview

The goal of the project is to create a version of [Nicholas L. Johnson's flip-card](https://github.com/Nicholas-L-Johnson/flip-card), which is a custom PCB in the form of a business card that runs a fluid impact particle simulation based on accelerometer data. This is displayed on a charlieplexed 21x21 LED array.

The working exanple of Cicholas Johnson's card is shown below:

![project-demonstration](https://github.com/WebTWJ/corahl-project-amp/blob/main/project-demonstration.gif)

We propose one main change to the Nicholas Johnson's project, running the fluid simulation on an FPGA instead of the microprocessor used originally, an RP2350.

### Design Overview (my plan going in)
FPGA Programming
- Do this first to get an idea of the LUT/Log Element requirements for the simulation
- Plan on using an Xilinx Arty-A7 development board
Choosing Materials
- Choosing the FPGA
    - Ideally a low IO count. The minimum for charlieplexing is 22, and the minimum for multiplexing is 42. The amount for the accelerometer (LIS2DH12TR) is 12. The amount the original project uses is 60 (the full amount of the RP2350)
    - Ideally a non BGA package, preferably QFP or LQFP (for easier attachment and lower PCB cost)
    - Enough LUTs/Logic Elements to run the simulation
    - Ideally non-volatile
- Will probably stick with the same LEDs used for the original project, 0402 LEDs.
- Will probably stick with the same accelerometer as the original project, an LISDH12TR

PCB Design

## Educational Value Added

This project is expected to cover aspects of PCB design, data processing, CAD, and general coding. A custom PCB is expected to have to be made due to the need for minimal size with given components, data processing will be needed to translate raw data from the pen to vector format, and general coding will be needed to turn the processed data into a readable format. CAD design will most likely be needed as well for the pen body.

## Tasks
<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Design Decisions

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Design Misc

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Steps for Documenting Your Design Process

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## BOM + Component Cost

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Timeline

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Useful Links

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Log

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->
