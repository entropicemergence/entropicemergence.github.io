---
title: Best architecture for neural network compute, 
author: gesit
date: 2023-2-3 01:10:00 +0800
categories: [work, ai]
tags: [work] #has to be lowercase
render_with_liquid: false
---

Imagine a grid of 10k by 10k cell, each cell 100 nm square, the total area would be 1 square mm with 100 million cell. Each cell will be a weight parameter of the network, its should be made with a materials who have smi permanent property which is an increasing conductivity with more current applied to it, and a default state of decay toward less conductivity. Two or maybe all fours of the side quadrant will contain activation unit. The activation unit contain a leaky capacitor, if the capacitor reach a threshold voltage, it will be discharged(activated), thus further increasing the current that goes trough the active weight.

## Floating Gate Based Parameter

A floating gate is add additional charge storage into mosfet's gate, this charge pocket will determine how much resistance the mosfet will have. Every floating gate mosfet unit can become dual purpose weight parameter storage and computation. Suppose we put a capacitor at avery neural unit, the current required to charge the capacitor will depend on the voltage of the previous unit and floating gate charge content. A leaky capacitor will be our friend, because we want a certain tres hold voltage where capacitor will be discharged. A learning method where one can adjust the charge content inside the floating gate with accordance to how much current goes through the weight probably could work, this is analogous to a river system, where the depth and width of the river will vary automatically with how much water goes trough. Here temperature is our friend, because we need a mechanism where the weight will continuously decay, so the only activation pattern will be the most commonly recurring one. higher temperature will accelerate charge leakage from floating gate. 

Architecture such as this, in my estimation, could achieve one trillion parameter in 100 cm square for single layer floating gate, a 100 layer system such as in modern nand will achieve 100 trillion parameter, more than human brain. 


sbvfdnvb 










