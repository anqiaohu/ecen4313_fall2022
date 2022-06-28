# ECEN 4313 Lab: Open Source Analog IC Design
A three-part lab for undergraduate students to learn open source analog. Designed for
ECEN 4313: Linear Electronics Circuit Design at Oklahoma State University (Fall 2022)

## Pre-Lab: Open Source Tool
Tutorials to be added.
1. GitHub
2. xschem
3. ngspice

## Lab 1: CS Stage

Design Specifications.

| Specifications | Min | Typ | Max | Unit |
| ---------| ------| -------|-------|-----|
| VDD  |  1.7   |  1.8   |  1.9   |  V   |
| DC gain | 20  |      |    |  dB |
| Output swing |    | 600   |    |  mV |

### Report Requirements
1. Report transistor sizing (W,L) and ideal voltage/current source bias conditions.
2. Share the path to your public repository on GitHub.

## Lab 2: Single stage OTA design

Design specifications. Try to meet as many specs as possible at the TT corner.

| Specifications | Min | Typ | Max | Unit |
| ---------| ------| -------|-------|-----|
| DC gain | 20  |      |    |  dB |
| UGF    |  10   |     |     |  kHz   |
| IQ    |     |  50   |     |  uA |

### Report Requirements
1. Report transistor sizing (W,L) and ideal sources if any.
2. Share the path to your public repository on GitHub.

## Lab 3: Folded-Cascode 

Design specifications TBD. Try to meet as many specs as possible at the TT corner.

## Lab 1.1: Current Mirror

This lab is an intermediate step between Lab 1 and 2. We will use this lab
to try out a unified design flow in Google Colab from schematic entry to post-layout simulations.

**Objective**: We will design a basic two-transistor NMOS current mirror with minimal area to meet
the specs. See the schematic in Fig. 1.



Design Specifications: Meet as many specs as possible across process, voltage,
and temperature (PVT) variations and global and local mismatch. 
* Process corners: FF, SS, SF, FS, TT
* Temperature: -40C, 25C, 125C
* $V_{OUT}$: 0.3, 0.6, 0.8 V
* Monte Carlo simulation $N>100$.
* Min, max for $I_{OUT}$ based on $3\sigma$, i.e., $I_{OUT,avg} - 3\sigma >$ Min and $I_{OUT,avg} + 3\sigma <$ Max. 

| Specifications | Min | Typ | Max | Unit |
| --------- |  ----- | ------ | ------ | ----- |
| $I_{REF}$  |      |  1    |     | $\mu A$  |
| $I_{OUT}$ |  9    |  10   |  11  | $\mu A$  |

### Report Requirement / Grading Rubric

Report the size (W/L) and the total layout area ($\mu m^2$). The more compact design that meets all specs will receive a higher grade.

