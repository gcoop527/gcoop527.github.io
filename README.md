# George Coop Technical Portfolio

## Control Developments
I worked for Control Developments as a student electronics engineer from June 2021 - September 2022, as well as 8 weeks throughout 2023 and another 8 weeks throughout 2024.

What follows is the projects I worked on during my time there.


### CANView II
*Sector: Automotive/Military*

The original CANView was a vehicle display that would take messages from the CAN bus and provide the user with information about the vehicle, in addition to providing the capbility to manage other aspects of the car depending on customer needs. This includes brake lights, suspension controllers and our custom hydrostatic transmission controller.

We had tight deadline restrictions, so I implemented a modular software structure that let myself and a senior engineer work on the project simultaneously.
I mainly focused on the user interface.



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
  - Within this I created a graphics library to be used in-house

I also spent a large amount of time working on digital sampling and filtering to replace the current analogue system. This invovled utisilising the DSP features of the dsPICs, which goes down to optimising the assemble. 
While this wasn't used on this iteration of the product, it sets up a base for when we would want to significantly shrink the package size.

[Fluvia RC3](https://www.aqua-data.com/fluvia-rc3)

![image](https://github.com/user-attachments/assets/a42054f0-069d-4e58-807e-9972dc5985a0)

### RV4X

The RV4X is the probe that connects to the RC3, which contains the electrodes and the first stage of amplification. 

The potential on the electrodes is of ther oder of 100nV, with an impedance of ~10-500kΩ, which requires some precision amplification. 
This combined with strong, switching magnetic fields results in a complex problem to solve.

### Automotive Configurator
*Sector: Automotive*



### KowoLed Bright-Spot Non-Destructive Testing Viewer
*Sector: Civil and Mechanical Engineering*

The KowoLed Bright-Spot is a high-intensity lightbox used for inspecting x-ray film for non-destructive testing.

The goal of the project was to make the birghtest lightbox on the market with more technical features than our competitions.

Our system was 750W which allowed for a brightness of 15,000 Cd/m2 over all cells, or 1,000,000 Cd/m2 over a 2x2 hotspot which could be controlled using a touch screen interface and a Bluetooth footswitch. It has 60 individually controllable cells.

I worked on the software for the master controller which managed the other 5 controllers as well as the user interface. 

[KowoLed Bright-Spot](http://www.ie-ndt.co.uk/brightspot.html)

![image](https://github.com/user-attachments/assets/2a233b8f-054c-4d2e-82c5-915f073e739f)


## Oxford Uni Racing (Formula Student)
In my first year at university, I joined the team as an electronics team member, as I had a large amount of experience with this kind of work.

This including fixing many of the exisiting electronics hardware as well as completely re-writing the software for the vehicle control unit. 
This was a master system that connected to the CAN bus and coordinated information between the pedals, inverters, battery and dashboard. It also managed all the software based safety features that are required from the FSUK rules.

In June 2023 we took the car to Silverstone where we passed electrical scrutineering for the first time.

In my second year (23-24), I was Chief of Electronics, where I developed a small team's technical skills to be able to effectively work on the car. 
We had a goal to pass electrical scrutineering again with a minimal budget. This led to a focus on making software improvements, as well as integrating and tuning our new Sevcon GEN4 inverters. 
Unfortunately our chasis welding was signficiantly delayed, and despite our best efforts to work on the car, we could not finish it in time for the competition.

In my thrid (current) year, I've continued on as Chief of Electronics, where I am managing a complete hardware re-design, with a focus on reliablility.
My goal for the year is to pass electrical scrutineering with flying colours, and have our electronics package last us the next 2-3 years. 
This includes:
- Custom vehicle control unit
  - Multiple PWM output, Multiple Generic IO, 2x CAN, RS232 for diagnostic
  - Using STM32F446RC
  - Porting over the control code
- New TSAL System
  - Light system to display if the car is in a safe state or not
- New LV board within our battery
- Complete re-design of our harness using EPLAN.
  - Previous years harness has been, to be honest, poor.
  - Focus on investing in the right tools to do it properly.
- Focus on next years major design choices involving powertrain and battery options

![FS1](https://github.com/user-attachments/assets/3a37b0f9-7a89-464b-a3f5-c12747dc4045) ![FS2](https://github.com/user-attachments/assets/ad1223be-dbba-4b7d-860a-395628357d87) 
![FS3](https://github.com/user-attachments/assets/5a729187-9930-40f5-b807-faed4a753ba3)

