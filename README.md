# George Coop Technical Portfolio

## Control Developments
I worked for Control Developments as a student electronics engineer from June 2021 - September 2022, as well as 8 weeks throughout 2023 and another 8 weeks throughout 2024.

What follows is the projects I worked on during my time there.


### CANView II
*Sector: Automotive/Military*

The original CANView was a vehicle display that would take messages from the CAN bus and provide the user with information about the vehicle, in addition to providing the capbility to manage other aspects of the car depending on customer needs. This includes brake lights, suspension controllers and our custom hydrostatic transmission controller.



### Fluvia RC3X
*Sector: Hydrology*

The Fluvia RC3 is a touch scren device that connects to a water velocity probe to provide a user-interface to take depth, velocity and flow measurement.

It contains the precision current source and analogue sensing circuit to operate the probe. In addition, it can store data logs and convert veocity measurements to flow after providing a river/ conduit profile. Additional features include GPS and the option to upload data to a PC via serial / Bluetooth.

Due to the major component shortage following COVID, I led a complete, independent hardware and software redesign to ensure uninterrupted customer supply. This was called the RC3x. This was also an opportunity to switch to more modern components and make improvements.

This included:
- Eliminating the need for a single-source battery, allowing for 20% extended battery capacity
- Increasing velocity refresh rate from 1Hz to 10Hz due to software optimisations
- 7500 lines of C code
- 2 Processor system communication via UART
- Creating a multi-purpose graphics controller board, with a custom hardware and middlewear abstraction layers

I also spent a large amoutn of time working on digital sampling and filtering to replace the current analogue system. This invovled optimising down to processor specific optimisations. 

[Fluvia RC3](https://www.aqua-data.com/fluvia-rc3)




### Automotive Configurator
*Sector: Automotive*

### KowoLed Bright-Spot Non-Destructive Testing Viewer
*Sector:: Civil and Mechanical Engineering*

The KowoLed Bright-Spot is a high-intensity lightbox used for inspecting x-ray film for non-destructive testing.

The goal of the project was to make the birghtest lightbox on the market with more technical features than our competitions.

Our system was 750W which allowed for a brightness of 15,000 Cd/m2 over all cells, or 1,000,000 Cd/m2 over a 2x2 hotspot which could be controlled using a touch screen interface and a Bluetooth footswitch. It has 60 individually controllable cells.

I worked on the software for the master controller which managed the other 5 controllers as well as the user interface. 

[KowoLed Bright-Spot](http://www.ie-ndt.co.uk/brightspot.html)

## Oxford Uni Racing (Formula Student)
In my first year at university, I joined the team as an electronics team member, as I had a large amount of experience with this kind of work.

This including fixing many of the exisiting electronics hardware as well as completely re-writing the software for the vehicle control unit. 
This was a master system that connected to the CAN bus and coordinated information between the pedals, inverters, battery and dashboard. It also managed all the software based safety features that are required from the FSUK rules.

In June 2023 we took the car to Silverstone where we passed electrical scrutineering for the first time.

In my second year, I was Chief of Electronics, where I managed

