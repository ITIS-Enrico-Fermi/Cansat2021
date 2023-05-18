# Cansat 2021

A project by sCANSATi team.

<p align="center">
  <img width="50%" src="images/logo.png" />
</p>

_Awarded Highest Technical Achievement in the European Cansat Competition of 2021_

## Description

A Cansat is a small probe (its dimensions are roughly those of a soda can) that is launched from an altitude of 1000
meters. Cansats usually carry out a scientific mission onboard during their descent, and communicate with the ground
station via a radio link.

Our mission was built around three goals: carry out an environmental analysis, a bacteriological sampling of the air
and proof-test LoRa for roaming and long range communications.

## Design

The can was entirely designed from scratch by the team. Its outer shell was 3D printed in ABS plastic.
Custom hardware was designed to achieve the different goals: temperature measurement, absolute positioning and
handling of sensors on board. Every component was fitted on a custom printed circuit board, also designed by us.

## Hardware and software

An ESP32 is the core component of our small can: its job is to handle data coming from each sensor, and send it to
the ground station via a radio link.
Using FreeRTOS and ESP-IDF, we custom tailored a software for our needs and to exploit the full power of the ESP32
(which is a very powerful dual-core microcontroller).

To find out more on the software side, we published our source code. Feel free to take a look at
[cansat_firmware](https://github.com/ITIS-Enrico-Fermi/cansat_firmware).

## National Flight Competition

The first step of the competition is the _National Flight_. Three teams from Italy competed to pass on to the
European Competition.

This flight validated our design. Data gathered from the National Flight Competition is available in this repository
in the [flight.csv](data/flight.csv) file.

## European Competition

Unfortunately the European Competition took place online solely. The judges presented us a new challenge based on
the flaws they found on our project from the National Competition.

## Awards

We were awarded with the **Highest Technical Achievement** by M. Bandecchi, Lead System Engineer at ESA.

## Report

Our report for the European Competition is included in this repository. You may read it for all the details about
the project.

[sCANSATi European Competition Report](report.pdf)
