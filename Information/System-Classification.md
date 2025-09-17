>[!note]
> this file is not completed and will be worked on constantly!

| Section Title | Rundown |
| -------| ------- |
| [Introduction](#Introduction) | Self explanatory |
| [Terminology](#Teriminology) | Terminology for systems, diagrams, etc. |
| [Reactor Specs](#Reactor-Specificatiobs) | Specifications and general information for the nuclear reactor |
| [Annunciators](#Annunciator-Guide)| a Guide that explains how Annunciators are labeled, how to refer to indications on annunciators, ad annunciator types|

# Introduction
This document is intended to help explain what different parts of the reactor, documents, and other things that may be unclear.
This document will contain Teriminology, Mechanics, Design ideas, and more!

# Terminology
Below is a list of Terms, Information about the term, and Abbreviation if applicable.
|Term|Info|Abbreviation|
|----|----|------------|
|CR|Control Rod|
|PCR| Primary Control Rod|
|SCR| Secondary Control Rod|
|TCR| Tertiary Control Rod|
|QCR| Quaternary Control Rod|
|ECR| Emergency Control Rod|
|EOP| Emergency Operating Procedures|
|SOP| Standard Operating Procedures|
|SSOP|Standard Startup Operating Procedures|
|MWt| Megawatt Thermal. it's the reactors energy output|
|Void| fancy way to say steam bubbles|
|RX| Received signal|
|TX| (rarely used) Transmit Signal|


# Reactor-Specifications

Reactor specs:
- BWR
- Recirculation Loops: 2
- Water pumps: 3
- Turbines: 2
- Max Rated Power (in MWt): 4800
- Positive temperature Coefficient
- Positive Void Coefficient
- probably a pain to operate: true

> [!tip]
> Control Rod information can be found in [this](https://github.com/RandomVOTVplayer/Goober-Generating-Station/blob/RandomVOTVplayer-patch-1/Information%2FRod-Layout.md) document!


Level zones:
9 meters ( 354 Inches) - RCIC, LPCI, and Pumps 1 and 2 trip

8 meters ( 314 Inches) - High-High water level warning

7 meters ( 275 inches) - High Water Level warning

4 - 6 Meters (157 inches to 236 inches) - Standard Operating Level

3 meters (118 inches) - Low water level warning

2 meters (78 inches) - Reactor Trip and automatic RCIC actuation, Diesel Generator Auto actuation (unless bypassed)

1 meter (39 inches) - MSIV closure and turbine trip

0 meters (FUEL RANGE) - Meltdown begins in 2 minutes

> [!WARNING]
> if water level is in the fuel range for too long, a Meltdown will start. signs of a full meltdown and partial meltdown will begin to appear after 30 seconds to a minute. See the below information about meltdowns.

## signs of a partial meltdown
- Control rods stuck
- temperature consistently above 1200°F
- temperature gauge cannot maintain a stable temperature
- Feedwater Pumps struggle to maintain a reactor level
- the following annunciators all are receiving an ignition signal
    - CONT_RAD_HI (Radiation > 50 mSv/h)
    - PRIM_CIRC_RAD_HI (Radiation > 15 Sv/h)
    - SEC_CIRC_RAD_HI (Radiation > 5 mSv/h) (only triggers in full meltdown. usually)
    - RECIRC_CAVITATION_[pumps 1 or 2]
    - MSIV_ISOL_SINGLE_RX (based on many conditions. only one condition in the list has to be met for the isolation single to be triggered. theblist can be found here[link coming soon])
- Reactor pressure cannot be maintained properly 
- Reactor power cannot be controlled

# Annunciator-Guide
> [!note]
> not ready yet