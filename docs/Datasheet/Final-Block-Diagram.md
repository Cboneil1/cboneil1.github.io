Final Block Diagram for Microphone Input
![Block Diagram Schematic](Block_Team203_CarterONeill.jpg)
## Zip File  
[Download ZIP](./block.zip)
## Decision Process
For my subsection, there was a need to process the audio input for use in the other group member's subsystems. To address this need, I decided a few key processes needed implementation. First, the microphone needed to filter out wasteful signals and noise, since our focus was on the human voice. A low pass filter was developed to meet that need. It was set after the Op-Amp to reduce noise further. The Op-Amp is critical, because the electret microphone selected for the team board outputs a very weak signal. The ADC selected for this project was selected for its I2S communication pins. 

This selection meets our product requirements for both our goals, as well as our technical requirements as follows:

* Functions as an I2C communication sensing input
* Aides to educate on scientific concept of audio waves
* Allows for accessibility for children
* Aligns with technical goals of product requirements
* Can educate on basics, and not overwhelm
