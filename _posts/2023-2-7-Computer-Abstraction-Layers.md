---
title: Computer Abstraction Layer From Atoms
author: gesit
date: 2023-2-7 01:10:00 +0800
categories: [education]
tags: [computer, hardware] #has to be lowercase
render_with_liquid: false
---

Simulate  every component in this stack, differentiate by simulatability

Elements needed to build computers :
1. Silicon; 
2. 



Fundamental electronic components:
1. Mosfet, max frequency?, energy consumption curve?, theoretical minimum size in atoms? how its made into gates
2. Dram capacitor cell , how it connected, minimum latency, max frequency? capacitor leakage rate? temperature changes behavior ? 
3. Floating gate Cell, how it connected, manufacturing, maximum frequency ? minimum latency?, how much layer? how much level?
4. HDD, How it write and read data, materials?
5. Optical drive, how it actually write data? what materials it uses, laser wavelength? Layers?

Packaging technology :
1. Integrated circuit, how heat dissipate? how it connect to outside component?(ball joint, wire,), maximum number of layer?, design software?
2. Silicon interposer, maximum wire density?, manufacturing cost?, wire length-current-voltage-fet_driver_size relation?, maximum number of layer? design software
3. PCB, same as silicon interposer

Procesing Unit Design:
1. Instruction set, how it relates to machine code?, how it is implemented in silicon ROM?, how much die space it takes? how much x86, ARM, RISC V, GPU instruction has?   

Risc V is load and store architecture which clearly differentiate instrution into memory access(between memory and register), and ALU instruction which operate between register, ADD in RISC V are only between register, in x86 it could directly from memory.

An instruction may take several clock cycle to execute, which is controlled by control unit. To speed up the execution, the cpu will try to find implicit parallelism in i the machine code, and try to execute several different instruction in parallel, jump, or even discard an instruction. Every clock cycle the proccessor execute micro instruction, micro instruction will be unique in every proccesor architecture and may different across families of instruction set (two x86 architecture will have different micro instruction) , providing another abstraction layer.

How modern CPU work:
It will load hundreds of machine code line, then try to find the fastest way to execute it;
a. find the graph dependencies, then execute independent tree in parallel
b. speculative execution; guess the result of conditional (an if) operation, then execute the "do something" operation before the conditional calculation are completed, 

jim keller said that for modern cpu, the most important optimization is instruction predictability, branch  predictability amd data locality.



2. Cache, how much gate it takes? how addressing works? transistor density? max bandwidth? min latency? 
3. Register, how much in every processor?, what size it has? how its implemented in gate level?
4. Branch predictor, how its implemented in silicon? how its works? how instruction dropped ? 
5. Arithmetic Logic Unit, its throughput? how many clock cycle it takes ? 
6. What determine max frequency? transistor gate-drain voltage-time curve? pipe lining? silicon area influence?  
7. Memory controller, how data transfer works(is it serializing)?, how big the drive transistor? how much energy does a memory controller takes? what front side bus, hypertransport do? how much silicon does it takes? how much wire hbm, DDR, GDDR needs? why DDR has lower latency while it has longer path length? what makes communication very expensive bandwidth wise? why does it's very difficult latency wise?
8. PCI-E, same as memory controller, why does it takes so much die area?


Assembly Language, write and calculate it's throughput for various operation, GPU and CPU

C

C++

Javascript, Python









