---
title: Schematic For Audio Input PCB
---

## Image 1: Carter ONeill's Schematic for Team 203
![Screenshot](EGR314_CarterONeill_Schematic1.jpg)
My schematic satisfies the needs of the k-12 children expected to use this equipment by providing them a means of interacting with our model vocally. The inclusion of a simple low fidelity microphone allows for raw self expression. Requirements for our group project are to include one sensor subsystem which communicates to my micro-controller via I2C, and with the inclusion of the ADC I take the input signal from the amp and output to my micro-controller with I2C as intended. 
## PDF Link
[Open PDF](./EGR314_CarterONeill_Schematic1.pdf)
## Zip File  
[Download ZIP](./EGR314_CARTERONEILL00.zip)
## Power Budget
![Screenshot](PowerBudgetNew.jpg)
## Zip File  
[Download ZIP](./Power_Budget_Carter.zip)

The power budget highlights how efficient my system is, and demonstrates the need for a switching regulator. Running a linear regulator with this setup would generate a lot of heat. The components I am using will likely be lower energy than calculated here, in the tens of milliamps, due to the majority of accessories being excluded from use. 