# Home Automation System with KNX and Zelio PLC

## Overview

This repository contains the technical documentation and project files for a home automation (domotics) physical simulation. The project was designed to learn and implement a smart home installation from scratch, integrating **KNX technology** with a **Zelio PLC**.

The system controls various household elements, including lighting, a motorized blind, and a smart plug, all manageable via a central multitouch interface.

> **Note on Language:** The original technical documentation (`Memoria_tècnica_KNX.pdf`) included in this repository is written in **Catalan**, as it was developed for a local academic project. However, the schematics, component lists, and software parameterizations are easily understandable for anyone familiar with KNX and PLC systems.

## Features

* **Centralized Control:** A Schneider Multitouch screen is used as the primary interface to manage the entire room's ecosystem.

* **Lighting Automation:** Independent control and dimming of multiple lighting circuits.

* **Motorized Blind Control:** Programmed ascent/descent times and blade rotation control.

* **Custom Scenes ("Party Mode"):** A programmed LADDER sequence to create synchronous lighting pulses (designed via Zelio Soft).

* **Robust Fallback:** The project demonstrates real-world troubleshooting; when the Zelio PLC faced last-minute technical constraints, the system was successfully adapted to operate via direct KNX manual controls.

## Tech Stack & Hardware

* **Protocol:** KNX

* **Software:**

  * ETS6 (for KNX parameterization and group addressing)

  * Zelio Soft 4.2.2 (LADDER programming)

* **Key Hardware (Schneider Electric):**

  * KNX Power Supply (MTN683832)

  * Multitouch Display (MTN6215-5910)

  * USB Communication Interface (MTN681829)

  * Dimming Actuator (MTN6710-0002)

  * Blind/Switch Master (MTN6705-0008)

  * Switch Actuator (MTN646808)

  * Binary Output 8S (MTN649204)

  * Zelio PLC

## Project Structure (Reference Document)

The attached PDF includes:

1. **Component Distribution & Electrical Plans:** Physical layout and wiring diagrams (KNX TP bus + traditional electrical wiring).

2. **Logical Distribution:** KNX group addresses and communication flow.

3. **Software Parameterization:** Detailed tables of ETS6 configurations for each device.

4. **Project Management:** Budget breakdown and Gantt chart planning.

## Authors

* Miquel Casals i Picornell

* Martí CS