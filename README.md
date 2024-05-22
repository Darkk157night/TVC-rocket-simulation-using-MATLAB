# TVC-rocket-simulation-using-MATLAB

![Main](https://github.com/Darkk157night/TVC-rocket-simulation-using-MATLAB/blob/main/Images/TVCmain.png)

## Intuition behind the model

MATLAB Simulink is a versatile software for simulation of various dynamic systems. The goal of my project was to accurately simulate a model Thrust Vectored Controlled (TVC) rocket and apply a PID control loop to get level stable flight. The model uses basic Simulink libraries along with the 3 Degree of freedom (3DOF) aerospace blockset which is the back bone of the entire simulation. 

A TVC rocket maintains it's stable flight by changing the angle of thrust vector mount in the X and Z (In this case) to maintain stable flight. The 

## Breaking down the model

### Thrust block
![Theust](https://github.com/Darkk157night/TVC-rocket-simulation-using-MATLAB/blob/main/Images/TVCthrust.png)

This block deals with the input to the system, here the input the system is assumed to be ideal constant thrust. The direction of the rocket’s magnitude vector is resolved into its vertical and horizontal vectors and then multiplied with the average thrust and feed into the 3DOF block, to simulate the force which acts on the moment arm the Center of mass values is also added.

### 3DOF Block
![3DOF](https://github.com/Darkk157night/TVC-rocket-simulation-using-MATLAB/blob/main/Images/TVC3DOF.png)

The 3DOF block form the aerospace blockset simulates a objects moves in air through the various differential equations governing movement, the thrust is given into this block along with the moment arm.

### PID Control block and Lag
![PID control](https://github.com/Darkk157night/TVC-rocket-simulation-using-MATLAB/blob/main/Images/TVCPID.png)

To simulate the time taken for the microcontroller and time for the servo to respond, these delay values are given and PID block is used here to take the servo angles and change them appropriately to make the system stable

## References
