# Physical-Design-of-Single-Port-RAM
This repository contains materials related to the RTL to GDS flow and single-port memory.
# Abstract:
This project aims to comprehensively understand the RTL (Register Transfer Level) to GDS (Graphic Data System) flow, a critical process in digital circuit design. The project covers every flow step, from RTL design using hardware description languages, and synthesis to gate-level representations, placement, and routing, to the final GDSII file generation. A significant portion of the project is dedicated to discussing the concept and theory of memory, with a particular focus on single-port memory.
# Contents
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
# ASIC Design Flow: Implementation of this Project from RTL to GDSII
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
# Let's get started
RTL Design: Understand how we converted the project specifications into RTL code using Verilog/VHDL.
RTL Simulation: Understand how we simulated the RTL code to verify the design functionality.
![Screenshot from 10-01-2024](https://github.com/user-attachments/assets/226160e7-fd16-4dac-a566-7fbc19218f56)
Logic Synthesis: Discover how we synthesized the RTL code into a gate-level netlist.

# Here is the graphical view:
![syn_img](https://github.com/user-attachments/assets/8884cf0b-8953-4613-b21b-4e2a0b206cc3)
Physical Design: Delve into the Place and Route process and how we created the final GDSII file.

# ASIC Physical Design Flow:
Welcome to our comprehensive guide on ASIC Physical Design Flow, also known as Netlist to GDSII Flow or PNR Flow. This guide is perfect for those who want to understand the practical aspects of chip creation.
# Let's get started
Design Import: This is the initial phase where the design data is imported into the physical design tools. When importing a design into Cadence Innovus, the following files are required:
1. Design Netlist File (Verilog): This file is created after the synthesis process and can either be generated using CADENCE Genus. Generally, it is a Modified Netlist, because I have to instantiate IOpad cells to the input and output port.
2. Physical Library Files (LEF Files): There are three kinds of LEF files required which are:
       1. Technology LEF File: This file contains information about the Metal layers, Vias, design rules, etc. for a certain technology.
       2. Standard Cell LEF File: This file contains the physical view of the standard cells of the current technology.
       3. IO Cell LEF File: This file contains the physical view of the IO cells, corner cells, IO fillers of the current technology.

# Floorplan (includes Powerplan): 
In this step, the layout of the chip is planned, including the placement of blocks and the power distribution network.
# Placement & Place Opt: 
After floorplanning, the components of the design are placed onto the layout, and their positions are optimized for performance and other factors.
# Clock Tree Synthesis & CTS Opt: 
This involves building a clock distribution network (clock tree) across the chip and optimizing it to ensure that all elements receive the clock signal on time, and check.
# Routing & Route Opt: 
The final step involves connecting the components with wires (routing) and optimizing the wire paths to minimize delays and other issues.

# Final Result of the Flow:
Final layout before and after translating the GDS stream file into Cadence Virtuoso.
![Screenshort 14-01-2024](https://github.com/user-attachments/assets/fc55efb8-58c9-4592-b79c-dee55d0fe4e4)
![Screenshort 15-01-2024](https://github.com/user-attachments/assets/842bef5f-9efc-4cd0-b978-baf4739d71be)





   





   
