# Motor Control Project
This project was part of Northwestern's Basic Mechatronics (ME333) course.

### Author: Anuj Karnik.

### Overview:
This project dealt with creating a smart motor controller.<br>
The user was able to communicate with the system via a simple GUI on MATLAB.<br>
The motor controller could be tasked to work in position or velocity control mode.<br>
It could even execute step or cubic trajectories depending on the user's choise.<br>

### Hardware:
1. NU32 development board with a PIC32MX795F512H microcontroller.
2. A generic brushed DC motor with an incremental encoder.
3. A MAX9918 current sensing amplifier.
4. A DRV8835 H-bridge.
5. n-Scope signal analyser.

### System Architecture:
The high-level system architecture can be seen in the diagram below:
![system architecture](images/mc3.jpeg).

### File Structure Details:
├── adc.c --> functions related to Analog to Digital conversion. <br>
├── adc.h<br>
├── client.m --> client file to run on MATLAB.<br>
├── currentcontrol.c --> current control functions<br>
├── currentcontrol.h<br>
├── encoder.c --> functions to read data from the encoder <br>
├── encoder.h<br>
├── genRef.m <br>
├── images<br>
│   ├── mc3.jpeg<br>
│   ├── mc4.jpeg<br>
│   └── mc5.jpeg<br>
├── main.c --> main function<br>
├── NU32bootloaded.ld --> bootloader<br>
├── NU32.c <br>
├── NU32.h<br>
├── positioncontrol.c --> functions related to position control mode<br>
├── positioncontrol.h
├── pwm.c --> functions related to PWM generation<br>
├── pwm.h<br>
├── README.md <br>
├── read_plot_matrix.m<br>
├── timer.c<br>
├── timer.h<br>
├── utilities.c<br>
└── utilities.h<br>

### Results:
The results of the step and cubic trajectories are shown below:
![step trajectory](images/mc4.jpeg).
![cubic trajectory](images/mc5.jpeg)

<br><br>
For a more detailed description and some videos, check out my [portfolio](https://sites.google.com/u.northwestern.edu/anuj-karnik/projects/advanced-mechatronics?authuser=0).

