+++
showonlyimage = false
draft = false
image = "img/portfolio/filabot.png"
date = "2023-11-05T18:25:22+05:30"
title = "3D Printing Independent Study"
weight = 6
+++
For my Senior year independent study, I decided to get hands-on experience with the Filabot filament recycling system, as well as further my materials science skills by comparing material properties and print quality of 3D printed filaments.
<!--more-->

### What is Recycled PLA?
PLA, or Polylactic acid is the plastic most commonly used for 3D printing. It is a thermoplastic polymers derived from a renewable resource such as corn starch or sugar cane, which mean it is able to biodegrade and often referred to as a “bioplastic”. 

### PLA at Olin
PLA is one of the most common 3D printed plastic materials at Olin, and as we prototype, iterate, and learn we create a large amount of waste. To combat this, students in the Fall 2022 Materials Creation Consumption and Impact (MCCI) class used the Filabot recycling system to begin recycling some of this waste. 

### My Goals
I want to get hands-on experience with the Filabot filament recycling system, a continuation of the Fall 2022 Materials Creation Consumption and Impact class work, as well as further my materials science skills by comparing material properties and print quality of 3D printed filaments. 

![Filabot Image][1]

### Method
I started by isolating the main process variables in the recycling system. 
The first two are the inputs, how it is grinded and what materials were grinded. For all my tests, I printed sheets of Inland brand filament PLA in the color natural, also known as the filament with no additional colors or dyes. I grinded those sheets using the same modified paper shredder from the MCCI work, and used the resulting pellets to create all the filament for testing. 

The filabot system has multiple components, and many settings to modify. 

We start on the left with the hopper. The hopper melts all the pellets, and pushes them though a die to make the filament. The hopper has a few adjustable inputs, but the ones I modified were the temperature and the extrusion speed.

Next is the airpath, an array of fans with magnetic guides to cool the filament as it goes over it. This hardens the filament into it’s thickness at that moment. 

Last is the spooler, which consists of the spool wheel, driver roller, and inline measure. The spool wheel holds the new spool of filament and winds it. The drive roller pulls the filament taut. When the drive roller is faster, the filament is thinner, and when it is slower the filament is thicker. The drive roller in conjunction with extruder speed chooses the thickness and the airpath hardens it at that thickness. The inline measure measures the filament on one axis. 

The factors I modified were first temperature, and then drive roller, extruder, and fan speed as needed to get as close to the 1.75 mm filament width. The filaments I created were created under the following properties

![Filabot Table][2]
The Speeds on the Filabot are not numerically defined, they are defined as a knob with dash marks around it. To quantify them in my report/poster I chose to mark these as hours on a clock, a system that translates easily into circle positions without having to create weird definitions of start and end since its standardized.

### Results
The differential scanning calorimeter (DSC) is a thermal analysis apparatus that measures how physical properties of a sample change, along with temperature against time. I measured the PLA samples over a temperature range of 0 to 250°C. 

By simply overlaying the data from the 4 filaments, we can see there is a noticeable difference with the recycled PLA. 

![Filabot Graph][3]
 
I know something must have happened as the filament has been reheated twice more (once to print, and once to remelt and be extruded). Sadly there was not enough time for me to study this data and determine the exact reactions that the materials went through.

#### Secondary Results
Through the results in the table above (as well as my multiple testing iterations) I was able to confirm a direct relationship between extruder speed and variation of the diameter of the filament. The higher the extruder speed the more variation present in the filament.

[1]: /img/portfolio/filabot_long.png
[2]: /img/portfolio/filabot_table.png
[3]: /img/portfolio/filabot_graph.png
