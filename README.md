# Physical-Design-of-Single-Port-RAM
This repository contains materials related to the RTL to GDS flow and single-port memory.
# Abstract:
This project aims to comprehensively understand the RTL (Register Transfer Level) to GDS (Graphic Data System) flow, a critical process in digital circuit design. The project covers every flow step, from RTL design using hardware description languages, synthesis to gate-level representations, placement, and routing, to the final GDSII file generation. A significant portion of the project is dedicated to discussing the concept and theory of memory, with a particular focus on single-port memory.
# Contennts
1. Single-Port Memory:
2. ASIC Flow (RTL to GDS Flow):

# Getting Started
#Single-Port Memory Module
#Introduction
This repository contains a Verilog module for a single-port memory. This type of memory is a fundamental component in digital systems, allowing data to be read from and written to a single memory location (address) at a time.
# Theory
A single-port RAM (Random Access Memory) is a simple form of memory that provides a basic storage mechanism for digital systems. Each memory location in a single-port RAM can store a fixed number of bits (usually a power of 2, such as 8, 16, 32, etc.). During a read operation, the data stored at a specific address is retrieved. During a write operation, new data is stored at a specific address, replacing the previous data.

The term "single-port" comes from the fact that this type of RAM has only one data port, which means that read and write operations cannot occur simultaneously at different addresses. If a write operation is in progress, a read operation must wait, and vice versa.
# Working Principle
The single-port memory module operates on the rising edge of the clock signal. If a write operation is in progress (signaled by the we control signal), the data at the specified address is updated. If a read operation is in progress (signaled by the absence of the we control signal), the data from the specified address is loaded into a temporary register.
The data output is controlled by the oe (output enable) control signal. If output is enabled and no write operation is in progress, the data from the temporary register is output.
# ASIC Design Flow:Implementation of this Project from RTL to GDSII
#Content Overview
1. RTL Design
2. RTL Simulation
3. Logic Synthesis
4. Physical Design
       Design Import
       Floorplan (includes Power plan)
       Placement & Place Opt
       Clock Tree Synthesis & CTS Opt
       Routing & Route Opt
#    

   
