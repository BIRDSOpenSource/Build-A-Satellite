---
title: For COM Team Members
has_children: true
nav_order: 5
permalink: 'com/guide'
layout: default
lang: en
---

# Guide for COM Team Members
{: .no_toc }

<details markdown="block">
<summary>Table of Contents</summary>

- Table of Contents
{:toc}

</details>

## Introduction and Fundamentals
{:toc}

Understanding CubeSat Communication Subsystems

The main objective is to establish efficient and effective link between the space and the ground segment 
- Provide a link to relay data findings (satellite to ground station) and send commands to the satellite 
- Provide the interface between the satellite and ground systems 
- Receives and demodulates uplink signals and modulates and transmits downlink signals 
- Consist of a transmitter, a receiver, an antenna, and a RF coax cable.
- Relay Payload mission data, and House keeping data 


Overview of RF communication in CubeSats.

Basics of uplink, downlink, and inter-satellite communication.

Overview of BIRDS Communication Design

Key lessons from BIRDS-X, BIRDS-5, and BIRDS-4.

Evolution of communication systems in these projects.

  <p>
    <img alt="birdsx-obc-eps-com-pic-sch" src="/assets/images/birdx-com-detailed-block-diagram.png">
  </p>
*Reference: [BirdsX COM block diagram]*

## Role and Responsibilities of the COM Team
{:toc}


        
  <p>
    <img alt="birdsx-obc-eps-com-pic-sch" src="/assets/images/birdx-obc-eps-com-pic-sch.png">
  </p>
*Reference: [BirdsX OBC/EPS schematic]*


## Satellite Communication Basics
{:toc}
COM Radio Links

|              | Uplink (Receive Mode)     | Downlink (Transmit Mode) | Beacon (CW Mode) |
|:-------------|:------------------        |:------                   | :------|
| Frequency    | 435.313 MHz               | 437.375 MHz              | 437.375 MHz |
| Bandwidth    | 8.5 kHz                   |8.5 kHz                   | 500 Hz |
| Modulation   | GMSK                      | GMSK                     | CW Morse Code |
| Output Power | --                        | 800mW (29.03 dBm)        | 100mW (20 dBm) |
| Rate         | 4800 bps                  | 4800 bps                 | 20 wpm |



## Frequency Selection and Licensing
{:toc}



## Transmitter and Receiver Design
{:toc}



## Antenna Design and Configuration
{:toc}



## Signal Processing and Data Encoding
{:toc}



## Link Budget Analysis
{:toc}



## Testing and Validation
{:toc}



## Documentation and Version Control
{:toc}



## Tools and Resources for COM Teams
{:toc}



-----

[BirdsX OBC/EPS schematic]: https://github.com/BIRDSOpenSource/BIRDSX-COM/blob/main/COMPIC_SCH/new_obc_eps_birds_x_v4.pdf
[BirdsX COM block diagram]: https://github.com/BIRDSOpenSource/BIRDSX-COM/tree/main/Diagram