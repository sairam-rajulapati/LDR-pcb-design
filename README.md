# LDR-pcb-design
Automatic Street Light System Using LDR (KiCad PCB Design).
this system is to optimize energy consumption by automatically controlling street lights based on ambient light conditions. The circuit detects daylight and darkness using an LDR sensor and switches the street light ON or OFF accordingly without human intervention.

## Table of Contents

1. [Introduction](#1-introduction)
2. [Methodology](#2-methodology)  
   - [schematic](#schematic)  
   - [Pcb layout](#pcblayout)
   - [3D view](#3dview)
3. [working](#working)
4. [circuit operation](#circuit)

   
# 1. Introduction
This project presents the design and implementation of an automatic street lighting system using a Light Dependent Resistor (LDR), developed and laid out using KiCad for schematic capture and PCB design.

The main objective of this system is to optimize energy consumption by automatically controlling street lights based on ambient light conditions. The circuit detects daylight and darkness using an LDR sensor and switches the street light ON or OFF accordingly without human intervention.

The project demonstrates practical skills in electronic circuit design, sensor integration, and PCB layout development, making it suitable for real-world smart lighting applications.

# 2. Methodology
## schematic
<img width="1327" height="847" alt="image" src="https://github.com/user-attachments/assets/e8bf3b9f-6110-4cce-ad19-d87d3677713c" />
## pcblayout
<img width="1172" height="802" alt="image" src="https://github.com/user-attachments/assets/61527970-fd5b-48df-ab80-14de982fe18f" />

## 3D view
<img width="1385" height="754" alt="LDR" src="https://github.com/user-attachments/assets/c1b842a1-7481-43d7-a4aa-bfc32b964b3f" />

## working
The system operates based on the light sensitivity property of the LDR:

The LDR (Light Dependent Resistor) changes its resistance depending on the intensity of light.

During daytime, when light intensity is high:

The LDR resistance decreases.

The voltage across the comparator/transistor circuit changes.

The switching device (transistor/relay) remains OFF, keeping the street light OFF.

During nighttime, when light intensity is low:

The LDR resistance increases.

This triggers the switching circuit.

The transistor or relay turns ON, activating the street light.

## circuit operation
The LDR is connected in a voltage divider configuration.

The output is fed into a transistor (or comparator like LM358/LM393).

The transistor acts as a switch:

Cut-off region → Light OFF

Saturation region → Light ON

An LED or street lamp (load) is connected as the output.

The entire circuit is implemented on a custom PCB designed in KiCad, including:

Schematic design

Component footprint assignment

PCB layout routing

Design rule checks (DRC)
